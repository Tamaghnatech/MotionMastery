# MotionMastery
Predicting Human Activity using Neural Networks



## Introduction
Human Activity Recognition (HAR) plays a pivotal role in various applications, especially with the advent of wearable technologies. Our project aims to recognize and classify human movements into activities such as walking, jogging, and sitting using deep learning.

![NeuroStride Logo](path_to_logo_image_if_you_have_one.png)

## Dataset Overview
We utilize the `human.csv` dataset that houses accelerometer data with `x`, `y`, and `z` axes measurements. Each entry is coupled with a timestamp, user identifier, and the corresponding activity label. The range of activities spans Walking, Jogging, Going Upstairs, Going Downstairs, Sitting, and Standing, among others.

## Model Architecture
Our deep learning solution is a multi-layer perceptron with the following design:

1. Input layer suited to the number of features.
2. Dense layer consisting of 128 neurons with RELU activation.
3. 20% Dropout layer for regularization.
4. Dense layer with 64 neurons, and RELU activation.
5. Another 20% Dropout layer.
6. Dense layer boasting 32 neurons, powered by RELU activation.
7. Output layer employing softmax activation, tailored for the number of activity labels.

The model leans on the Adam optimizer and was diligently trained on a `sparse_categorical_crossentropy` loss function, given our labels aren't one-hot encoded.

## Training Insights
Our neural model exhibited remarkable efficiency, showing rapid convergence across epochs. By the closing epoch, it proudly posted an impressive 94.59% training accuracy. Additionally, the validation accuracy was approximately 95.98%, suggesting that our model is proficiently tuned without any glaring overfitting concerns.

## Visualization and Animation
For an enriched, tangible understanding of data propagation through our model, we engaged tools such as TensorBoard. Such platforms offer an insightful lens to view the architecture, and comprehend weight distributions and gradients.

For those keen on a more animated visual experience, we have cultivated a tailored visualization on Google Colab, elucidating the data journey through each neuron. Feel free to delve into it:
[NeuroStride on Google Colab](https://colab.research.google.com/drive/132g6zNRSkz3Gy6mfWkaXr63ZUGU6O2M0#scrollTo=tmT1lGyyuK4I)

## Future Directions
While our current model is potent, the realm of HAR is vast. Prospective explorations might encompass recurrent neural networks or convolutional architectures, aiming to further harness the time-series essence of our data and escalate recognition precision.

## Contribute
Feel free to fork this repository, raise issues, or propose changes. All contributions are warmly welcomed!

---

Remember, you can further enhance the README by adding badges, contribution guidelines, and setting up instructions if required. This layout should serve as a solid starting point!
