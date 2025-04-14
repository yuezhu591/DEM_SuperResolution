# DEM_SuperResolution

# Project Title

This repository contains code and data produced in the study of “Improving Pluvial Flood Simulations with Multi-source DEM Super-Resolution”. The code and data are particularly for a proposed DEM super-resolution method that can enhance the spatial resolution of DEM data, which can contribute to improved performance in pluvial flood simulation.

## Dependencies

Please ensure the following versions are installed:
- Python == 3.6
- torch == 1.8.0
- torchvision == 0.8.0
- numpy == 1.19.2
- rasterio == 1.1.0
- pandas == 1.1.3  


## Project Structure

The dataset contains:
10m and 30m resolution DEM data, and 10m resolution multispectral images in Hong Kong and Shenzhen area.
 30m resolution DEM data and 10m multispectral images in the England area.

## Script Descriptions
## Script Descriptions

- `data/resample_dataset.py`:  
  Samples the raw data into small tiles for training, validation, and testing.
- `model/SRCNN.py`:  
  Script for one of the baseline DEM super-resolution models, SRCNN.
- `model/VDSR.py`:  
  Script for one of the baseline DEM super-resolution models, VDSR.
- `model/RCAN.py`:  
  Script for one of the baseline DEM super-resolution models, RCAN.
- `model/RCAN_MS_hr.py`:  
  Script for the proposed DEM super-resolution model, RCAN-MS.
- `pytorch_ssim/__init__.py`:  
  Contains the evaluation metric for the generated super-resolution DEM data.
- `train/train_SRCNN.py`:  
  Trains the SRCNN model using the sampled training dataset.
- `train/train_VDSR.py`:  
  Trains the VDSR model using the sampled training dataset.
- `train/train_RCAN.py`:  
  Trains the RCAN model using the sampled training dataset.
- `train/train_RCAN_MS_hr.py`:  
  Trains the proposed RCAN-MS model using the sampled training dataset.



## How to cite

Zhu, Y., Burlando, P., Tan, P. Y., Geiß, C., and Fatichi, S.: Improving Pluvial Flood Simulations with Multi-source DEM Super-Resolution, Nat. Hazards Earth Syst. Sci. Discuss. [preprint], https://doi.org/10.5194/nhess-2024-207, in review, 2024.

