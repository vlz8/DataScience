# Iris Flower Classification

Classifies images of flowers (daisy, dandelion, rose, sunflower, tulip) into five categories using a Convolutional Neural Network (CNN). The model is trained on resized 150x150 images and evaluated with accuracy, classification reports, and ROC curves.

## Dataset

A local `flowers/` directory containing labeled subdirectories for each flower type (daisy, dandelion, rose, sunflower, tulip) with a total of approximately 4,317 images.

## Results

The CNN achieves approximately 50% accuracy on the test set (5 flower classes). Training accuracy reaches ~83% by epoch 10, but validation accuracy plateaus around 50-54%, indicating overfitting. See notebook for classification reports and ROC curves.

## Tech Stack

- NumPy
- Pandas
- OpenCV (cv2)
- Matplotlib
- Seaborn
- scikit-learn
- Keras / TensorFlow
