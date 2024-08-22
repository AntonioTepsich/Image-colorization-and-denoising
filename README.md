# Image Colorization and Denoising
with Pix2Pix and DnCNN

### Authors
This repository was made by:
 - Antonio Tepsich | atepsich@udesa.edu.ar 
 - Maximo Gubitosi | mgubitosi@udesa.edu.ar 
 
### Adviser
<!-- PONER LO DE TRINI -->
 - Trinidad Monreal | tmonreal@udesa.edu.ar 

# Abstract
We developed and applied deep learning models to colorize black-and-white images, specifically using a DnCNN for noise reduction and a cGAN generator for colorization. Our study demonstrates that it is possible not only to convincingly restore colors but also to improve the visual quality of historical images, surpassing the limitations of their time. Despite certain limitations related to generalization in varied backgrounds and the quality of our own dataset images, the models showed significant ability to produce high-quality images.

# Motivation
The intersection of memory and technological innovation drives our project, where we strive to keep precious moments alive. As technology has evolved, from canvases to photographs, many memories have been relegated to grayscale due to the limitations of the era, leaving the original colors forgotten. The goal of this work is to revive the colors of our family images, bringing them back to life with modern technology. 

# Results
<p align="center">
  <img src="images/all_gan_pred.png" width="30%">
  <img src="images/all_gan_pred_2.png" width="30%">
  <img src="images/reales.png" width="24%">
</p>

# Architecture
![Model Architecture](images/model_architecture.png)

# Installation
```bash
git clone git@github.com/AntonioTepsich/Final-Project-ML
cd Final_Project_ML
pip install -r requirements.txt
```

The files: logs, runs and results must be created the first time running the code.

# Usage
### 1-Download the dataset from Kaggle
Enter your Kaggle Account and apiKey after executing this command:
```bash
python scripts/download_datasets.py
```
Example:
```bash
Your Kaggle username: XXXX
Your Kaggle Key: XXXXXXXXXXXXXXXXXX
```
If other dataset is wanted, search in the scripts folder.


### 2- Train Models
Specify the configurations of the models to run and execute this command:
```bash
./go.sh
```

### 3- TensorBoard

```bash
tensorboard --logdir runs
```
