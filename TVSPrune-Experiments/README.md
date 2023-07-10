# TVSPrune - Pruning Nondiscriminative Filters via Total Variation Separation of Intermediate Representations without fine tuning
The TVSPrune approach has been tried out on vgg16 and vgg11 on the cifar10 dataset. Test accuracy, inference time, and model size compression results have been obtained.

Refer: https://github.com/chaimurti/TVSPrune

## System specifications
The experiments have been performed on a machine with the following specifications:
* Operating system: macOS Ventura (Version 13.4)
* Processor: Apple M1 Pro
* Architecture: arm64
* RAM: 16GB
* conda version: conda 4.14.0

## Libraries to install
* torch
* torch-pruning
* torchvision
* scipy
* numpy
* sklearn
* matplotlib
* urllib (urllib.request is required)

## Note:
Please ensure the following before running the notebooks:
* torch.cuda.is_available() must be True

## Contributing
All contributions are appreciated, including bug fixes, new experiments, documentation, and more tutorials. Contributions can be initiated via Github pull requests.