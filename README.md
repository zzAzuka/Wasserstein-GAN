# Wasserstein Generative Adversarial Network (WGAN) for Synthetic Data Generation

## Overview

This project implements a Wasserstein Generative Adversarial Network (WGAN) to generate synthetic numerical data, addressing class imbalance in datasets.

## What are GANs?

Generative Adversarial Networks (GANs) are a class of machine learning frameworks designed for generating new data samples. They consist of two neural networks: a **generator** and a **discriminator** (or critic). The generator creates synthetic data samples, while the discriminator evaluates them against real data, providing feedback to improve the generator's performance. This adversarial training process continues until the generator produces samples that are indistinguishable from real data.

## Why Use Wasserstein Loss?

Wasserstein loss is employed in WGANs to improve training stability and convergence. Traditional GANs can suffer from issues like mode collapse, where the generator produces limited varieties of samples. Wasserstein loss measures the distance between the distributions of real and generated data more effectively than standard loss functions. It provides meaningful gradients even when the discriminator is not performing well, leading to more stable training dynamics and better-quality generated samples.

## Features

- Generates synthetic numerical data using WGAN architecture.
- Implements Wasserstein loss for improved training stability.
- Includes evaluation metrics like Precision and Recall to assess data quality.
