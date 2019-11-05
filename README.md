# RNN-tv-script-generation

The purpose of this project is to develop a *Recurrent neural network (RNN)* for generate a "fake" TV scripts based on patterns it recognizes in this training data and is my *third project* of the [*Udacity Deep Learning Nanodegree program*](https://www.udacity.com/course/deep-learning-nanodegree--nd101).

## Installation

This project is based on [Pytorch](https://pytorch.org/) and [Jupyter notebook](https://jupyter.org/). All the installation process are handled by [Anaconda](https://www.anaconda.com/), one of the the most popular ***Data Science platform***, so is quite straightforward.

Download and install the ***Anaconda platform*** for the OS and architecture in use:

    $ wget https://repo.anaconda.com/archive/Anaconda3-2019.03-Linux-x86_64.sh
    $ ./Anaconda3-2019.03-Linux-x86_64.sh

Create an ***Anaconda environment*** for the project based on Python 3.6:

    $ conda install python=3.6.8
    $ conda create -n tvscript python=3.6
    $ conda activate tvscript

Install all the ***required dependencies*** always using Anaconda (in this case without GPU support):

    $ conda install -c conda-forge matplotlib
    $ conda install numpy jupyter notebook
    $ conda install pytorch-cpu torchvision-cpu -c pytorch

## Dataset

The ***dataset*** used for training and testing are based on the original [*Seinfeld NBC TV Series*](https://en.wikipedia.org/wiki/Seinfeld) scripts, is maintained by Aman Shrivastava and available from [Kaggle](https://www.kaggle.com/thec03u5/seinfeld-chronicles).

## Goal

The aim of the project is to **Pre-process** the input dataset, **build an RNN** using Pytorch, **tune** the hyperparameters for the application, **train** the network achieving a loss *less than 3.5* and finally generate a **new script** using the trained *RNN* that should look structurally similar to the TV script in the dataset.
