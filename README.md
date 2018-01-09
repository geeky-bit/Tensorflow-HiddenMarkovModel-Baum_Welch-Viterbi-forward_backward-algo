**Note :: Most of the functions used are adapted from some other github repos and some online materials.


# Hidden Markov Model (Implementation using the computation graphs in TensorFlow)

## Jupyter Notebook:
These are some of the examples that I have included in the jupyter notebook. Feel free to add more.

## Baum Welch Algorithm
* Expectation Maximization Inference of unknown parameters of a Hidden Markov Model

## Viterbi Algorithm
* Efficient way of finding the most likely state sequence.
* Method is general statistical framework of compound decision theory. 
* Maximizes a posteriori probability recursively.
* Assumed to have a finite-state discrete-time Markov process.

## Forward-Backward Algorithm
* The goal of the forward-backward algorithm is to find the conditional distribution over hidden states given the data.
* It is used to find the most likely state for any point in time.
* It cannot, however, be used to find the most likely sequence of states (see Viterbi)

### Differences ::
The Baum-Welch algorithm and the Viterbi algorithm calculate different things.

***Use Viterbi : The Viterbi training algorithm (as opposed to the "Viterbi algorithm") approximates the MLE to achieve a gain in speed at the cost of accuracy***
 * known : transition probabilities for the hidden part of your model
 * known : emission probabilities for the visible outputs of your model
 * Gives : the most likely complete sequence of hidden states conditional on both your outputs and your model specification.


 ***Use Baum-Welch :  The Baum-Welch algorithm is essentially the Expectation-Maximization algorithm applied to a HMM***
 ***Gives ::***  
* The most likely hidden transition probabilities
* The most likely set of emission probabilities given only the observed states of the model (and, usually, an upper bound on the number of hidden states)

***Tip : If you know your model and just want the latent states, then there is no reason to use the Baum-Welch algorithm. 
If you don't know your model, then you can't be using the Viterbi algorithm.***


***Note : The codes are freely available. Please feel free to add more codes. Spread the word!***
