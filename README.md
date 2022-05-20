# Thesis Shyrano Karia: Using Degradation Representation Learning For Super-Resolving Face Images
Most of the code used in this thesis was conducted from another Github repository: https://github.com/The-Learning-And-Vision-Atelier-LAVA/DASR. A few modifications to this code have been done. 

## Required packages
- Python, version 3.7.9
- CUDA, version 10.0
- PyTorch, version 1.1.0
- Numpy
- Scikit image
- Imageio
- Matplotlib
- OpenCV


## Train
### 1. Prepare training data 

Download the [SiblingsDB](https://areeweb.polito.it/ricerca/cgvg/siblingsDB.html) dataset and save the dataset in `your_data_path/DF2K/HR`.

### 2. Begin to train
Run `./main.sh` to train on the SiblingsDB dataset. Update `dir_data` in the bash file as `your_data_path`.

## Test
### 1. Prepare test data 

1.1 Download [real-human dataset](https://www.kaggle.com/datasets/hamzaboulahia/hardfakevsrealfaces) in `your_data_path/benchmark`.

1.2 Run `imageformat.ipynb` to make sure the images are formatted to .png files.

### 2. Begin to test
Run `./test.sh` to test on real-human dataset. Update `dir_data` in the bash file as `your_data_path`.


## Acknowledgements
This code is built on [DASR](https://github.com/The-Learning-And-Vision-Atelier-LAVA/DASR)[EDSR (PyTorch)](https://github.com/thstkdgus35/EDSR-PyTorch), [IKC](https://github.com/yuanjunchai/IKC) and [MoCo](https://github.com/facebookresearch/moco). I would like to thank the authors for sharing their code. 

