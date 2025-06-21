# 🧪 Assignment: Variational Autoencoder with Encoder-Decoder Architectures

## 📌 Objective

Explore the effect of using **encoder-decoder architectures** within a **Variational Autoencoder (VAE)** framework. This week, we will:
- Build a standard VAE.
- Modify the encoder and/or decoder to follow an encoder-decoder sub-structure.
- Compare reconstruction quality and latent space representations.
- Analyze and report which structure works best.

---

## 🧱 VAE Architecture Overview

A **Variational Autoencoder (VAE)** normally has two main components:
- **Encoder**: Compresses the input data into a latent distribution.
- **Decoder**: Samples from this latent space to reconstruct the data.

### ➕ Extension: Encoder-Decoder Inside VAE

An **encoder-decoder architecture** has layers with:
- Decreasing size → bottleneck → increasing size.
- Think of it as downsampling then upsampling within a component (not just across encoder and decoder).

---

## 🔧 Task A – Implementing VAE Variants

You will implement **four VAE variants**:

### A.1 – Basic VAE (Baseline)
- Standard VAE with:
  - Encoder → [200, 100, 50]
  - Latent space
  - Decoder → [50, 100, 200]

### A.2 – Encoder Side as Encoder-Decoder
- Replace the **encoder** with an encoder-decoder structure.
  - Downsample → Upsample → Latent
- Decoder remains the same.

### A.3 – Decoder Side as Encoder-Decoder
- Encoder is standard.
- Replace the **decoder** with an encoder-decoder structure:
  - Latent → Downsample → Upsample → Output

### A.4 – Both Sides as Encoder-Decoder
- Both encoder and decoder use encoder-decoder sub-architectures.

---

## 📊 Task B – Evaluation and Comparison

### B.1 – Metrics
- Use metrics like:
  - Reconstruction Loss (MSE or BCE)
  - KL Divergence
  - Total VAE Loss

### B.2 – Visual Output
- Display 10 reconstructed images for each variant.

### B.3 – Analysis
- Write a brief report (~200 words):
  - Which architecture performed best and why?
  - Trade-offs (e.g., training time, complexity, overfitting).
  - Effect on reconstruction quality and latent representations.

---

## 💡 Hints and Resources

- Use TensorFlow/Keras for quick prototyping.
- You can choose **Dense** or **Conv** layers (or both).
- Examples of encoder-decoder architectures:
  - [SegNet](https://mi.eng.cam.ac.uk/projects/segnet/)
  - U-Net
  - Autoencoders with symmetrical structures

---

## 📁 Submission Guidelines

- Submit:
  - `vae_variants.ipynb` or `vae_variants.py`, containing the variations of autoencoders
  - `assignment.md` (this file, with Part B filled in)


---

Feel free to reach out on the discussion board for any clarifications or troubleshooting help.
