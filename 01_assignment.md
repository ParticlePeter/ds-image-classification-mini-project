# Webcam Image Classifier: Assignment

In this mini project you build your own image classifier and then use it on a picture you choose yourself. It is a short, hands-on introduction to convolutional neural networks (CNNs): you train a model on a standard image dataset, then apply it to a new image, ideally one you capture with your webcam.

The project comes in two parts. Work through them in order using the scaffolded notebook, [02_starter_notebook.ipynb](02_starter_notebook.ipynb). The notebook carries the detailed, step-by-step instructions; this file is the brief and the list of deliverables.

## What you will build

- **Part A: train a CNN.** Build and train a simple convolutional neural network on the CIFAR-100 image dataset, then evaluate how well it classifies images it has not seen.
- **Part B: apply the model.** Feed the trained model a new image (a webcam snapshot or any photo) and let it predict what the picture shows. Optionally, grow this into a small standalone application.

## Setup

Follow the steps in the [README](README.md) to install the environment with `uv` and open the notebook in VS Code. Then start with Part A in [02_starter_notebook.ipynb](02_starter_notebook.ipynb).

## Deliverables

1. A trained CNN, saved to disk (for example `webcam_classifier.keras`) so you can reload it without retraining.
2. A working prediction on a new image: the model loaded back from disk and used to classify a picture you supply.
3. **Optional:** a standalone application that combines image capture and prediction.
4. **Optional:** a public repository sharing what you built, even if you only complete some of the steps.

## Things to think about

- How does each layer change the shape of the data as it flows through the network?
- The starting accuracy will be low. Which changes (more layers, more training, different preprocessing) improve it, and which do not?
- Your new image has to match the training format before the model can use it: the same pixel size, colour format, and normalisation.

## Resources

- [Conv2D](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Conv2D), [MaxPool2D](https://www.tensorflow.org/api_docs/python/tf/keras/layers/MaxPool2D), [Flatten](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Flatten), and [Dense](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Dense) layer documentation.
- [Model.fit](https://www.tensorflow.org/api_docs/python/tf/keras/Model#fit) for training.
- [bonartm/imageclassifier](https://github.com/bonartm/imageclassifier): a small standalone webcam capture helper you can use for Part B.
