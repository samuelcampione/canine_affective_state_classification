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


### Setup and Usage
Clone this repository to your local machine:
```bash
git clone https://github.com/samuelcampione/canine_affective_state_classification.git
cd canine_affective_state_classification
```

- [prep_data.ipynb](https://github.com/samuelcampione/canine_affective_state_classification/blob/main/prep_data.ipynb): initial EDA, data storage setup, standard data resizing
- [data.py](https://github.com/samuelcampione/canine_affective_state_classification/blob/main/data.py):  image preprocessing functions and custom PyTorch Dataset class
- [models.py](https://github.com/samuelcampione/canine_affective_state_classification/blob/main/models.py): PyTorch models,  `ResNet` and `DINOv2`
- [train_eval.py](https://github.com/samuelcampione/canine_affective_state_classification/blob/main/train_eval.py): grid search, training, evalution functions
- [experiments.ipynb](https://github.com/samuelcampione/canine_affective_state_classification/blob/main/experiments.ipynb): explores and prepares data, performs hyperparameter experiments, and trains and evaluates models
- [visualizations.ipynb](https://github.com/samuelcampione/canine_affective_state_classification/blob/main/visualizations.ipynb): visualizes model performance

