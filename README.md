# Brain Tumor Prediction Model with CNN

This project utilizes Convolutional Neural Networks (CNNs) to predict and classify brain tumor types from MRI scan images. The model is trained to classify the following tumor types:

- Meningioma
- Glioma
- Pituitary Tumor
- No Tumor

## Dataset

The model is trained on a dataset consisting of MRI scan images of the brain, containing examples of each tumor type as well as images with no tumors. The dataset may suffer from class imbalance, which was addressed using downsampling techniques to ensure balanced representation during training.

## Model Architecture

The CNN architecture comprises multiple convolutional layers followed by batch normalization, dropout, and L2 regularization layers to prevent overfitting. The architecture is designed to extract features from the input MRI images and learn discriminative patterns for tumor classification.

## Techniques Used

- **Downsampling**: Addressing class imbalance by downsampling the majority classes to achieve a balanced dataset.
- **Batch Normalization**: Normalizing the input to each layer to stabilize and accelerate the training process.
- **Dropout**: Introducing dropout layers to randomly deactivate neurons during training to prevent overfitting.
- **L2 Regularization**: Applying L2 regularization to the model's weights to penalize large parameter values and reduce overfitting.
- **Early Stopping**: Employing EarlyStopping technique to monitor validation accuracy during training and halt training if the validation accuracy does not improve for a specified number of epochs (patience).

## Usage

1. **Training**: Use the provided dataset to train the model by running the training script.
2. **Evaluation**: Evaluate the model's performance on test data using the provided evaluation script.
3. **Prediction**: Utilize the trained model to make predictions on new MRI scan images for tumor classification.

## Dependencies

Ensure you have the following dependencies installed to run the code:
- TensorFlow
- NumPy
- Scikit-learn
- Matplotlib

## References

If you use this code for your research or project, please consider citing the relevant papers and datasets.

