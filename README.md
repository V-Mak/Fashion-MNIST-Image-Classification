# Fashion-MNIST-Image-Classification

Fashion-MNIST is a popular dataset for image classification tasks. It serves as a more challenging alternative to the classic MNIST dataset. Fashion-MNIST consists of 60,000 training images and 10,000 testing images, with each image being a grayscale 28x28 pixel clothing item from one of 10 different categories. The goal is to train a machine learning model to correctly classify these images into their respective categories.

categories in the Fashion-MNIST dataset are:

* `Label`	`Description`
* `0`  `T-shirt/top`
* `1`  `Trouser`
* `2`	 `Pullover`
* `3`	 `Dress`
* `4`	 `Coat`
* `5`	 `Sandal`
* `6`	 `Shirt`
* `7`	 `Sneaker`
* `8`	 `Bag`
* `9`	 `Ankle boot`

`Dataset Selection`: You chose the Fashion-MNIST dataset, which is a collection of 28x28 grayscale images of clothing items from 10 different categories. This dataset is often used for benchmarking image classification models.

`Data Preprocessing`: You loaded the dataset and performed data preprocessing, which included:

`Normalizing the pixel values`: Scaling the pixel values to the range of 0 to 1 to make the training process more stable.
Splitting the dataset: Separating the dataset into training and testing sets. This helps you train the model on one portion and evaluate its performance on another.
Model Architecture: You designed a neural network model for image classification. The architecture included:

`A Flatten layer`: This layer converted the 28x28 images into a flat vector of 784 values.
Dense hidden layer: A densely connected layer with 128 neurons and ReLU activation function. This layer extracts features from the flattened input.
Dense output layer: A densely connected output layer with 10 neurons (one for each clothing category) and a softmax activation function. This layer provided the final classification probabilities.
Model Compilation: You compiled the model by specifying:

`The optimizer`: You used the Adam optimizer, which is an effective optimization algorithm for training neural networks.
The loss function: You chose 'sparse_categorical_crossentropy' as the loss function, which is suitable for multiclass classification tasks like Fashion-MNIST.
Evaluation metric: You selected 'accuracy' as the evaluation metric to monitor the model's performance during training.
