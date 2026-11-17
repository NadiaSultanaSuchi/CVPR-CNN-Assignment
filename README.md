# CNN Assignment on NWPU RESISC45

Student: Nadia Sultana Suchi

ID: 23-53645-3

Course: CVPR

## Project

Satellite scene classification using a custom CNN. The model looks at a satellite image and tells what kind of place it is, such as forest, river, harbor or desert.

## Files

CNN_23_53645_3.ipynb : complete notebook with code, outputs, graphs and explanations

CNN_23-53645-3.pth : trained model weights, 8.38 MB

## Dataset

NWPU RESISC45 from Hugging Face: https://huggingface.co/datasets/timm/resisc45

The full dataset has 45 classes and 31,500 images. I used 10 classes: airport, beach, desert, forest, harbor, industrial area, lake, mountain, rectangular farmland and river.

Train: 4214 images, Validation: 1386 images, Test: 1400 images

The dataset downloads automatically when the notebook runs, so it is not uploaded here.

Citation: Cheng, Han and Lu, 2017, Remote sensing image scene classification: Benchmark and state of the art.

## Model

A custom CNN with 3 convolution blocks. Each block has Conv2d, BatchNorm, ReLU and MaxPool. After that come Flatten, a Linear layer, Dropout 0.5 and a final Linear layer with 10 outputs. The model has 2,193,674 parameters.

## Training Settings

Image size: 64 by 64

Batch size: 32

Optimizer: Adam

Learning rate: 0.001

Loss: Cross Entropy

Epochs: 20

## Result

Test accuracy: 80.36 percent

Test loss: 0.59

## How to run

Open the notebook in Google Colab, select GPU and run all cells.
