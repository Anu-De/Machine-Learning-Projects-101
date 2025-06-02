Project Report: Fashion MNIST Classification Using CNN

1. Dataset Overview


The Fashion MNIST dataset comprises 70,000 grayscale images of 28x28 pixels, categorized into 10 fashion apparel classes such as T-shirts, trousers, shoes, etc. The data is split into training (60,000) and testing (10,000) samples.

2. Data Preprocessing  

    Normalization: Pixel values were scaled from the range [0, 255] to [0, 1] to improve training stability.
    Reshaping: The images were reshaped to include a single channel dimension, resulting in shape (28, 28, 1), suitable for CNN input.

3. Model Architecture
A Convolutional Neural Network (CNN) was constructed with the following layers:

    Conv2D layer with 32 filters, 3x3 kernel, ReLU activation
    MaxPooling2D with 2x2 pool size
    Conv2D with 64 filters, 3x3 kernel, ReLU activation
    MaxPooling2D with 2x2 pool size
    Flatten layer to convert 2D feature maps to 1D feature vectors
    Dense layer with 64 units and ReLU activation
    Output Dense layer with 10 units and softmax activation for multi-class classification

4. Training Results
The model was trained for 10 epochs with the following key metrics:

    Epoch-wise accuracy and validation accuracy:
        Epoch 1: 77.16% accuracy, 87.03% val accuracy
        Epoch 10: 95.23% accuracy, 91.07% val accuracy
    Training loss decreased steadily across epochs, indicating effective learning.

5. Model Performance  

    Test Accuracy: 90.89%
    Test Loss: 0.2963
    The model demonstrated good generalization to unseen data, with validation accuracy stabilizing around 91%.

6. Conclusion
The CNN effectively learned to classify fashion items with over 90% accuracy. The architecture, combined with proper normalization and reshaping, contributed to robust performance. Future improvements could involve hyperparameter tuning, data augmentation, or advanced CNN architectures to potentially increase accuracy further.
