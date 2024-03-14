# Optical-Character-Recognition

## Overview
This project advances Optical Character Recognition (OCR) technology by extracting textual content from images through state-of-the-art machine learning and computer vision techniques. The goal is to accurately convert written text into a machine-readable format, facilitating a wide range of applications from document digitization to automated data entry.

The OCR process encompasses several crucial steps, including image preprocessing to enhance text readability, feature extraction to identify distinctive attributes, and text recognition where the actual conversion takes place.

In this project, we explore three core machine learning models, each offering unique strengths to the OCR task:

- **Random Forest**: An ensemble learning method for classification that operates by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) of the individual trees. Renowned for its accuracy and ability to run efficiently on large datasets.

- **K-Nearest Neighbors (KNN)**: A simple, intuitive model that classifies texts by a majority vote of its neighbors, with the object being assigned to the class most common among its k nearest neighbors. KNN is especially useful for its ease of implementation and strong performance on a variety of datasets.

- **Support Vector Machine (SVM)**: A powerful, versatile machine learning model capable of performing linear or nonlinear classification, regression, and even outlier detection. It is particularly suited for complex text recognition tasks with high-dimensional data.

- **Gaussian Mixture Model (GMM)**: A probabilistic model that assumes all the data points are generated from a mixture of a finite number of Gaussian distributions with unknown parameters. GMM is especially adept at handling cases where the data involves multiple subpopulations, each of which can be modeled by a Gaussian distribution. This model is beneficial for OCR when dealing with varied text styles and densities, as it can adaptively segment different text features based on their statistical properties.


The dataset fueling our models' training and evaluation is the Standard OCR Dataset, which can be found on Kaggle: [Standard OCR Dataset](https://www.kaggle.com/datasets/preatcher/standard-ocr-dataset). This dataset provides a robust foundation for developing and testing OCR technologies.

## Preprocessing
The preprocessing stage is critical in the OCR pipeline, ensuring that the input images are optimized for text recognition. This process typically includes the following steps:

- **Image Loading**: Images are loaded into the system for processing. This is the first step in preparing the data for analysis.

- **Grayscale Conversion**: Color images are converted to grayscale to reduce complexity, focusing on the intensity of pixels rather than color information, which is essential for the subsequent steps.

- **Noise Reduction**: Various techniques, such as Gaussian blur or median filtering, are applied to reduce image noise. This step is crucial for improving the accuracy of the text detection process.

- **Thresholding**: To further simplify the image and highlight the text, thresholding techniques are used to create a binary image where the text is separated from the background.

- **Feature Extraction**: Before feeding the images into the machine learning models, relevant features are extracted. This can include edges, contours, or specific patterns that are characteristic of the text to be recognized.

These preprocessing steps are designed to enhance the quality and clarity of the text in the images, significantly improving the performance of the OCR models.

## Installation
To set up the project environment, follow these steps:
1. Clone the project repository to your local machine.
   
        git clone https://github.com/premkjain/Optical-Character-Recognition.git
        
2. Open a terminal and navigate to the project directory.
3. Ensure Python is installed on your system. If not, download and install it from [python.org](https://www.python.org/downloads/).
4. Install the required Python dependencies.

## Usage
Execute the `main.ipynb` notebook to walk through the OCR process. This notebook guides you through exploratory data analysis, model training, evaluation, and making predictions. It serves as the entry point for understanding and interacting with the OCR system.

## Models
Within the `Models` directory, you will find notebooks detailing the implementation and usage of specific OCR models, including Random Forest, KNN, SVM and GMM. These documents offer insights into model selection, training, and performance evaluation.

## Basic EDA
The `Basic_EDA.ipynb` notebook performs an exploratory analysis of the OCR dataset. It illustrates the dataset's structure, visualizes sample images, and outlines initial preprocessing steps, providing a foundational understanding of the data handling process.

## Documentation
For a detailed overview of the project, including its objectives, methodologies, and key findings, refer to the `Brief_Documentation.pdf`. This document is essential for gaining an in-depth understanding of the project's implementation and outcomes.

## Presentation
The project's findings and insights are further disseminated through presentations stored in the `Presentation` folder. These materials are useful for sharing the project's success and methodologies with a broader audience.

## License
This project is licensed under the MIT License - see the `LICENSE` file for details.
