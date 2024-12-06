# Perceptron Neural Network Application

This repository contains a neural network application implementing a multilayer perceptron for image recognition tasks, such as digit recognition using the MNIST dataset. The app allows you to train, predict, save, and load models easily.

## Features

- **Create Custom Models:** Define the number of neurons in hidden layers.
- **Train on Random Images:** Train the model on randomly selected images.
- **Make Predictions:** Predict the class label for an input image.
- **Save and Load Models:** Save the current model to disk and load it for later use.
- **Train on Custom Data:** Train the model using your own dataset.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/mcaramba563/final_project_git.git
   cd final_project_git
   ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. To start app
   ```bash
   python main.py
   ```
3. Create a Custom Model
To create a model with specific hidden layers:
    ```bash
    make_custom_model 'array of layers'"
    ```
Example:
    ```bash
    make_custom_model 400 256 128"
    ```

2. Train on Random Images
To train the model on N random images for epochs with a specific learning rate
    ```bash
    python -c "from app import do_train_on_random_images; do_train_on_random_images(['train_on_random_images', '20000', '2', '0.01'])"
    ```

3. Predict an Image
To make a prediction for a specific image
    ```bash
    python -c "from app import do_predict; do_predict(['predict', 'images/mnist_png/test/0/10.png'])"
    ```

4. Save the Model
To save the current model:
    ```bash
    python -c "from app import do_save_model; do_save_model(['save_model', 'models/my_model.npy'])"
    ```

5. Load a Model
To load a previously saved model:
    ```bash
    python -c "from app import do_load_custom_model; do_load_custom_model(['load_custom_model', 'models/my_model.npy'])"
    ```
