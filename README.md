# CNN for Arbitrary Input Dimensions

## Motivation

While building Convolutional Neural Networks (CNNs), managing input dimensions can be challenging, as slight changes in dimensions can affect the entire architecture. Therefore, a generic structure is needed that accepts any input dimension.

## Goal

The goal is to build a CNN that can accept any input dimensions and can be used as a feature extractor for images with arbitrary dimensions.

## Objective

To construct a CNN capable of accepting any input dimensions and functioning as a feature extractor for images with arbitrary dimensions.

## Performance Metric

- Overall Accuracy
- Multi-class Precision and Recall

## Dataset

- **Source:** [Fashion-MNIST](https://research.zalando.com/project/fashion_mnist/fashion_mnist/)
- Fashion-MNIST is a dataset of Zalando’s article images consisting of 60,000 training examples and 10,000 test examples. Each example comprises a 28×28 grayscale image and an associated label from one of 10 classes.

## Experiment

The experiment involves building a CNN architecture that can handle arbitrary input dimensions using the principle of encapsulation and ADAPTIVE AVG POOL


### References

- [PyTorch Tutorials - Data](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html)
- [PyTorch Tutorials - Quickstart](https://pytorch.org/tutorials/beginner/basics/quickstart_tutorial.html)
- [PyTorch Documentation - AdaptiveAvgPool2d](https://pytorch.org/docs/stable/generated/torch.nn.AdaptiveAvgPool2d.html)
