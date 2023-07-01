# Filter Pruning via Geometric Median (FPGM)
The FPGM pruning approach has been tried out on a vgg16 model on the cifar10 and cifar100 datasets, with different amounts of fine-tuning after pruning.
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
* torch-pruning

## Note:
Please ensure the following before running the notebooks:
* torch.cuda.is_available() must be True
* The folders "fpgmdata" and "pretrainedmodel" must be present in the same directory as the notebooks.
* Since the folders "fpgmdata" and "pretrainedmodel" contain large files, they have been stored using Git LFS. Ensure that you have cloned this repository and haven't downloaded the code as a zip file.

## Contributing
All contributions are appreciated, including bug fixes, new experiments, documentation, and more tutorials. Contributions can be initiated via Github pull requests.