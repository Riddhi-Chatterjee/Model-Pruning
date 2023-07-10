# Filter Pruning via Geometric Median (FPGM)
The FPGM pruning approach has been tried out on ResNet models on the Cifar100 and ImageNet datasets (ResNet110 for Cifar100 and ResNet152 for ImageNet).
Refer: https://github.com/he-y/filter-pruning-geometric-median

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
* argparse
* numpy
* os
* shutil
* sys
* time
* random
* math

## Note:
Please ensure the following before running the notebooks:
* torch.cuda.is_available() must be True
* For Cifar100, the folder "resnet-fpgm-data" must be present in the same directory as the "fpgm-arch-pruning-resnet-cifar.ipynb" notebook.
* For ImageNet:
* * Firstly, download the "imagenet-object-localization-challenge" dataset from Kaggle into the same directory as the "fpgm-arch-pruning-resnet-imgnet.ipynb" notebook.
* * Secondly, the folder "resnet-imagenet-fpgm" must be present in the same directory as the "fpgm-arch-pruning-resnet-imgnet.ipynb" notebook.
* Since the folders "resnet-fpgm-data" and "resnet-imagenet-fpgm" contain large files, they have been stored using Git LFS. Ensure that you have cloned this repository and haven't downloaded the code as a zip file.

## Contributing
All contributions are appreciated, including bug fixes, new experiments, documentation, and more tutorials. Contributions can be initiated via Github pull requests.