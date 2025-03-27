# DDPM
This repository contains an implementation of a Denoising Diffusion Probabilistic Model (DDPM) built from scratch using PyTorch. The project aims to generate images by modeling the gradual denoising of noise into structured data, following the methodology introduced in the paper "Denoising Diffusion Probabilistic Models" by Ho et al. (2020). 
The implementation is designed with modularity and clarity in mind, using Jupyter Notebooks to facilitate experimentation and understanding. The project is structured as follows:
Dataset: MNIST is used as the initial dataset, loaded and preprocessed via a custom DataLoader.

Forward Process: A noise scheduler progressively adds Gaussian noise to images over a series of timesteps, following a linear variance schedule.

Time-Step Embedding: Sinusoidal positional encodings are employed to represent timesteps, processed through an MLP for integration into the model.

Configuration: Hyperparameters (e.g., number of timesteps, noise schedule) are managed in a config.yaml file for easy customization.

