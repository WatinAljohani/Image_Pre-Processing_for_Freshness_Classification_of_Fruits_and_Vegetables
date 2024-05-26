# Image Pre-Processing for Freshness Classification of Fruits and Vegetables

### Project Overview

This project tackles the critical issue of food waste caused by unclear expiration labels by enhancing the classification accuracy of fruits and vegetables through advanced image processing techniques. The primary objective is to develop an effective image pre-processing methodology to support machine learning models in accurately determining the quality and category of fruits and vegetables.

### Methodology

1. **Image Pre-Processing**:
   - Convert images to HSV color space.
   - Apply thresholding.
   - Utilize morphological operations such as closing and dilation.

2. **Models Used**:
   - **ResNet-18 Convolutional Neural Network (CNN)**: Adapted with additional dense layers for multi-label classification, predicting both the fruit's name and its freshness.
   - **Vision Transformer (ViT)**: Fine-tuned for our dataset, demonstrating superior performance in capturing intricate image features through its transformer architecture.

### Results

- **ViT Model**:
  - Achieved 100% accuracy for fruit type classification.
  - Achieved 98% accuracy for fruit quality assessment.

- **ResNet-18 Model**:
  - Achieved 100% accuracy for fruit type classification.
  - Achieved 99% accuracy for fruit quality assessment.

### Conclusion

Our image pre-processing techniques significantly improve classification accuracy. The superior performance of the ViT model highlights its potential in addressing food waste by enhancing the precision of freshness classification in fruits and vegetables.
