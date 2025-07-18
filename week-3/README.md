# Week 3: Building and Exploring Autoencoders with TensorFlow

## Objectives
In this week, you will:

- Understand the concept and architecture of autoencoders.
- Build and train various types of autoencoders using TensorFlow.
- Apply autoencoders to tasks like noise reduction, dimensionality reduction, and data generation.
- Explore Variational Autoencoders (VAEs) and their generative capabilities.
- Compare types of autoencoders: Vanilla, Denoising, Sparse, and Variational.

---

## Topics Covered

### 1. Introduction to Autoencoders
- Learn the basic structure: encoder, bottleneck, and decoder.
- Understand the reconstruction loss (e.g., MSE, binary cross-entropy).
- Explore use cases: data compression, denoising, anomaly detection.
- **Resource**:
  [VAEs explained!](https://www.youtube.com/watch?v=fcvYpzHmhvA)
  [YT playlist](https://www.youtube.com/playlist?list=PLyFpZIg7OtNRRcaOEdmiz1WEd97VHqfd6)

---

### 2. Vanilla Autoencoders with TensorFlow
- Build a simple autoencoder using the MNIST dataset.
- Use Dense layers for compression and reconstruction.
- Visualize original vs reconstructed images.
- **Tutorial**: [TensorFlow Autoencoder Guide](https://www.tensorflow.org/tutorials/generative/autoencoder)

---

### 3. Denoising Autoencoders
- Learn to add noise to inputs and train the autoencoder to recover clean data.
- Understand the robustness benefits in image reconstruction tasks.
- **Code Example**: [Denoising Autoencoder](https://www.geeksforgeeks.org/machine-learning/denoising-autoencoders-in-machine-learning/)

---

### 4. Variational Autoencoders (VAEs)
- Learn how VAEs model the latent space probabilistically.
- Use sampling and KL divergence in the loss function.
- Generate new data (e.g., handwritten digits).
-  **Tutorial**: [Variational Autoencoder with TensorFlow](https://www.tensorflow.org/tutorials/generative/cvae)

---

### 5. Visualization of Latent Space
- Use t-SNE or PCA to visualize compressed data representations.
- Compare latent space clustering for different types of autoencoders.
-  **Tool**: [Scikit-learn t-SNE Guide](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)

---

### 6. Optional: Autoencoders for Anomaly Detection
- Train on normal data and detect anomalies by reconstruction error.
- Apply to fields like fraud detection or medical imaging.
-  **Tutorial**: [Anomaly Detection with Autoencoders (TensorFlow)](https://www.tensorflow.org/tutorials/generative/autoencoder#anomaly_detection)

---

## Additional Resources

-  **Video**: [What are Autoencoders? - StatQuest](https://www.youtube.com/watch?v=9zKuYvjFFS8)

---

## Optional: Image Segmentation with U-Net
- Explore the U-Net architecture for semantic segmentation.
- Commonly used in biomedical image analysis.
-  **Code**: [U-Net Implementation (GitHub)](https://github.com/zhixuhao/unet)

