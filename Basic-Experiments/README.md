# Basic experiments on Model Pruning
Built-in pruning functionalities offered by PyTorch have been tried out and comparisons between different pruning approaches have been made using a pre-trained CNN for Cifar10 classification.
Refer: https://pytorch.org/tutorials/intermediate/pruning_tutorial.html

## A simple example -- for demo purposes
A simple experiment has been performed where PyTorch's L1 Structured Pruning utility has been used. We chose a CNN model trained for classification on the cifar10 dataset (cifar_net.pth) with an original accuracy of 78%. 

After pruning 40% of the channels/filters (having least L1 norm) of the 1st convolutional layer, we get rid of 2862 (0.019%) weight parameters, and the accuracy drops to 76%.

We observe that after pruning, weights of some of the filters have been set to zero (i.e. pruned). We also obtain a weight mask after pruning. Internally, this weight mask is multiplied element-wise with the original weight parameter to obtain the final (pruned) weight parameter of the module

## Files used
* cifar10-classification: A notebook for classification on the cifar10 dataset.
* cifar_net.pth: A pretrained model for classification on the cifar10 dataset, as obtained from the cifar10-classification notebook.
* model-pruning: A notebook for carrying out basic experiments on model pruning using built-in pruning utilities available in PyTorch.

## System specifications
The experiments have been performed on a machine with the following specifications:
* Operating system: macOS Ventura (Version 13.4)
* Processor: Apple M1 Pro
* Architecture: arm64
* RAM: 16GB
* conda version: conda 4.14.0

## Libraries to install
* torch
* torchvision
* scipy
* numpy
* sklearn
* matplotlib

## Steps to be followed
* Use requirements.txt file to configure your conda environment according to the one that has been originally used.
* Execute the cifar10-classification notebook to obtain a CNN model trained for classification on the cifar10 dataset. Such a model has already been provided (cifar_net.pth).
* Execute the model-pruning notebook to try out all the built-in pruning techniques provided by PyTorch.
*** Windows specific steps: ***
* conda create -n environment_name
* conda activate environment_name
* conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
* conda install scipy
* conda install -c intel scikit-learn
* conda install matplotlib
* conda install jupyterlab

## Note:
For executing the model-pruning notebook, download the cifar_net.pth model as well, and set the PATH variable in the notebook to the appropriate path of the cifar_net.pth file.

cifar_net.pth is a model trained using cuda enabled. If your device doesn't support cuda, execute the cifar10-classification notebook to obtain your own pretrained model for pruning.

## Contributing
All contributions are appreciated, including bug fixes, new experiments, documentation, and more tutorials. Contributions can be initiated via Github pull requests.