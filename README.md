# AIML Recruitment 2026 — Task 2: Neural Network

## Candidate Details

-**Name:**Enduri Krishna Pranathi
-**Year:** 2nd Year
-**Task:** Task 2 — Neural Network
-**Dataset:** MNIST Handwritten Digit Database

---

## Problem Statement

The objective of this task is to build and train a simple neural network to classify handwritten digits from 0 to 9 using the MNIST dataset.

The project also analyses how changing a component of the neural network affects its performance.

---

## Dataset

The MNIST dataset contains grayscale images of handwritten digits from 0 to 9.

* Image size: 28 × 28 pixels
* Number of classes: 10
* Classes: Digits 0 through 9
* Training samples: 60,000
* Testing samples: 10,000

---

## Approach

The project was completed using the following steps:

1. Loaded the MNIST dataset.
2. Inspected the dataset and visualized sample handwritten digits.
3. Normalized pixel values from the range 0–255 to 0–1.
4. Flattened each 28 × 28 image into a 784-element vector.
5. Built a feedforward neural network.
6. Used ReLU activation in the hidden layer.
7. Used Softmax activation in the output layer.
8. Trained the model using the Adam optimizer.
9. Evaluated the model using test accuracy, loss, confusion matrix, and classification metrics.
10. Performed an experiment by increasing the hidden-layer neurons from 128 to 256.

---

## Neural Network Architecture

### Original Model

* Input layer: 784 features
* Hidden layer: 128 neurons
* Hidden activation: ReLU
* Output layer: 10 neurons
* Output activation: Softmax

### Modified Model

For the experiment, the hidden layer was changed from 128 neurons to 256 neurons.

All other major training settings were kept the same for comparison.

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab
* GitHub

---

## Results

### Original Model

| Metric         |  Result |
| -------------- | ------: |
| Hidden neurons |     128 |
| Test Loss      | 0.07389 |
| Test Accuracy  |  97.82% |

### Modified Model

| Metric         |  Result |
| -------------- | ------: |
| Hidden neurons |     256 |
| Test Loss      | 0.06361 |
| Test Accuracy  |  98.07% |

Increasing the hidden-layer size from 128 to 256 neurons increased the test accuracy from 97.82% to 98.07%. The test loss also decreased from 0.07389 to 0.06361.

The improvement was relatively small because the original model was already performing well on the MNIST dataset.

---

## Evaluation

The model was evaluated using:

* Test accuracy
* Test loss
* Confusion matrix
* Precision
* Recall
* F1-score

The confusion matrix was used to examine correct predictions along the diagonal and misclassifications between different digit classes.

---

## Key Learnings

1. Learned how to preprocess image data for a neural network.
2. Understood the role of ReLU and Softmax activation functions.
3. Learned how to build and train a neural network using TensorFlow/Keras.
4. Learned how to evaluate a classification model using accuracy and a confusion matrix.
5. Understood how changing the number of hidden neurons can affect model performance.

---

## Challenges

One challenge was understanding how image data can be provided to a fully connected neural network. MNIST images are originally 28 × 28 pixels, so they were flattened into 784 features before being passed to the network.

Another challenge was comparing the original and modified architectures fairly. To make the experiment meaningful, the main training settings were kept the same while changing the number of hidden neurons.

---

## Limitations

1. The model uses a simple fully connected architecture rather than a convolutional neural network designed specifically for image data.
2. Only one architectural change was tested in the experiment.
3. MNIST is relatively simple compared with more complex real-world image datasets.
4. More advanced architectures may provide better performance on more challenging image-classification problems.

---

## Future Improvement

A possible next step would be to implement a Convolutional Neural Network (CNN). CNNs are designed for image data and can learn spatial features such as edges, shapes, and patterns more effectively.

---

## Conclusion

A simple neural network was successfully developed to classify handwritten digits from the MNIST dataset. The original 128-neuron model achieved a test accuracy of 97.82%.

As an experiment, the hidden layer was increased to 256 neurons. The modified model achieved a test accuracy of 98.07% and a lower test loss of 0.06361.

This project demonstrated the complete workflow of preparing image data, building a neural network, training the model, evaluating its performance, and experimenting with the model architecture.
