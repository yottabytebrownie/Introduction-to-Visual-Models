# Diffusion Model Assignment

## Objective
- Implement the diffusion model from the video for CIFAR-10.
- Train with two sets of hyperparameters and compare results.
- Start with partially noised samples and analyze the denoising process.

## Tasks

1. **Implement Diffusion Model**  
   - Build a model that adds noise to an image and learns to denoise it.

2. **Hyperparameter Tuning**  
   - Train with 2 sets of hyperparameters (learning rate, noising schedule β, denoising steps).
   - Plot loss curves and justify parameter choices.

3. **Sample Generation**  
   - Generate 1 sample per class (CIFAR-10, 10 classes) after training.

4. **Partially Noised Samples**  
   - Denoise a partially noised sample (50, 10, and 5 iterations of noise).
   - Comment on denoising ability and any new features/shapes added during recovery.

## TO SUBMIT
- Code (including model architecture, training, and denoising process).
- Loss curves for both hyperparameter settings.
- 10 CIFAR-10 samples, one per class.
- Observations on denoising for partially noised samples
