# Part 2: Computer Vision Problem Formulation and CNN Prototype

## Dataset
Source: https://drive.google.com/drive/folders/1akV6po4Nrgkc3yQrJkzA6cJIV-wBvUYs

## Problem Type: Image Classification
The dataset contains labelled image folders. Each image is assigned to one
category. This is a supervised multi-class classification problem.

## CNN Concept Explanations

**What is convolution?**
A small filter (kernel) slides over the image computing dot products at each
position, detecting local patterns such as edges and textures. Different
filters learn different features automatically.

**Why is pooling used?**
MaxPooling reduces spatial dimensions, making the model robust to small
position shifts (translation invariance) and cutting computation.

**Why ReLU in CNNs?**
ReLU (max(0,x)) introduces non-linearity without the vanishing gradient
problem of sigmoid/tanh. It is fast and keeps gradients flowing.

**CNNs vs Feed-Forward Networks**
Regular networks treat every pixel independently, losing spatial structure.
CNNs use shared filters to capture local patterns, using far fewer parameters.

## Business Use Case: Manufacturing Quality Inspection
- Input: Product surface images from factory cameras
- Output: Defect class (normal / scratch / dent / stain)
- Impact: Automated real-time quality control, reducing manual inspection cost and catching defects before products leave the production line.

## Results
- Validation Accuracy: 0.2500
