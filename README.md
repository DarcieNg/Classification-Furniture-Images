

# 🛋️ Furniture Image Classification

![Project Banner](https://via.placeholder.com/1200x400?text=Furniture+Image+Classification+Project)

This repository contains the code and resources for **Furniture Image Classification**, a machine learning project that classifies furniture images into categories and recommends similar items based on user-uploaded images.

![GitHub repo size](https://img.shields.io/github/repo-size/your-username/furniture-image-classification)
![GitHub contributors](https://img.shields.io/github/contributors/your-username/furniture-image-classification)
![GitHub last commit](https://img.shields.io/github/last-commit/your-username/furniture-image-classification)
![License](https://img.shields.io/github/license/your-username/furniture-image-classification)

---

## 📜 Table of Contents

1. [Project Overview](#project-overview)
2. [Tasks](#project-tasks)
    - [Task 1: Category Classification](#task-1-furniture-category-classification)
    - [Task 2: Similar Furniture by Category](#task-2-finding-similar-furniture-by-category)
    - [Task 3: Similar Furniture by Category & Style](#task-3-finding-similar-furniture-by-category-and-style)
3. [Datasets](#datasets)
4. [Models Used](#models-used)
5. [How to Run the Project](#running-the-project)
6. [Results](#results)
7. [Contributors](#team-members)


---

## 🌟 Project Overview

The goal of this project is to build a **Furniture Recommendation System** that utilizes deep learning to classify furniture images and suggest similar items. Users upload furniture images, and the system provides category-based recommendations using advanced image processing techniques.

<p align="center">
    <img src="https://via.placeholder.com/600x300?text=Model+Architecture" alt="Model Architecture" />
</p>

## 🛠️ Project Tasks

### Task 1: Furniture Category Classification

Classify images into six furniture categories (e.g., tables, chairs). Models such as **CNN**, **ResNet50**, and **InceptionV3** were used, with **InceptionV3** chosen for its superior accuracy.

| Model       | Train Accuracy | Validation Accuracy |
|-------------|----------------|---------------------|
| CNN         | 71.52%         | 71.56%              |
| ResNet50    | 93.09%         | 90.52%              |
| **InceptionV3** | **97.46%**  | **96.63%**          |

![Task 1 Results](https://via.placeholder.com/800x400?text=Model+Performance+Graph)

### Task 2: Finding Similar Furniture by Category

This task focuses on identifying 10 similar images to a given input using **ResNet50** and the **NearestNeighbors** algorithm.

<p align="center">
    <img src="https://via.placeholder.com/600x300?text=Feature+Extraction+Process" alt="Feature Extraction" />
</p>

### Task 3: Finding Similar Furniture by Category and Style

Further refines the similarity search by incorporating both category and style information. **ResNet50** continues to be the main architecture used.

---

## 🗂️ Datasets

The dataset includes **90,000+ images** categorized into 6 types of furniture and 11 interior styles. Preprocessing involved duplicate removal and resizing to fit model inputs.

| Category  | Percentage |
|-----------|------------|
| Lamps     | 36%        |
| Chairs    | 25%        |
| Tables    | 20%        |

---

## 🧠 Models Used

1. **Convolutional Neural Networks (CNN)**: Used as a baseline for image classification.
2. **ResNet50**: Employed for both feature extraction and classification in all tasks.
3. **InceptionV3**: Provided the best accuracy for the image classification task.

<p align="center">
    <img src="https://via.placeholder.com/600x300?text=ResNet50+Model+Architecture" alt="ResNet50 Architecture" />
</p>

---

## 🚀 Running the Project

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

3. Train and evaluate the model:
   ```bash
   python train_model.py
   ```

4. Test the recommendation system:
   ```bash
   python recommend.py --input your_image.jpg
   ```

---

## 📊 Results

- **InceptionV3** achieved the highest accuracy of **96.63%** in Task 1.
- **NearestNeighbors** produced reliable results for similarity matching in Task 2.
  
<p align="center">
    <img src="https://via.placeholder.com/600x300?text=Example+Results+Screenshot" alt="Example Results" />
</p>

---

## 👥 Team Members

- **Shirin Shujaa** – S3983427
- **Nguyen Vu Thuy Duong** – S3865443
- **Huynh Quang Dong** – S3938006
- **Nguyen Bao Minh** – S3926080
- **Tran Viet Hoang** – S3928141

