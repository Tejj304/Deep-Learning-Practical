# Deep-Learning-Practical
ass 6 - Transfer Learning =>
https://towardsdatascience.com/transfer-learning-with-convolutional-neural-networks-in-pytorch-dd09190245ce
The basic premise of transfer learning is simple: take a model trained on a large dataset and transfer its knowledge to a smaller dataset. For object recognition with a CNN, we freeze the early convolutional layers of the network and only train the last few layers which make a prediction. The idea is the convolutional layers extract general, low-level features that are applicable across images — such as edges, patterns, gradients — and the later layers identify specific features within an image such as eyes or wheels.
Following is the general outline for transfer learning for object recognition:
Load in a pre-trained CNN model trained on a large dataset
Freeze parameters (weights) in model’s lower convolutional layers
Add custom classifier with several layers of trainable parameters to model
Train classifier layers on training data available for task
Fine-tune hyperparameters and unfreeze more layers as needed

