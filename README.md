MixUp vs. CutMix: Regularization Study on CIFAR-10
Overview

This project compares MixUp and CutMix, two data-augmentation and regularization strategies for image classification. Using a ResNet-18 classifier trained on CIFAR-10, the study evaluates how each method affects validation accuracy, loss behavior, and training stability under a controlled optimization setup.

The training framework uses AdamW optimization, warm-up followed by cosine learning-rate scheduling, mixed-precision training, reproducibility controls, checkpointing, and epoch-level metric logging. MixUp blends full images and labels, while CutMix replaces localized image regions and adjusts labels by the replaced area.

Project Goals:
Implements baseline, MixUp, and CutMix training configurations for controlled comparison.
Uses ResNet-18, AdamW, mixed-precision training, and warm-up/cosine learning-rate scheduling.
Logs training loss, validation loss, and validation accuracy across epochs.
Achieved peak recorded validation accuracies of 94.47% with MixUp and 94.67% with CutMix.

Tools used
Python, PyTorch, torchvision, ResNet-18, AdamW, mixed-precision training, CIFAR-10
