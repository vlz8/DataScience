# DataScience

A collection of end-to-end data science projects covering classification, regression, computer vision, and natural language processing. Each project includes exploratory data analysis, data preprocessing, model training, and evaluation.

## Projects

| # | Project | Problem Type | Key Model | Accuracy | Tech Stack | Description |
|---|---------|-------------|-----------|----------|------------|-------------|
| 01 | [Titanic Survival Prediction](./01.%20Titanic%20Survival%20Prediction/) | Binary Classification | Logistic Regression | **83.8%** | Pandas, scikit-learn, Seaborn | Classic Kaggle dataset. Full pipeline: EDA with survival patterns by sex, class, age, and family size. Feature engineering (Title, FamilySize, HasCabin). 7 classifiers compared with cross-validation and GridSearchCV tuning. |
| 02 | [Iris Flower Classification](./02.%20Iris%20Flower%20Classification/) | Multi-class Classification | CNN (Keras/TF) | ~50% (5 classes) | TensorFlow, OpenCV, Keras | Image classification of 5 flower types (daisy, dandelion, rose, sunflower, tulip) using a CNN on 150x150 resized images. Includes training/validation curves and ROC analysis. |
| 03 | [Customer Churn](./03.%20Customer%20Churn/) | Binary Classification | Custom Logistic Regression | **88.9%** | Pandas, NumPy, scikit-learn | Predicts marketing agency customer churn. Implements logistic regression from scratch — custom sigmoid, cost function, and gradient descent. Applied to new customer data for real-world prediction. |
| 04 | [Heart Failure Prediction](./04.%20Heart%20Failure%20Prediction/) | Binary Classification | Logistic Regression | **84%** | Pandas, scikit-learn, Seaborn | Clinical data analysis for cardiovascular death prediction. Logistic Regression with confusion matrix and classification report evaluation on 12 clinical features. |
| 05 | [Rental Prices of AirBnb](./05.%20Rental%20Prices%20of%20AirBnb/) | Regression | Linear Regression | R² = 0.14 | Pandas, scikit-learn, Matplotlib | Regression model on 27,379 AirBnB listings. Covers outlier analysis, label encoding, and linear regression. Discusses why R² is low and what could improve it. |
| 06 | [Message Spam Filtering](./06.%20Message%20Spam%20Filtering/) | Text Classification | SVM / Naive Bayes | — | NLTK, scikit-learn, TF-IDF | NLP pipeline: text cleaning (stopword removal, stemming), TF-IDF vectorization, and classification with SVM (sigmoid kernel), Multinomial Naive Bayes, and Decision Tree. |
| 07 | [Cyber-Bullying Prediction](./07.%20Cyber-Bullying%20Prediction/) | Text Classification | SVC (sigmoid) | **95.1%** | NLTK, scikit-learn, TF-IDF | Detects bullying in Formspring Q&A posts. TF-IDF + multiple classifiers with GridSearchCV hyperparameter tuning. Addresses class imbalance challenges. |
| 08 | [Gender Classification](./08.%20Gender%20Classification/) | Image Classification | EfficientNetV2-S | **91%** | PyTorch, torchvision | Fine-tuned EfficientNetV2-S for binary gender classification from images. Data augmentation, early stopping, and evaluation with confusion matrix and per-class metrics. |
| 09 | [Face Detection](./09.%20Face%20Detection/) | Computer Vision | MTCNN / Haar Cascades | — | OpenCV, MTCNN, TensorFlow | Compares two face detection approaches: OpenCV Haar Cascades and MTCNN. Runs on 1,800 face images, visualizes bounding boxes, and compares detection accuracy. |

## Tech Stack

**Languages & Libraries**

- **Python** — core language across all projects
- **Pandas / NumPy** — data manipulation and numerical computing
- **Matplotlib / Seaborn** — visualization and EDA
- **scikit-learn** — classical ML models, preprocessing, evaluation metrics
- **TensorFlow / Keras** — deep learning (CNNs, EfficientNet)
- **PyTorch / torchvision** — transfer learning and image classification
- **OpenCV / MTCNN** — computer vision and face detection
- **NLTK** — natural language processing, tokenization, stemming

**Techniques Used**

- Supervised learning (classification & regression)
- Convolutional Neural Networks (CNNs)
- Transfer learning (EfficientNetV2-S)
- NLP preprocessing (TF-IDF, stemming, stopword removal)
- Hyperparameter tuning (GridSearchCV)
- Cross-validation
- Data augmentation
- Custom model implementations (logistic regression from scratch)

## Getting Started

Each project is self-contained with its own `requirements.txt`. To run any project:

```bash
cd " "
pip install -r requirements.txt
jupyter notebook
```
