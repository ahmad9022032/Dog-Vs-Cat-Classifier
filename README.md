# Cat vs Dog Classifier

This repository contains code for a convolutional neural network (CNN) classifier designed to distinguish between images of cats and dogs. The classifier is built using TensorFlow and Keras, two popular deep learning libraries.

## Description

The classifier is trained on a dataset containing images of cats and dogs. It utilizes convolutional neural network architecture, which is well-suited for image classification tasks due to its ability to capture spatial hierarchies in images.

### Data Preprocessing
Before training, the image data is preprocessed using the `ImageDataGenerator` class from Keras. This includes rescaling the pixel values to a range of [0, 1], applying data augmentation techniques such as shear range, zoom range, and horizontal flip to increase the variability of the training data.

### Model Training
The training data is fed into the CNN model in batches using the `flow_from_directory` method. The model is trained using the binary cross-entropy loss function and the Adam optimizer.

### Prediction
After training, the model can be used to predict whether an input image contains a cat or a dog. The `prediction.py` script provides an example of how to load an image, preprocess it, and obtain a prediction from the trained model.

### Evaluation
The performance of the model is evaluated using metrics such as accuracy and loss on both the training and validation sets. These metrics provide insights into how well the model is performing and help identify potential areas for improvement.

## Usage

1. **Data Preparation**: Organize the training and testing data into separate directories according to the specified structure.
2. **Dependencies Installation**: Install the required dependencies listed in the `Requirements_Libraries.txt` file using `pip install -r requirements.txt`.
3. **Training**: Run the code snippet provided in `catvsDog_classifier.py` to train the model.
4. **Prediction**: Use the provided code snippets to predict images using the trained model (`prediction.py`).
5. **Visualization**: Visualize predictions and evaluate model performance using the code provided in `visualization.py`.

## Results

The model achieved the following performance on the training and validation sets:

- Training Accuracy: 99.96%
- Training Loss: 0.002454
- Validation Accuracy: 97.56%
- Validation Loss: 0.102678

These results indicate that the model has learned to effectively distinguish between images of cats and dogs.

 In case you need any assistance or suggestions for further improvement, feel free to reach out to me via the contact details provided in the profile. 
