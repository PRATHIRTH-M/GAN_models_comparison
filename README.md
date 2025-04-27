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


Models Overview

Model | Discriminator  | Generator | Key Difference
LSGAN | MSE Loss-based | MLP | Least Squares loss instead of BCE
WGAN | Critic (No Sigmoid) | MLP | Wasserstein loss with weight clipping
WGAN-GP | Critic | MLP | Wasserstein loss with Gradient Penalty

