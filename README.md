# MCMCsim: Markov chain Monte Carlo simulation toolkit for julia

[![Build Status](https://travis-ci.org/drbjsmith/MCMCSim.jl.png)](https://travis-ci.org/drbjsmith/MCMCSim.jl)

`MCMCsim` is a programming environment and toolset for the implementation and inference of Bayesian models using Markov chain Monte Carlo (MCMC) sampling.  The package provides a framework for (1) specification of hierarchical models through stated relationships between data, parameters, and statistical distributions; (2) block-updating of parameters with samplers provided, defined by the user, or available from other packages; (3) execution of MCMC sampling schemes, and (4) posterior inference.  It is designed to give users access to all levels of the design and implementation of MCMC simulators to particularly aid in the development of complex models.


## Features

`MCMCsim` is designed to

* Have an intuitive, interactive, and extensible interface.
* Accommodate a wide range of model and distributional specifications.
* Let all interactions with the software be made through a single, interpreted programming language.
  * Any julia operator, function, type, or package can be used for model specification.
  * Custom distributions and samplers can be written in julia to extend the package.
* Allow the arbitrary blocking of model parameters and designation of block-specific samplers.
* Provide samplers that can be used with the included simulation engine or apart from it.
* Give command-line access to all package functionality, including its simulation API.
* Produce run-time performance on-par with or better than established MCMC software.
