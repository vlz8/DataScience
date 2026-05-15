# Gender Classification

Classifies images of people as male or female using a fine-tuned EfficientNetV2-S model. Includes data augmentation, training with early stopping, and evaluation with a confusion matrix and classification report. Achieves approximately 91% accuracy on the validation set.

## Dataset

[Gender Detection and Classification Image Dataset](https://www.kaggle.com/datasets/trainingdatapro/gender-detection-and-classification-image-dataset) from Kaggle. Contains labeled JPG images split into `train/` and `test/` folders, each with `men/` and `women/` subfolders. The notebook includes a download command.

## Results

| Class | Precision | Recall | F1-Score |
|-------|-----------|--------|----------|
| Men | 0.96 | 0.89 | 0.93 |
| Women | 0.83 | 0.94 | 0.88 |
| **Overall Accuracy** | | | **91%** |

## Tech Stack

- PyTorch
- torchvision (EfficientNetV2-S, transforms v2)
- OpenCV
- Pillow
- pandas
- NumPy
- scikit-learn
- seaborn
- matplotlib

