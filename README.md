# MNIST Handwritten Digits Recognition - C++ Machine Learning 

The MNIST database of handwritten digits, curated by Yann LeCun and others, is a widely used dataset in the machine learning community. This repository contains code and experiments related to training models on the MNIST dataset.

## Overview

The MNIST database consists of a training set with 60,000 examples and a test set with 10,000 examples of handwritten digits. The goal is to recognize and classify these digits using various machine learning techniques.

## Files

The dataset is provided in four files:

- `train-images-idx3-ubyte.gz`: Training set images
- `train-labels-idx1-ubyte.gz`: Training set labels
- `t10k-images-idx3-ubyte.gz`: Test set images
- `t10k-labels-idx1-ubyte.gz`: Test set labels

Please note the file formats and instructions for handling these files are detailed in the file format section below.

## Experiments

The repository includes experiments conducted on the MNIST dataset using various machine learning classifiers and techniques. Results from different classifiers and preprocessing methods are provided in the project documentation.

## Examples

Here are some examples of classifiers and their respective test error rates:

- **Linear Classifiers:**
  - Linear classifier (1-layer NN): 12.0% error
  - Pairwise linear classifier (deskewing): 7.6% error

- **K-Nearest Neighbors:**
  - K-nearest-neighbors, Euclidean (L2) (deskewing): 2.4% error
  - K-NN with non-linear deformation (IDM) (shiftable edges): 0.54% error

- **SVMs:**
  - SVM, Gaussian Kernel: 1.4% error
  - Virtual SVM, deg-9 poly, 2-pixel jittered (deskewing): 0.56% error

- **Neural Nets:**
  - 2-layer NN, 300 HU (deskewing): 1.6% error
  - 3-layer NN, 500+300 HU, softmax, cross entropy (no distortions): 1.53% error

- **Convolutional Nets:**
  - Convolutional net LeNet-5 (no distortions): 0.8% error
  - Large/deep conv. net, 1-20-40-60-80-100-120-120-10 (elastic distortions): 0.35% error

## How to Use

1. Download the MNIST dataset files from the provided links.
2. Extract the dataset files and ensure they are in the correct format.
3. Explore the experiments and examples in the repository to understand different approaches to solving the MNIST classification problem.

Feel free to contribute your own experiments, improvements, or additional classifiers to this repository.

## File Formats for the MNIST Database

The IDX file format is used to store vectors and multidimensional matrices of various numerical types. Refer to the [IDX file format section](#the-idx-file-format) for more details on handling these files.

## References

- Y. LeCun, L. Bottou, Y. Bengio, and P. Haffner. "Gradient-based learning applied to document recognition." Proceedings of the IEEE, 86(11):2278-2324, November 1998. [on-line version]

- Additional references and details about experiments can be found in the provided documentation.

## Contributors

- Yann LeCun (Professor, The Courant Institute of Mathematical Sciences, New York University)
- Corinna Cortes (Research Scientist, Google Labs, New York)

Happy hacking!
