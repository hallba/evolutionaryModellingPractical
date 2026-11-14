Getting started

This practical uses conda and pip to manage packages. The key package for
simulations is taken from here: 

https://github.com/michaelhall28/clone-competition-simulation

environment.yml contains the conda packages needed to run the code. There
are however some other prerequisites that need to be installed from 
elsewhere depending on your operating system. If you are using windows, 
it is recommended you install ubuntu on windows subsystems for linux (WSL)
and follow ubuntu linux instructions.

To install the conda packages and activate the environment, run 

 conda env create -f environment.yml && conda activate evoPractical

This should install all needed packages; the additional steps below are only necessary
if something is not available.

Ubuntu linux

Install ffmpeg and gsl using the apt package management system.

 sudo apt install ffmpeg gsl-dev

If using another linux variant, these packages should be available through
your local package manager.

Mac

Install ffmpeg and gsl using MacPorts
 
 sudo port install gsl ffmpeg

Conda and pip packages

Once system wide tools are installed, create a conda environment as below

 conda env create --name somaticEvolutionPractical

Then install the clone competition library

 pip install clone-competition-simulation

Working through the practical

The practical is structured as a series of jupyter notebooks to be worked 
through as below

- Introduction
- Simple models
- Fitting models
- Exploring competition and epistasis

Each notebook contains questions and missing code sections. There are no
set answers but each should be worked through to enforce learning.
