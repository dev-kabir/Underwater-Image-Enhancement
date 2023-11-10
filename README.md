# Underwater Image Enhancement Project

## Introduction

This project is dedicated to enhancing the quality of underwater images through the application of the FUNIE-GAN (FusionGAN for Underwater Image Enhancement) technique. Underwater imaging poses unique challenges due to factors such as low light, reduced clarity, and color distortion. The primary objective of this project is to develop a solution for improving the visual quality of underwater images.

## Data Collection and Preparation

### Data Collection

The initial step of this project involved collecting a dataset of underwater images. Underwater videos were obtained from various sources on the internet, and frames were extracted from these videos at a rate of 30 frames per second using FFmpeg. These extracted frames serve as the ground truth images for the project.

### Data Degradation

To comprehensively test the FUNIE-GAN model, a set of degraded images was created to simulate the challenges frequently encountered in underwater photography. A Python script was developed for this purpose. The script introduced various degradation effects to the original images, including:

- Illumination changes
- Reduced contrast
- Color cast
- Added noise
- Gaussian blur
- Foggy conditions
- Desaturation

## Model Loading

After preparing the dataset of degraded images, the FUNIE-GAN model was pre-trained and loaded for testing. The model architecture and weights were loaded from the specified checkpoint directory, enabling subsequent testing of the model's performance.

## Testing Process

The central component of this project involved conducting tests on the FUNIE-GAN model using the dataset of degraded underwater images. The testing process included several stages:

1. **Image Preprocessing**: Each image in the test dataset was preprocessed, which involved resizing the image to a fixed size of 256x256 pixels and normalizing it to prepare it for input to the model. The preprocessed image was expanded to match the expected input shape for the model (1, 256, 256, 3).

2. **Image Enhancement**: The FUNIE-GAN model was utilized to generate enhanced versions of the degraded underwater images. The model's prediction for each image was computed, resulting in an improved image.

3. **Image Saving**: Both the input (degraded) and enhanced images were saved. These images were stored side by side, enabling a direct visual comparison between the original degraded image and the enhanced result. The saved images facilitated the assessment of the model's capabilities in improving underwater image quality.

## Statistics

Upon the completion of the testing loop, the project generated critical statistics:

- The total number of test images in the dataset.
- The cumulative processing time for enhancing all images.
- The average frames per second (FPS) achieved during the testing process. This was calculated as the reciprocal of the mean processing time, providing insights into the efficiency of the image enhancement process.
- The MSE and PSNR results of dataset

## Dependencies

To run this project, you will need the following Python packages. You can install them using the provided requirements.txt file.

## Installation

1. Clone this repository.
2. Create a Python virtual environment (recommended).
3. Install the required dependencies using pip:
   ```bash
   pip install -r requirements.txt
