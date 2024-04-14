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

The experiment involves building a CNN architecture that can handle arbitrary input dimensions. The dataset used is Fashion-MNIST.

### Results

#### Training Data

- **Classification Report:**
  - precision    recall  f1-score   support

     T-Shirt       0.66      0.77      0.71      6000
     Trouser       0.98      0.91      0.94      6000
    Pullover       0.52      0.67      0.59      6000
       Dress       0.72      0.83      0.77      6000
        Coat       0.58      0.57      0.58      6000
      Sandal       0.79      0.82      0.81      6000
       Shirt       0.41      0.19      0.26      6000
     Sneaker       0.83      0.77      0.80      6000
         Bag       0.93      0.88      0.90      6000
  Ankle Boot       0.83      0.92      0.87      6000

    accuracy                           0.73     60000
   macro avg       0.73      0.73      0.72     60000
weighted avg       0.73      0.73      0.72     60000

#### Testing Data

- **Classification Report:**
  |     Class     | Precision | Recall | F1-Score | Support |
|:-------------:|:---------:|:------:|:--------:|:-------:|
|    T-Shirt    |    0.65   |  0.75  |   0.69   |  1000   |
|    Trouser    |    0.98   |  0.91  |   0.94   |  1000   |
|   Pullover    |    0.51   |  0.67  |   0.58   |  1000   |
|     Dress     |    0.72   |  0.80  |   0.75   |  1000   |
|      Coat     |    0.57   |  0.57  |   0.57   |  1000   |
|     Sandal    |    0.82   |  0.82  |   0.82   |  1000   |
|     Shirt     |    0.36   |  0.17  |   0.23   |  1000   |
|    Sneaker    |    0.84   |  0.80  |   0.82   |  1000   |
|      Bag      |    0.91   |  0.88  |   0.90   |  1000   |
|  Ankle Boot   |    0.82   |  0.93  |   0.87   |  1000   |
|   **Accuracy**   |         |        |   0.73   |  10000  |
|  **Macro Avg**  |    0.72   |  0.73  |   0.72   |  10000  |
| **Weighted Avg**|    0.72   |  0.73  |   0.72   |  10000  |

### References

- [PyTorch Tutorials - Data](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html)
- [PyTorch Tutorials - Quickstart](https://pytorch.org/tutorials/beginner/basics/quickstart_tutorial.html)
- [PyTorch Documentation - AdaptiveAvgPool2d](https://pytorch.org/docs/stable/generated/torch.nn.AdaptiveAvgPool2d.html)
