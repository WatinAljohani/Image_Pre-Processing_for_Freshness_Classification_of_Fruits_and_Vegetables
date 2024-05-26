# Image Pre-Processing for Freshness Classification of Fruits and Vegetables

### Project Overview

This project tackles the critical issue of food waste caused by unclear expiration labels by enhancing the classification accuracy of fruits and vegetables through advanced image processing techniques. The primary objective is to develop an effective image pre-processing methodology to support machine learning models in accurately determining the quality and category of fruits and vegetables.

### Image Processing Techniques

The project uses morphological operations and image segmentation to enhance the classification of fruits and vegetables. The primary steps in the image processing methodology are:

1. **Importing Images**: Extract and verify images from the dataset zip file using a loop.
2. **Color Space Conversion**: Convert images from BGR to RGB for better control.
3. **Alpha and Beta Adjustments**: Enhance image quality by adjusting brightness (beta) and contrast (alpha).
4. **Resize Images**: Standardize images to 224x224 pixels.
5. **Convert to HSV Color Space**: Separate color information from brightness by converting images from RGB to HSV.
6. **Extract Saturation Channel**: Use the saturation (S) channel for color-based segmentation and object detection.
7. **Thresholding**: Apply a binary threshold to the S-channel to distinguish fruits and vegetables from the background.
8. **Morphological Operations**: Use closing to bridge gaps and dilation to expand segmented regions for smoother segmentation.
9. **Bitwise AND Operation**: Merge the segmented mask with the RGB image to highlight the desired regions.

### Models Used

- **ResNet-18 Convolutional Neural Network (CNN)**: Adapted with additional dense layers for multi-label classification, predicting both the fruit's name and its freshness.
- **Vision Transformer (ViT)**: Fine-tuned for our dataset, demonstrating superior performance in capturing intricate image features through its transformer architecture.

### Results

- **ViT Model**:
  - Achieved 100% accuracy for fruit type classification.
  - Achieved 98% accuracy for fruit quality assessment.

- **ResNet-18 Model**:
  - Achieved 100% accuracy for fruit type classification.
  - Achieved 95% accuracy for fruit quality assessment.

### Conclusion

Our image pre-processing techniques significantly improve classification accuracy. The superior performance of the ViT model highlights its potential in addressing food waste by enhancing the precision of freshness classification in fruits and vegetables.
