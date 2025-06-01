A lightweight PyTorch CNN that recognizes individual playing cards from images in real time using OpenCV.

---

## Overview

This project trains a small convolutional network to classify playing cards (e.g., “Ace of Spades,” “3 of Hearts,” etc.) using images resized to 224×224. The included Jupyter notebook demonstrates:

- Data loading from a dataset directory where each subfolder represents a card class.
- A simple CNN architecture (Conv→ReLU→Pool→FC).
- Training loop with loss/accuracy visualization.
- Test evaluation showing accuracy metrics and confusion matrix.
- Real-time inference on a webcam feed using OpenCV.

---

## Model Summary

- **Conv1**: 3→32 channels, 5×5 kernel, ReLU, 2×2 MaxPool  
- **Conv2**: 32→64 channels, 5×5 kernel, ReLU, 2×2 MaxPool  
- **(Optional) Conv3**: 64→128 channels, 3×3 kernel, ReLU, 2×2 MaxPool  
- **FC1**: Flatten → 512 units, ReLU  
- **FC2**: 512 → num_classes  

The notebook code is easy to modify (add/drop layers, change channels).

---

## Results

- Typical test accuracy: ~97–99% on a standard 53‐card dataset.  
- Confusion matrix is available in the evaluation section showing most errors on visually similar cards.

---
