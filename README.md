# LeNet Traffic Sign Classification

This project utilizes the LeNet architecture to classify traffic signs from a dataset of 32x32 pixel images.

## Dataset

The dataset comprises images of traffic signs, categorized into 43 distinct classes. Each class represents a different type of traffic sign, creating a multi-class classification challenge.

## Model Architecture

The model is built using the LeNet CNN architecture, featuring:

- **Convolutional Layers:** 2 layers with 5x5 kernels for feature extraction from the images.
- **Pooling Layers:** 2 average pooling layers to reduce dimensionality and emphasize important features.
- **Fully Connected Layers:** Layers that perform classification based on the features extracted by the convolutional and pooling layers.

## Training and Performance

The model was trained for 20 epochs, yielding the following performance metrics:

- **Training Loss:** 0.0765
- **Training Accuracy:** 98.26%
- **Validation Loss:** 0.5685
- **Validation Accuracy:** 87.21%

### Observations

- The model achieves high accuracy on the training set but experiences a significant drop in validation accuracy, suggesting potential overfitting.
- Potential improvements include:

  - **Extended Training:** Increasing the number of epochs to enhance learning and model performance.
  - **Image Augmentation:** Using techniques like rotation, scaling, and flipping to enrich the training dataset and improve generalization.
  - **Regularization:** Applying dropout or weight regularization to mitigate overfitting.
  - **Hyperparameter Tuning:** Fine-tuning learning rates, batch sizes, and other parameters for optimal performance.

## Conclusion

The LeNet model performs effectively in classifying traffic signs with strong training accuracy. To further improve validation performance, consider extending training, employing data augmentation, and exploring regularization and hyperparameter adjustments.
