# CIFAR-10 Custom ResNet Model


**Team Members :**

> *   Sai Navyanth Penumaka : sp8138
> *   Karthik Sunkari : ks7929
> *   Geethika Rao Gouravelli : gg2879

## Overview
Custom ResNet model with Squeeze-and-Excitation (SE) blocks to classify images from the CIFAR-10 dataset.

# Summary

---

## Steps

### Data Preparation
- Loads CIFAR-10 training and test data, reshapes images, and combines batches.
- Normalizes pixel values and applies mean and standard deviation normalization.
- One-hot encodes labels for multi-class classification.
- Splits training data into training and validation sets.

---

### Model Design
- Builds an 80-layer ResNet model with SE blocks for enhanced feature extraction.
- Includes residual connections and SE optimization for improved accuracy.

---

### Training
- Augments training data with random transformations (rotation, flipping, zooming).
- Implements learning rate scheduling and uses callbacks like early stopping, model checkpointing, and learning rate reduction.
- Trains the model using augmented data for 400 epochs.

---

### Evaluation and Prediction
- Applies test-time augmentation (TTA) to improve predictions on test data.
- Generates predictions and creates a submission file with class labels.

---

### Visualization
- Plots training and validation accuracy/loss curves to monitor performance.

---

### Output
Validation Accuracy (10% of Dataset) : 94.10%

---

### Parameters

Total params: 4,628,210 (17.66 MB)

Trainable params: 4,617,010 (17.61 MB)

Non-trainable params: 11,200 (43.75 KB)


Total number of parameters: 4628210 (<5Million)
