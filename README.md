# Tumor_MRI_Data_Classification
# MRI Data Classification - Brain Tumor Detection

This repository contains code and resources for classifying MRI (Magnetic Resonance Imaging) data for brain tumor detection. The goal of the project is to accurately classify MRI images into two classes: images with tumors and images without tumors. The tumor types considered in this classification are glioma, meningioma, and pituitary tumors.

## Dataset

The dataset used in this project is sourced from Kaggle and can be found at [Kaggle Brain Tumor MRI Dataset](https://www.kaggle.com/masoudnickparvar/brain-tumor-mri). The dataset contains MRI images of the brain, both with and without tumors, along with corresponding labels indicating the presence and type of tumor in each image.

Please download the dataset from the provided Kaggle link and place it in the appropriate location within the project directory structure.

## Project Structure

The repository is organized as follows:

```
.
├── data
│   ├── train
│   │   ├── glioma
│   │   ├── meningioma
│   │   └── pituitary
│   └── test
├── models
│   ├── efficientnet.py
│   └── utils.py
├── utils
│   ├── data_preprocessing.py
│   └── evaluation.py
├── README.md
└── main.py
```

- The `data` directory contains the training and testing data for the classification task. The training data is further divided into subdirectories based on the tumor types: `glioma`, `meningioma`, and `pituitary`. The `test` directory contains the MRI images for testing.

- The `models` directory contains the implementation of EfficientNet architecture in `efficientnet.py` and utility functions in `utils.py`.

- The `utils` directory provides utility scripts such as `data_preprocessing.py` for preprocessing the data and `evaluation.py` for evaluating the performance of the trained models.

- The `README.md` file (this file) provides an overview of the project, dataset information, and instructions for usage.

- The `main.py` file serves as the entry point for running the classification pipeline. You can modify this file to experiment with different hyperparameters or configurations.

## Getting Started

To get started with this project, please follow these steps:

1. Clone this repository to your local machine using the following command:
   ```
   git clone <repository_url>
   ```

2. Download the dataset from the [Kaggle Brain Tumor MRI Dataset](https://www.kaggle.com/masoudnickparvar/brain-tumor-mri) and place it in the `data` directory.

3. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

4. Modify and run the `main.py` script to train and evaluate the EfficientNet model on the brain tumor classification task. Adjust the hyperparameters as needed and experiment with different configurations.

## Results

The trained EfficientNet model achieves remarkable accuracy of more than 99% and a low loss of less than 0.02 on the brain tumor classification task.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

We would like to acknowledge the original authors of the [Kaggle Brain Tumor MRI Dataset](https://www.kaggle.com/masoudnickparvar/brain-tumor-mri) for providing the dataset.
