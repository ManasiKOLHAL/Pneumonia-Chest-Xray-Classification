# Pneumonia Detection from Chest X-ray Images Using Deep Learning

**Project ID:** PRAICP-1012  
**Team ID:** PTID-AIE-MAR-26-11144 – AIE  
**Author:** Manasi Kolhal

## Project Overview

This project explores deep learning techniques for classifying chest X-ray images into two categories: **Normal** and **Pneumonia**.

Four architectures were developed and compared: Custom CNN, ResNet50, MobileNetV2, and VGG16.

This is an educational machine learning project and is not intended for clinical diagnosis.

## Objectives

- Develop a binary chest X-ray image classification system.
- Apply image preprocessing and augmentation.
- Experiment with CNN and transfer learning architectures.
- Compare model validation performance.
- Understand class-wise model evaluation.

## Technologies Used

- Python
- TensorFlow and Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Dataset

The project uses a chest X-ray dataset containing:

| Dataset | Images |
|---|---:|
| Training | 5,216 |
| Original validation | 16 |
| Testing | 624 |
| **Total** | **5,856** |

The training folder was divided into training and validation subsets using an 80:20 split.

### Classes
- NORMAL
- PNEUMONIA

## Project Workflow

1. Dataset loading and exploration.
2. Image resizing to 224 × 224 pixels.
3. Pixel normalization.
4. Data augmentation.
5. Model development and training.
6. Validation and performance comparison.
7. Sample image prediction.

## Models Implemented

- Custom Convolutional Neural Network (CNN)
- ResNet50
- MobileNetV2
- VGG16

**Training configuration:** Image size 224 × 224, batch size 32, and 3 epochs per model.

## Validation Results

| Model | Best Validation Accuracy |
|---|---:|
| Custom CNN | 87.06% |
| ResNet50 | 76.32% |
| MobileNetV2 | 94.44% |
| VGG16 | 92.43% |

These values represent the best validation accuracy recorded during training. They are not independent test-set results.

### ResNet50 Classification Report

- Accuracy: 72%
- Normal class recall: 6%
- Pneumonia class recall: 94%

The low recall for the Normal class indicates that class-wise performance requires further improvement.

## Limitations

- Models were trained for only three epochs.
- Class-wise performance is not balanced.
- Independent test-set evaluation remains necessary.
- Hyperparameter tuning and further experimentation are required.
- Predictions should not be used for medical decisions.

## Future Scope

- Apply class-balancing techniques.
- Perform hyperparameter optimization.
- Evaluate models on an independent test set.
- Explore additional transfer learning architectures.
- Improve recall for both classes.
- Investigate explainability techniques such as Grad-CAM.

## Conclusion

This project provided practical experience in chest X-ray image classification using deep learning. MobileNetV2 achieved the highest recorded validation accuracy among the four evaluated architectures. Further evaluation and improvement are necessary before drawing conclusions about model reliability.

**Disclaimer:** This project is developed for educational purposes only. It is not a medical diagnostic tool.
