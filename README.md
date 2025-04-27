# GAN_models_comparison
This project presents a comprehensive comparison of three popular Generative Adversarial Network (GAN) architectures — LSGAN, WGAN, and WGAN-GP — using the ChestMNIST dataset from MedMNIST for medical image generation.

The aim is to explore how different loss functions and training strategies affect the quality, stability, and realism of generated images.

We train and evaluate each model under identical settings, visualize results through TensorBoard, and report quantitative metrics including:

Inception Score (IS)

Fréchet Inception Distance (FID)

This project provides clear insights into how different GAN variants perform on biomedical data, making it ideal for academic studies, benchmarking, or practical GAN experimentation.

✨ Features
Fully implemented LSGAN, WGAN, and WGAN-GP from scratch using PyTorch
TensorBoard integration for real-time visualization of images and metrics
Quantitative evaluation using Inception Score (IS) and Frechet Inception Distance (FID)
Lightweight implementation optimized for the ChestMNIST dataset
Clean and modular code structure

Dataset
Dataset: ChestMNIST (subset of MedMNIST v2)

Type: Multi-label chest X-ray images

Image Size: 28×28 pixels with 3 color channels (RGB)

Purpose: Benchmark for low-resolution biomedical image generation

Setup
Framework:

PyTorch (Deep Learning Framework)

Environment:

Python 3.8+

TorchMetrics (for IS and FID evaluation)

TensorBoard (for visualization)Training Details
Epochs: 50 per model

Batch Size: 64

Optimizers: Adam for both Generator and Discriminator

Loss Functions:

LS-GAN: Least Squares Loss

WGAN: Wasserstein Loss with Weight Clipping

WGAN-GP: Wasserstein Loss with Gradient Penalty

Evaluation Metrics
Inception Score (IS): Higher is better, measures image quality and diversity.

Fréchet Inception Distance (FID): Lower is better, measures similarity to real images.

 Visual Insights
Training curves (Generator and Discriminator losses) and sample generations were logged using TensorBoard for better monitoring and analysis.

Observations:

LS-GAN: Showed fluctuating loss patterns over epochs.

WGAN: Displayed steady convergence but some variance in generator loss.

WGAN-GP: Achieved smooth, stable convergence throughout training.



