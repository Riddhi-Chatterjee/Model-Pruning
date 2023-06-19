# Basic experiments on Model Pruning
* cifar10-classification: A notebook for classification on the cifar10 dataset.
* distpruning-cifar10-vgg11: A notebook implementing TVSPrune model-pruning approach for the cifar10 dataset and vgg11 model. 
Refer: TVSPrune - Pruning Non-discriminative filters via Total Variation separability of intermediate representations without fine tuning
* model-pruning: A notebook for carrying out basic experiments on model pruning using in-built pruning utilities available in PyTorch.

## Requirements:
* torch
* torchvision
* scipy
* numpy
* sklearn
* matplotlib

## Note:
For executing the model-pruning notebook, download the cifar_net.pth model as well, and set the PATH variable in the notebook to the appropriate path of the cifar_net.pth file.