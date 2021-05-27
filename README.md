# Single-neuron convexification for binarized neural networks

This repository is the official implementation of [Single-neuron convexification for binarized neural
networks](https://arxiv.org/abs/2030.12345). The codes are divided into two parts -- BNN training and robustness verifying. It is easy to run them in Jupyter Notebook.

## Requirements
- A commercial mathematical programming solver [Gurobi 9.1](https://www.gurobi.com/) is required to install. It is free for academic users.
- The python dependency file for anaconda is provided in [environment.yml](./environment.yml).

## BNN Training

To train a BNN, implement [training.ipynb](./training.ipynb) using Jupyter Notebook or Google Colab Notebook. You can also download the weights for pretrained models [here](./weights_for_trained_BNN.zip) trained on MNST. The accuracy of the trained BNN for each configuration is also provided in the file accuracy.txt.

## BNN Robustness Verifying

We formulate the problem of BNN robustness verifying as a mixed integer program (MIP) or its convex relaxation.  One can implement [verifier_h1.ipynb](./verifier_h1.ipynb) and [verifier_h2.ipynb](./verifier_h2.ipynb) using Jupyter Notebook. 

