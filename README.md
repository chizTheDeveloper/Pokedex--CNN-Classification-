# Pokedex (CNN Classification)
 Classification of Pokemon Types based of images trained with CNN
This project involves creating a convolutional neural network (CNN) using TensorFlow and Keras for image classification. Here's a summary of the key components and steps in the project:

# Accuracy Result:
Training Loss: 0.17190910317003727, Training Accuracy: 0.9486111998558044
Testing Loss: 0.24200911819934845, Testing Accuracy: 0.9111111164093018

# Import Libraries: 
Import necessary libraries, including TensorFlow, Keras, NumPy, and others.

# Define Data Directory: 
Specify the directory where your image data is located.

# ImageDataGenerator for Data Augmentation: 
Use the ImageDataGenerator from Keras for data augmentation, which includes rescaling, shearing, zooming, and horizontal flipping. This is useful for increasing the diversity of the training dataset.

# Create Training and Validation Datasets: 
Use the flow_from_directory method of the ImageDataGenerator to create training and validation datasets. This involves specifying parameters such as target size, batch size, class mode, and subset for training or validation.

# Visualize Images: 
Display a few images from the training dataset along with their corresponding class labels. This step is useful for understanding the data and ensuring it is loaded correctly.

# Define Model Architecture: 
Create a CNN model using the Sequential API from Keras. The model includes convolutional layers, max-pooling layers, a flattening layer, and dense layers. The output layer uses the softmax activation function for multi-class classification.

# Compile Model: 
Compile the model using the binary cross-entropy loss function, the Adam optimizer, and accuracy as the evaluation metric.

# Train the Model: 
Train the model using the fit method with the training dataset. The number of epochs and steps per epoch are specified.

# Evaluate Model: 
Evaluate the model on both the training and testing datasets using the evaluate method.

# Generate Predictions: 
Generate predictions for a random image from the training dataset and display the image along with the predicted class.

# Final Output:
Print the training and testing loss and accuracy, as well as the predicted class for a random image.

Overall, the project demonstrates the end-to-end process of building, training, and evaluating a CNN for image classification, with a specific focus on Pokemon types (Fire, Grass, Water). The model is capable of making predictions on new images based on the learned patterns from the training dataset.
