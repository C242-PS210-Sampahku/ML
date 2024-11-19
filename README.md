# Sampahku Model - Machine Learning

## Overview
This project aims to classify various types of garbage into different categories using a convolutional neural network (CNN) model. The categories include batteries, biological waste, cardboard, clothes, glass, metal, paper, plastic, shoes, and general trash.

## Model Performance
The model was trained and evaluated on a dataset consisting of diverse garbage images. Below are the key performance metrics for the current model configuration:

- **Training Accuracy**: 88.00%
- **Training Loss**: 0.3811
- **Validation Accuracy**: 92.78%
- **Validation Loss**: 0.2488
- **Learning Rate**: 1.0000e-05
- **Test Accuracy**: 92.84%
- **Test Loss**: 0.2165

## Why This Model Configuration is Optimal
We have tested various configurations, including models with higher accuracy on the training data. However, those models exhibited signs of overfitting, where the model performs well on the training data but poorly on unseen data. Overfitting reduces the model's generalizability and makes it less reliable for real-world applications.

### Key Points:
- **Balanced Performance**: The current model strikes a balance between training accuracy and validation accuracy, ensuring it generalizes well to new data.
- **Reduced Overfitting**: By avoiding excessively high accuracy on training data, the model remains robust and reliable when predicting on unseen data.
- **Stable Learning Rate**: A learning rate of 1.0000e-05 has been found to provide a stable training process without rapid fluctuations in loss values.

## Conclusion
The current model configuration, with its balance of accuracy and loss metrics, is well-suited for practical use in classifying garbage images. It avoids the pitfalls of overfitting, ensuring that the model remains reliable and effective across diverse datasets.

For further improvements, we suggest continuing to explore data augmentation techniques and regularization methods. However, the present model provides a solid foundation for accurate and consistent garbage classification.

## How to Use
To use this model for your own predictions, follow these steps:
1. Load the pre-trained model (`model.h5`).
2. Preprocess your images to match the input requirements of the model (224x224 pixels, normalized).
3. Use the model's `predict` method to classify new images.

For more detailed instructions, please refer to the code and comments provided in the repository.

## Author
Developed by [Your Name]

For any questions or contributions, feel free to reach out!

