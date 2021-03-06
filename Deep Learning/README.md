# Variable Importance for Bayesian Neural Networks

Here, we demonstrate how to implement RATE with Bayesian neural network architectures as described in [Ish-Horowicz et al. (2019)](https://arxiv.org/abs/1901.09839). The `Notebooks` directory contains notebooks used to generate the results and plots in the paper. These are meant to serve as examples of how to build and train Bayesian neural networks and determine variable importance for its input features.

The source code in the `src` directory is organized as follows:
* `BayesNN.py` contains a class implementing the Bayesian neural network.
* `rate_bnn.py` contains code for computing RATE values for a Bayesian neural network.
* `utils.py` contains functions for loading data and computing accuracies across Monte Carlo sampled predictions.
