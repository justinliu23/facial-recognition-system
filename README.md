# facial-recognition-system
 

# Face Recognition Project

## Table of Contents
- [Notebook Recap](#notebook-recap)
- [Installation Instructions](#installation-instructions)
  - [Dependencies](#dependencies)
  - [Setup](#setup)
- [Usage](#usage)
  - [Running the Project](#running-the-project)
  - [Example Usage](#example-usage)
- [Configuration](#configuration)

## Notebook Recap

- Posed face recognition as a binary classification problem.
- Implemented one-shot learning for a face recognition problem.
- Applied the triplet loss function to learn a network's parameters in the context of face recognition.
- Mapped face images into 128-dimensional encodings using a pretrained model.
- Performed face verification and face recognition with these encodings.

## Installation Instructions

### Dependencies
This project requires the following Python libraries and packages:
- `tensorflow`
- `numpy`
- `pandas`
- `PIL`
- `keras`

You can install these dependencies using pip:
```sh
pip install tensorflow numpy pandas pillow keras
```

### Setup
1. Clone the repository to your local machine:
    ```sh
    git clone https://github.com/justinliu23/facial-recognition-system.git
    ```
2. Navigate to the project directory:
    ```sh
    cd face_recognition
    ```
3. Ensure all dependencies are installed

## Usage

### Running the Project
1. Launch Jupyter Notebook:
    ```sh
    jupyter notebook
    ```
2. Open the notebook `Face_Recognition.ipynb`.
3. Execute the cells in the notebook sequentially to run the face recognition pipeline.

### Example Usage
Here is a brief guide on how to use the project:

#### Naive Face Verification
In this section, you will compare two images pixel-by-pixel to determine if they are of the same person.

#### Encoding Face Images into a 128-Dimensional Vector
Using a Convolutional Neural Network (ConvNet), you will compute encodings for face images.

#### Using the Triplet Loss
The Triplet Loss function helps learn parameters that improve the accuracy of the model in distinguishing between different faces.

#### Loading the Pre-trained Model
You will load a pre-trained model to compute the 128-dimensional encodings for the face images.

#### Applying the Model
- **Face Verification**: Determine if two images are of the same person (1:1 matching).
- **Face Recognition**: Identify the person in an image from a set of K persons (1:K matching).

## Configuration
### Model Configuration
- **Input Shape**: The input images are expected to have the shape (96, 96, 3).
- **ConvNet Architecture**: The model architecture includes convolutional layers, batch normalization, pooling layers, and dense layers.
- **Loss Function**: Triplet loss function is used to train the model.

### Data Configuration
- **Data Format**: The images should be in a format that can be processed by PIL (e.g., JPG, PNG).
- **Dataset Structure**: Organize your dataset such that each person has their own folder containing images of their face.
