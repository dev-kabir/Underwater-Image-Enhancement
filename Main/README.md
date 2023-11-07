There are 5 ipynb files:
  1. DCE.ipynb - It is used to compare 3 datasets by aggregated MSE Loss and PSNR values. It selects random 890 images from all 3 datasets.
           It enhances those images and saves them in the output folder.
           *Datasets:
             a) EUVP
             b) UIEB
             c) Degraded (It is a custom dataset which contains images with simulated underwater degradation effects)
           
           
  2. Dataset-Coparision.ipynb - It compares all 3 datasets and provides aggregated MSE Loss and PSNR values from the random 890 images of each dataset.
  
  
  3. Each-Image.ipynb - It selects random 890 images from all 3 datasets. Then it provides MSE Loss and PSNR values of each image. 
                  It enhances those images and saves them in the output folder.


  4. test.ipynb - It takes input from the provided images in the "data/test/A" folder. Then it enhances them and saves in the output folder.


  5. Degrade.ipynb - This script helps to degrade any underwater images into 7 types :
 - Illumination: Variations in lighting conditions underwater.
- Low Contrast: Reduced differentiation between objects and their background.
- Color Cast: Unwanted color shifts in images.
- Noisy: Presence of random, unwanted elements in the image.
- Blurred: Loss of image sharpness and details.
- Foggy: Simulation of foggy conditions underwater.
- Desaturated: Reduction in image color intensity.




Download the datasets:

1. EUVP: https://www.kaggle.com/datasets/pamuduranasinghe/euvp-dataset
2. UIEB: https://www.kaggle.com/datasets/larjeck/uieb-dataset-raw


**To create a degrade dataset use Degrade.ipynb on: https://teraboxapp.com/s/1oVhanbLyTnncq909X6f_gw
                          
