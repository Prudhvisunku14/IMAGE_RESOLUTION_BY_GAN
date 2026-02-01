

# 🖼️ Image Super-Resolution using CNN and GAN

## 📌 Overview

This project focuses on enhancing **low-resolution images into high-resolution images** using two deep learning techniques:

* **Convolutional Neural Network (CNN / SRCNN)**
* **Generative Adversarial Network (GAN / SRGAN)**

The objective is to **compare pixel-based super-resolution and perceptual super-resolution** by analyzing visual quality and texture reconstruction in the generated images.

---

## 🚀 Key Features

* Super-resolution using **CNN (SRCNN)**
* Perceptual image enhancement using **GAN (SRGAN)**
* Side-by-side visual comparison of CNN and GAN outputs
* Improved reconstruction of edges, textures, and fine details
* 4× image upscaling (22×22 → 88×88)

---

## 🧠 Methods Used

### 🔹 CNN-Based Super-Resolution (SRCNN)

* Learns **pixel-to-pixel mapping** between low-resolution and high-resolution images
* Trained using **reconstruction loss** (MSE/L1)
* Produces **smooth and stable** outputs with reduced noise
* Effective for basic resolution enhancement

---

### 🔹 GAN-Based Super-Resolution (SRGAN)

* Uses a **Generator–Discriminator** adversarial framework
* Generator learns to produce high-resolution images
* Discriminator differentiates between real and generated images
* Optimized using **adversarial loss + content loss**
* Produces **sharper images with richer textures and better perceptual quality**

---

## 🏗️ Model Architecture

### 🔸 CNN Model

* **Input:** Low-resolution image
* **Architecture:** Multiple convolutional layers with non-linear activations
* **Output:** High-resolution reconstructed image

---

### 🔸 GAN Model

* **Generator:** Residual blocks followed by upsampling layers
* **Discriminator:** CNN-based binary classifier to distinguish real and generated images

---





## 📊 Results

The proposed super-resolution models were evaluated by converting **low-resolution images of size 22×22 pixels into high-resolution images of size 88×88 pixels (4× upscaling)**.
<img width="924" height="268" alt="RRR" src="https://github.com/user-attachments/assets/3d3c35b7-79ac-4365-8612-b4357335c8ee" />
### 🔹 CNN (SRCNN) Results

The CNN-based model successfully improves spatial resolution and recovers the overall structure of the image. The output images are smoother with reduced noise, but fine texture details are limited due to pixel-wise optimization.

### 🔹 GAN (SRGAN) Results

The GAN-based model produces visually sharper and more realistic high-resolution images. By learning perceptual features through adversarial training, SRGAN enhances texture details and edges more effectively than the CNN model.

### 🔹 Visual Comparison

The comparison below shows the transformation from **Low Resolution (22×22)** to **Super-Resolved (88×88)** images using both models. SRGAN demonstrates superior perceptual quality, while SRCNN provides stable and consistent reconstruction.




