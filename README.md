# CycleGAN for Image Translation

## Project Overview
This project implements **CycleGAN** using **PyTorch** to translate images of apples to oranges and vice versa. The goal is to learn an unsupervised mapping between two domains without paired examples.
---
## Dataset
We use an unpaired dataset of **apples and oranges** to train CycleGAN. The dataset consists of images from both domains without explicit one-to-one correspondences.
---

## Implementation
The model consists of:
- **Generators** (ResNet-based architecture) to learn domain translation.
- **Discriminators** to classify real vs. fake images.
- **Cycle Consistency Loss** to ensure images maintain their structure during translation.

## Key Features
- **Residual Blocks**: Improve feature retention and transformation.
- **Instance Normalization**: Helps stabilize training.
- **Reflection Padding**: Reduces edge artifacts.
---

## Future Improvements
1. **Histogram Matching**: Aligns the color histograms of domain X (Apples) closer to the target domain Y (Oranges) to reduce color artifacts.
2. **Cosine Annealing for Learning Rate Scheduling**: Helps stabilize training and improve convergence.


