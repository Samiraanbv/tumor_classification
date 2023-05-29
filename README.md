
# MRI Data Classification
# MRI Data Classification - Brain Tumor Detection
This project focuses on classifying MRI (Magnetic Resonance Imaging) data into different categories, specifically without tumor, and with tumor types such as glioma, meningioma, and pituitary. The dataset used for this classification task is obtained from Kaggle, available at https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri.

## Methodology
To solve this problem, transfer learning using EfficientNet is employed. The weights of the EfficientNet model are set to be trainable, allowing the model to adapt and learn from the MRI dataset. The implementation is done using the PyTorch framework, leveraging its powerful deep learning capabilities.

## Data Preprocessing
To ensure robustness and prevent overfitting, several transformations are applied to the training dataset. These transformations include:

- Resize: The images are resized to a specific dimension suitable for the EfficientNet model.
- Random Flip: Images are randomly flipped horizontally or vertically to introduce variation and aid in generalization.
- Gaussian Blur: A Gaussian blur is applied to the images, which can help reduce noise and improve overall image quality.
These transformations are carefully designed to be independent of the evaluation data to prevent any data leakage and maintain the integrity of the model's performance assessment.

## Model Training
The training process involves optimizing the model's weights using the Adam optimizer. The model is trained for 20 epochs with a learning rate of 0.0001. This configuration ensures an adequate number of iterations while controlling the step size for gradient updates during training.

## Evaluation Metrics
The performance of the classification model is evaluated using two key metrics:

Accuracy: The accuracy metric measures the proportion of correctly classified MRI images in the test dataset.
Loss: The loss metric represents the discrepancy between the predicted and true labels, aiming to minimize the error during training.
Results
After training the model using the described methodology, the achieved results are as follows:

Accuracy: Approximately 99.5% accuracy on the test dataset, indicating the model's ability to classify MRI images correctly.
Loss: Less than 0.02 loss, demonstrating a minimal discrepancy between the predicted and true labels.
These results highlight the effectiveness of transfer learning with EfficientNet and the success of the chosen configuration in accurately classifying MRI images into different tumor categories.

## Getting Started
To replicate and build upon this work, follow these steps:

Clone the repository: git clone https://github.com/your-username/repository-name.git
Download the MRI dataset from https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri and place it in the appropriate data directory.
Set up the required dependencies, including PyTorch and other necessary packages.
Modify the dataset path and other hyperparameters in the code, if necessary.
Run the training script and monitor the progress and performance of the model.
Evaluate the trained model using the test dataset and analyze the results.
Feel free to customize and experiment with the code to further enhance the classification performance or adapt it to other similar problems.

## Acknowledgments
We acknowledge the contribution of the Kaggle community and specifically the dataset provider, Masoud Nickparvar, for making the brain tumor MRI dataset publicly available. Their efforts enable the development of innovative solutions in medical image analysis and classification.


