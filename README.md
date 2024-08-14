# PneumoNet: Pneumonia Detection from Chest X-Rays

PneumoNet is a deep learning project aimed at detecting pneumonia in chest X-ray images using Convolutional Neural Networks (CNNs) built with PyTorch. This project covers the entire workflow, from data preprocessing and model training to evaluation and deployment as a web application.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Dataset](#dataset)
- [Usage](#usage)
  - [Data Preprocessing](#data-preprocessing)
  - [Model Training](#model-training)
  - [Model Evaluation](#model-evaluation)
  - [Model Deployment](#model-deployment)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Pneumonia is a serious respiratory infection, and early detection is crucial for effective treatment. This project leverages deep learning techniques to build a model that can classify chest X-ray images as either pneumonia-positive or pneumonia-negative. 

## Project Structure

```
PneumoNet/
├── data/
│   ├── raw/
│   ├── processed/
│   └── README.md
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_model_training.ipynb
│   ├── 03_model_evaluation.ipynb
│   └── 04_deployment.ipynb
├── src/
│   ├── __init__.py
│   ├── data_preprocessing.py
│   ├── model.py
│   ├── train.py
│   ├── evaluate.py
│   └── utils.py
├── app/
│   ├── app.py
│   ├── requirements.txt
│   └── README.md
├── tests/
│   ├── test_data_preprocessing.py
│   ├── test_model.py
│   └── test_train.py
├── .gitignore
├── README.md
├── requirements.txt
├── LICENSE
└── setup.py
```

## Installation

To get started with PneumoNet, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/azizharouna/PneumoNet.git
   cd PneumoNet
   ```

2. **Install dependencies:**
   Create a virtual environment and install the required packages:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```

3. **Download the dataset:**
   Follow the instructions in the `data/README.md` to download and prepare the dataset.

## Dataset

The dataset used in this project is the [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia) dataset from Kaggle. It contains labeled X-ray images of patients with and without pneumonia.

### Dataset Structure:

```
data/
├── raw/                # Original dataset files
├── processed/          # Preprocessed data (train, validation, and test sets)
└── README.md           # Instructions on data acquisition and processing
```

## Usage

### Data Preprocessing

1. **Preprocess the data:**
   Run the `01_data_preprocessing.ipynb` notebook to load, explore, and preprocess the dataset, including data augmentation techniques.

2. **Split the data:**
   The notebook splits the data into training, validation, and test sets, and stores the processed data in the `data/processed/` directory.

### Model Training

1. **Train the model:**
   Open and run the `02_model_training.ipynb` notebook to design the CNN architecture, set up the training loop, and train the model on the preprocessed dataset.

2. **Save the model:**
   The trained model will be saved in the `models/` directory for later evaluation and deployment.

### Model Evaluation

1. **Evaluate the model:**
   Use the `03_model_evaluation.ipynb` notebook to evaluate the model's performance on the test set using metrics such as accuracy, precision, recall, and F1-score.

### Model Deployment

1. **Deploy the model:**


## Results

The model's performance, including accuracy, precision, recall, and F1-score, is documented in the `03_model_evaluation.ipynb` notebook. Example predictions and visualizations are also provided.

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository, create a new branch, and submit a pull request. For major changes, please open an issue to discuss your ideas.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
