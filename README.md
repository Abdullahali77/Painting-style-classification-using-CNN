# **Painting-style-classification-using-CNN**
This project focuses on classifying paintings into different styles using Convolutional Neural Networks (CNNs). The dataset used in this project is the keremberke/painting-style-classification dataset from Hugging Face, which contains various painting styles as classes.

## Data Preprocessing
The dataset is already split into training, validation, and testing sets.
The preprocessing pipeline involves resizing images to 224x224 pixels, normalizing pixel values to the range [0, 1], and converting the images and labels to tensors. This preprocessing is applied to the training, validation, and test datasets.

## Model Architectures
Several CNN architectures were tested to find the best-performing model for painting style classification. All models are implemented using TensorFlow and Keras.

### First Architecture
Layers: 3 Convolutional layers, 2 MaxPooling layers, 2 Dropout layers, and 1 Fully connected layer.
Optimizer: Adam with a learning rate of 1e-4.
Loss Function: Sparse Categorical Crossentropy with logits.
Metrics: Accuracy.
### Second Architecture
Simplified version of the first architecture with fewer layers and lower dropout rates.
### Third Architecture
Adds an extra convolutional layer and increases dropout in certain layers.
### Fourth Architecture
Similar to the third but with adjusted dropout rates.

## Results
Each architecture was trained for 17 epochs, with validation accuracy and loss monitored throughout the training process. The models were evaluated on the test set, and the learning curves were plotted to visualize training performance. The best architecture(highest accuracy) was the first one.

## Predicting a New Image
To predict the style of a new painting, you can use the trained model to make predictions on a single image after preprocessing it with the same transformations.


