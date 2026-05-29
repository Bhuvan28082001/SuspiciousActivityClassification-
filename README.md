# Suspicious Activity Classification Using CNN and Transfer Learning

## Project Overview

This project develops a deep learning-based suspicious activity classification system capable of identifying violent and non-violent activities from surveillance images.

## Dataset

Real Life Violence Situations Dataset

https://www.kaggle.com/datasets/abdulmananraja/real-life-violence-situations

## Models Used

- Custom CNN
- ResNet50
- MobileNetV2

## Results

| Model | Validation Accuracy |
|---------|---------|
| Custom CNN | 73.49% |
| ResNet50 | 54.07% |
| MobileNetV2 | 88.03% |

## Final Performance

- Accuracy: 88.03%
- Precision: 0.88–0.89
- Recall: 0.87–0.89
- F1 Score: 0.88–0.89

## Output Files

- accuracy_loss_curve.png
- confusion_matrix.png
- mobilenet_violence_model.h5

## Technologies

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn

## Conclusion

MobileNetV2 achieved the highest validation accuracy (88.03%) and was selected as the final model for suspicious activity classification.
