# MNIST Handwritten Digit Recognition Using Deep Learning

A beginner-friendly Deep Learning project for handwritten digit recognition using TensorFlow, Keras and the MNIST dataset.

## About the Project

This was my first hands-on Deep Learning project. I built and trained a neural network to recognize handwritten digits from 0 to 9.

The project covers the basic Deep Learning workflow:

**Dataset → Preprocessing → Neural Network → Training → Evaluation → Prediction**

## Dataset

The project uses the MNIST handwritten digit dataset.

- 60,000 images for training
- 10,000 images for testing
- Image size: 28 × 28 pixels
- 10 classes: digits 0–9
- Grayscale images

The pixel values were normalized from 0–255 to a range of 0–1 before training.

## Deep Learning Model

The neural network was built using TensorFlow and Keras.

The model consists of:

- **Flatten layer** — converts each 28 × 28 image into 784 input values
- **Dense layer with 128 neurons** — learns patterns from the pixel data using ReLU activation
- **Output layer with 10 neurons** — predicts the probability of each digit from 0 to 9 using Softmax activation

The model was trained for **5 epochs** using the **Adam optimizer**.

## Training Performance

The model's training and validation accuracy improved during the 5 training epochs.

![Training and Validation Accuracy](https://github.com/user-attachments/assets/7ad301e5-a3f3-4aa0-b1f2-f907904693f8)

## Results

The model was evaluated on 10,000 test images that were not used during training.

| Metric | Result |
|---|---:|
| Test Accuracy | **97.66%** |
| Test Loss | **0.0789** |

The model achieved a test accuracy of **97.66%**, showing that it was able to correctly recognize most of the unseen handwritten digits.

## Confusion Matrix

The confusion matrix shows the number of correct and incorrect predictions for each digit.

![Confusion Matrix](https://github.com/user-attachments/assets/26289bae-91d3-4740-bcec-ae25e7c2f0c6)

Most predictions are along the diagonal, which represents correctly classified digits.

## Sample Predictions

Here are some sample predictions made by the trained model:

![Sample Predictions](https://github.com/user-attachments/assets/e8674601-0afc-4324-bfe7-84b552c3fb6f)

The model correctly recognized most of these sample digits. Some handwritten digits can still be misclassified when they look visually similar.

## Limitations

- The model was trained only on the MNIST dataset.
- The images are limited to 28 × 28 grayscale images.
- Performance may be lower on handwriting that looks very different from the MNIST examples.
- This project uses a basic neural network rather than a more advanced Convolutional Neural Network (CNN).

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## Project File

`MNIST_Handwritten_Digit_Recognition_DL.ipynb`

The complete implementation is available in the Jupyter Notebook included in this repository.

## What I Learned

Through this project, I got practical experience with:

- Preparing image data for Deep Learning
- Normalizing pixel values
- Building a neural network
- Training a model using TensorFlow/Keras
- Evaluating model performance
- Understanding confusion matrices
- Making predictions on unseen data
