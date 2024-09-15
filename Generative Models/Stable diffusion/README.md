## How diffusion model works
A diffusion model is conceptually quite simple. We start with images and progressively add noise to them, gradually corrupting the original data. The model is then trained to reverse this process, learning to reconstruct the original images from the noisy versions. Once trained, the model is capable of generating or reconstructing images even from purely random noise. Essentially, the model learns to denoise data step by step, enabling it to generate realistic outputs from noise during inference.


# REST Stable Repos
* https://github.com/CompVis/stable-diffusion?tab=readme-ov-file