# Canine Affective State Classification: A Deep Learning Approach

## Overview
This repository contains the code and deep learning models aimed at classifying the emotive states of dogs based on their facial expressions captured in video frames. The project utilizes state-of-the-art convolutional neural networks (ResNet34, ResNet50) and a Vision Transformer (DINOv2) to analyze and predict the emotive states as either positive (anticipation of a reward) or negative (frustration).

### Objectives
- To evaluate the capability of deep learning models to interpret non-human animal emotions.
- To contribute to the improvement of interspecies communication and enhance understanding of animal emotions.

### Performance
| Model   | Validation Accuracy | Test Accuracy | Learning Rate | Weight Decay |
|---------|----------|----------|----------|----------|
| `ResNet-50` |**98%**| **91%**|0.01 | 0.0001 |
| `ResNet-34` | 82% | 88.9% |0.01 | 0.0001 |
| `DINOv2-ViT` | 89% | 82.2% |0.01 | 0.0001 |


### Setup
Clone this repository to your local machine:
```bash
git clone https://github.com/samuelcampione/canine_affective_state_classification.git
cd canine_affective_state_classification
```
