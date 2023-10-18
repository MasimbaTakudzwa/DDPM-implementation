# UndergraduateDiffusionModel

Abstract
Diffusion probabilistic models are a part of a family of deep generative models that are used to synthesise high quality images. This paper details an
attempt to implement this type of generative model to synthesise high quality images. This class of generative models were inspired by considerations
of non equilibrium thermodynamics. 

 Introduction
There are a number of different models that can be used for artificial image generation. Each
model has different strength and weaknesses. Most of these models are able to yield high
quality samples in a number of data modalities. Generative Adversarial Networks (GANs),
Auto-regressive Models, Flows and Variational Auto-encoders (VAEs) have all demonstrated
the ability to synthesise incredibly high quality image samples. In this paper I present an
implementation of a Diffusion Probabilistic Model (also known as Diffusion models) based
on the paper written by Jonathan Ho and colleagues in 2020 titled, ”Denoising Diffusion
Probabilistic Models”. The aim of this implementation was to synthesise images of similar
quality of the ones presented by Jonathan Ho but at lower resolutions of 128x128 or 94x94
on the STL10 Data set. A diffusion probabilistic model (diffusion model) is a parameterized
Markov chain trained using variational inference to produce samples matching the data
after finite time (Ho et al., 2020). By using this chain the aim is to teach a neural network
to reverse the forward diffusion process that is iteratively applied to the images until they
reach a perfect Gaussian distribution.

The first draft of the full paper is availble in the repo
