# Food Image Classification

## Project Overview
This end-to-end machine learning project focuses on classifying food images using deep learning techniques. The goal is to develop a robust model capable of accurately identifying different food items while also predicting their calorie counts.

---

## Steps & Techniques

### 1. Data Preparation:
- Loaded the dataset and performed an initial exploration.
- Visualized sample images for each class to understand the dataset distribution.
- Created training and testing datasets, then generated mini versions containing images from three classes to simplify fitting:
  - Mini training set: 7,850 images.
  - Mini test set: 2,535 images.

### 2. Data Augmentation & Normalization:
- Applied data augmentation techniques such as shear, zoom, and horizontal flip to enhance model generalization.
- Normalized images by scaling pixel values to the range [0, 1].

### 3. Model Building:
- Utilized ResNet50 as the base model with pre-trained weights.
- Added custom layers with L2 regularization to reduce overfitting and improve generalization.

### 4. Training:
- Trained the model with a batch size of 16.
- Applied early stopping to halt training when validation loss stopped improving.
- Implemented ModelCheckpoint and CSVLogger callbacks to save the best-performing model and log training history.

### 5. Evaluation:
- Assessed model performance on the test set using true labels.
- Predicted calorie counts for various food items and analyzed accuracy.

---

## Tools & Technologies Used
- **Programming Language**: Python  
- **Deep Learning Framework**: TensorFlow/Keras  
- **Libraries**: NumPy, Pandas, Matplotlib, Seaborn, OpenCV  
- **Model Architecture**: ResNet50

---

# Explore the dataset on Kaggle 🌐 [View Dataset ](https://www.kaggle.com/dansbecker/food-101)


