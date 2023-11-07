There are 4 ipynb files:
  1. DCE - It is used to compare 3 datasets by aggregated MSE Loss and PSNR values. It selects random 890 images from all 3 datasets.
           It enhances those images and saves them in the output folder.
           *Datasets:
             a) EUVP
             b) UIEB
             c) Degraded (It is a custom dataset which contains images with simulated underwater degradation effects)
           
           
  2. Dataset-Coparision - It compares all 3 datasets and provides aggregated MSE Loss and PSNR values from the random 890 images of each dataset.
  
  
  3. Each-Image - It selects random 890 images from all 3 datasets. Then it provides MSE Loss and PSNR values of each image. 
                  It enhances those images and saves them in the output folder.


  4. test - It takes input from the provided images in the "data/test/A" folder. Then it enhances them and saves in the output folder.
     
                          
