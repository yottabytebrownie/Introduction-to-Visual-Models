# Diffusion models
## Video Resources
* [what are diffusion models](https://www.youtube.com/watch?v=fbLgFrlTnGU)
* [how AI image generators work](https://www.youtube.com/watch?v=1CIpzeNxIhU)
* [diffusion implementation](https://www.youtube.com/watch?v=XTs7M6TSK9I)

Diffusion models are a class of generative models that simulate the process of adding and removing noise to generate data.
They have gained prominence for their ability to generate high-quality data, especially in fields like image and speech generation.

The process involves two main stages: forward diffusion and reverse diffusion. In the forward process, noise is gradually added to the data, transforming it into pure noise. The reverse process involves a neural network that learns to remove this noise step-by-step, reconstructing the original data or generating new samples. This is achieved by minimizing a loss function that measures the difference between actual and predicted noise.

Mathematically, the forward process can be represented as:

`x_t = \sqrt{1 - \beta_t} x_{t-1} + \sqrt{\beta_t} \epsilon`
Here, `β_t` controls the noise schedule, and `ε` is Gaussian noise. The reverse process uses a neural network to approximate the conditional probability of denoising.

## Applications
1. Image Generation: Producing high-quality images from noise, often conditioned on text prompts.

2. Image Super-Resolution: Enhancing image resolution.

3. Image Inpainting: Filling in missing or degraded parts of an image.

4. Speech Synthesis: Generating human-like audio signals.

5. Anomaly Detection: Identifying deviations from normal data distributions.

## Advantages
1. Stable Training: Unlike GANs, they avoid issues like [mode collapse](https://www.geeksforgeeks.org/machine-learning/modal-collapse-in-gans/#:~:text=Modal%20collapse%20in%20GANs%20(Generative%20Adversarial%20Networks)%20occurs,the%20full%20diversity%20of%20the%20real%20data%20distribution.).

2. High-Quality Outputs: They often surpass GANs in generating realistic samples.

3. Flexibility: Capable of modeling complex data distributions.

4. Robustness: Less sensitive to hyperparameter changes.

## Limitations
1. Computational Intensity: Training and sampling require significant resources due to iterative steps.

2. Slow Sampling: Generating a single sample involves multiple reverse diffusion steps.

3. Complexity: Their architecture and training process can be challenging to implement and understand.
