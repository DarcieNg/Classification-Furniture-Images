
# Furniture Image Classification

This repository contains the code and resources for **Furniture Image Classification**, a machine learning project that aims to classify images of furniture into various categories and recommend similar items based on user-uploaded images.

## Project Overview

The main goal of this project is to build a **Furniture Recommendation System** that classifies images into furniture categories and suggests similar items. The system uses **deep learning** techniques, including **Convolutional Neural Networks (CNNs)** and **ResNet50**, to accurately categorize and recommend furniture styles and types.

## Team Members

- Shirin Shujaa - S3983427
- Nguyen Vu Thuy Duong - S3865443
- Huynh Quang Dong - S3938006
- Nguyen Bao Minh - S3926080
- Tran Viet Hoang - S3928141

## Project Tasks

### Task 1: Furniture Category Classification
This task involves classifying images into six furniture categories (e.g., tables, chairs, etc.) using models like **CNN**, **ResNet50**, and **InceptionV3**. After model evaluation, **InceptionV3** was selected as the final model due to its superior accuracy.

### Task 2: Finding Similar Furniture by Category
Using the **ResNet50** model for feature extraction, this task identifies 10 similar images to an input based on category. The **NearestNeighbors** algorithm achieved the best performance in this task.

### Task 3: Finding Similar Furniture by Category and Style
Building upon the category classification from Task 1, this task further refines the recommendation to find similar images by both category and style using **ResNet50** and separate models for each furniture category.

## Datasets

The dataset used consists of over **90,000 images** divided into 6 categories and 11 interior styles. The data underwent extensive preprocessing, including duplicate removal and resizing to support model inputs.

### Data Preprocessing
- **Duplicate Removal**: Eliminated duplicate images to maintain dataset integrity.
- **Resizing**: Adjusted image sizes to fit the model requirements.
- **Imbalance Handling**: Applied oversampling techniques to manage class imbalances.

Filtered datasets are stored in:
- `categorial_filter_df.csv`
- `style_filter_df.csv`

## Models Used

1. **Convolutional Neural Networks (CNN)**: Used as a baseline model with 6 layers, including convolutional and max pooling layers.
2. **ResNet50**: A 50-layer CNN used for tasks involving feature extraction and similarity matching.
3. **InceptionV3**: The selected model for Task 1 due to its high accuracy and ability to handle large datasets.

## Key Libraries and Tools

- **TensorFlow / Keras**: Used for model implementation.
- **scikit-learn**: Used for applying feature extraction and nearest neighbor algorithms.
- **Pillow & os**: For image processing and duplicate removal.

## Running the Project

To run the project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/furniture-image-classification.git
   cd furniture-image-classification
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the model training and evaluation scripts:
   ```bash
   python train_model.py
   ```

4. To test the recommendation system, use the `recommend.py` script:
   ```bash
   python recommend.py --input your_image.jpg
   ```

## Results

- **InceptionV3** achieved the highest validation accuracy of **96.63%** for Task 1.
- The **NearestNeighbors** algorithm produced the most reliable similarity results in Task 2.


