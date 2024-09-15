# Introduction

# Autoencoders (AE)

# (Cond) Variational Autoencoders (VAE) TODO
A Conditional Variational Autoencoder (cVAE) is a generative model that extends the basic VAE architecture by incorporating conditional information, allowing for controlled generation of data based on specific attributes.

**Conditional**: A class label or other condition is appended to the latent space, guiding the generation process and specifying what type of data to generate.

**Autoencoder**: It consists of an encoder and a decoder. The encoder compresses the input data into a latent space, while the decoder reconstructs the data from the latent representation.

**Variational**: The latent space is sampled from a normal distribution N(0, I). The encoder is trained to make the latent representations approximate this distribution through the use of Kullback-Leibler divergence. This regularization ensures that the latent space is smooth and allows for sampling new data points during generation.

The goal of the cVAE is to learn meaningful features of the data (in the latent space) and use these features, along with random variations, to generate new, similar data based on the given condition.


## Generative Adversarial Networks (GAN)
GANs consisting of two neural networks: a generator and a discriminator, which are trained together in a competitive process.

**Generator**: Its role is to create images that are as similar as possible to those from the training dataset. It starts from random noise, typically sampled from a normal distribution (N(0, I)), and tries to generate realistic images to deceive the discriminator.

**Discriminator**: This network attempts to distinguish between real images from the training set and the fake images produced by the generator. It acts as a critic, providing feedback to the generator about the quality of the generated images.

The training is adversarial: the generator improves by trying to "fool" the discriminator, while the discriminator improves by getting better at identifying fake images. Gradients are propagated through both networks so that the generator learns how to adjust its output.

In many cases, GANs can be conditional, meaning additional information (like class labels) is provided to both networks to guide the generation process.

However, GANs are known for having a difficult loss function, and training can be unstable. The generator and discriminator pull in opposite directions, and if one becomes significantly stronger than the other, the model may not converge properly.


**Stitch it in Time: GAN-Based Facial Editing of Real Videos**:
*https://stitch-time.github.io/

# Conditional GANs (Pix2Pix, CycleGAN)

## Diffusion Models
We teach the model to de-noise images:
* we have some training set and slowly noise it (step by step more and more)
* we teach the model to reproduce the originals
* can also be conditioned
* 
**Denoising Diffusion Probabilistic Models**:
* https://arxiv.org/abs/2006.11239

# Dall-E

## Intresting
**Difference between AutoEncoder (AE) and Variational AutoEncoder (VAE)**:
* https://towardsdatascience.com/difference-between-autoencoder-ae-and-variational-autoencoder-vae-ed7be1c038f2 




