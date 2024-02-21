# CNN-Colorized-MNIST
CNN models created to classify randomly colorized MNIST data

Data from the MNIST handwritten digit dataset was randomly colorized to either 1 hue (hue on white background) or 2 hues (hue on second hue background).

The models were the LeNet model developed by LeCun (modified to take an input of 3 values per pixel instead of 1) and two variations of the AlexNet model by Krizhevsky (modified to take an image size of 32x32 pixels).
The AlexNet models were made of 2 convolution (sigmoid) layers (each followed by a pooling layer), 2 convolution (ReLU) layers, a pooling layer, a flattening layer, and finally 3 dense layers.
The AlexNet models proved to be overly complex; the LeNet model was more accurate and had less loss for each iteration of the dataset.

As predicted, colorizing the dataset led to every model being less accurate (LeNet Val Accuracy for the Original, 1-Hue, and 2-Hue datasets: 0.961, 0.958, 0.872).
