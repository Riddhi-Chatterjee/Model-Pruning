# Basic experiments on Model Pruning
Built-in pruning functionalities offered by PyTorch have been tried out and comparisons between different pruning approaches have been made using a pre-trained CNN for Cifar10 classification.
Refer: https://pytorch.org/tutorials/intermediate/pruning_tutorial.html

## Files used:
* cifar10-classification: A notebook for classification on the cifar10 dataset.
* cifar_net.pth: A pretrained model for classification on the cifar10 dataset, as obtained from the cifar10-classification notebook.
* model-pruning: A notebook for carrying out basic experiments on model pruning using built-in pruning utilities available in PyTorch.

## Libraries to install:
* torch
* torchvision
* scipy
* numpy
* sklearn
* matplotlib

## Steps to be followed:
* Use requirements.txt file to configure your conda environment according to the one that has been originally used.
* Execute the cifar10-classification notebook to obtain a CNN model trained for classification on the cifar10 dataset. Such a model has already been provided (cifar_net.pth).
* Execute the model-pruning notebook to try out all the built-in pruning techniques provided by PyTorch.

## Note:
For executing the model-pruning notebook, download the cifar_net.pth model as well, and set the PATH variable in the notebook to the appropriate path of the cifar_net.pth file.
cifar_net.pth is a model trained using cuda enabled. If your device doesn't support cuda, execute the cifar10-classification notebook to obtain your own pretrained model for pruning.