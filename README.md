# Perceptron Neural Network Application

This repository contains a neural network application implementing a multilayer perceptron for image recognition tasks, such as digit recognition using the MNIST dataset. The app allows you to train, predict, save, and load models easily.

---

## Features

- **Create Custom Models**: Define the number of neurons in hidden layers.
- **Train on Custom Data**: Train the model using your own dataset.
- **Train on Random Images**: Train the model on randomly selected images.
- **Make Predictions**: Predict the class label for an input image.
- **Save and Load Models**: Save the current model to disk and load it for later use.
- **Load Default Model**: Reset the model to the default pretrained configuration.
- **Reset Training**: Revert the current model to its state before any training.

---

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

# Start the App
Run the app in interactive mode:
    ```bash
    python main.py```

# Features and Commands
1. Create a Custom Model
Create a model with specific hidden layer sizes:

    ```bash
    make_custom_model layer1_size layer2_size
    ```
Example:
    ```bash
    make_custom_model 400 256 128
    ```

# Train on Custom Data
Train the model on labeled data from a specified file:

    ```bash
    train path_to_dataset_file number_of_epochs learning_rate
    ```
Example:

    ```bash
    train dataset/train_data.txt 5 0.01
    ```

# Train on Random Images
Train the model on randomly selected images:

```bash
train_on_random_images number_of_images number_of_epochs learning_rate
Example:

```bash
train_on_random_images 20000 2 0.01
Make Predictions
Predict the class of a given image:

```bash
predict path_to_image
Example:

```bash
predict images/mnist_png/test/0/10.png
Save the Model
Save the current model to a file:

```bash
save_model path_to_model_file
Example:

```bash
save_model models/my_model.npy
Load a Custom Model
Load a previously saved model:

```bash
load_custom_model path_to_model_file
Example:

```bash
load_custom_model models/my_model.npy
Load Default Model
Reset the model to its default pretrained state:

```bash
load_default_model
Reset Training
Revert the current model to its initial state before training:

```bash
reset_training
Exit the Application
Exit the interactive mode:

```bash
exit
Example Workflow
Start the app:

```bash
python main.py
Create a custom model with hidden layers of sizes 400, 256, and 128:

```bash
make_custom_model 400 256 128
Train on custom data for 5 epochs with a learning rate of 0.01:

```bash
train dataset/train_data.txt 5 0.01
Save the trained model:

```bash
save_model models/my_trained_model.npy
Load the default pretrained model:

```bash
load_default_model
Predict the class of a test image:

```bash
predict images/mnist_png/test/0/10.png
Exit the app:

```bash
exit```



