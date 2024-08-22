# Image-colorization-and-denoising
with Pix2Pix and DnCNN

### Authors
This repository was made by:
 - Antonio Tepsich | atepsich@udesa.edu.ar 
 - Maximo Gubitosi | mgubitosi@udesa.edu.ar 
 
### Adviser
<!-- PONER LO DE TRINI -->
 - Trinidad Monreal | tmonreal@udesa.edu.ar 

### Abstract
We developed and applied deep learning models to colorize black-and-white images, specifically using a DnCNN for noise reduction and a cGAN generator for colorization. Our study demonstrates that it is possible not only to convincingly restore colors but also to improve the visual quality of historical images, surpassing the limitations of their time. Despite certain limitations related to generalization in varied backgrounds and the quality of our own dataset images, the models showed significant ability to produce high-quality images.

### Motivation
The intersection of memory and technological innovation drives our project, where we strive to keep precious moments alive. As technology has evolved, from canvases to photographs, many memories have been relegated to grayscale due to the limitations of the era, leaving the original colors forgotten. The goal of this work is to revive the colors of our family images, bringing them back to life with modern technology. 



# Installation
```bash
git clone git@github.com/AntonioTepsich/Final-Project-ML
cd Final_Project_ML
pip install -r requirements.txt
```

Ademas deben crear los archivos logs, runs, results en caso de ser la primera vez que corra.

# Usage
### 1-Descargar el Dataset de Kaggle
Deberas ingresar tu usuario y apiKey de Kaggle luego de ejecutar el siguiente comando:
```bash
python scripts/download_datasets.py
```
Ejemplo:
```bash
Your Kaggle username: XXXX
Your Kaggle Key: XXXXXXXXXXXXXXXXXX
```
En caso de querer otro dataset, buscar en la carpeta scrips



### 2- Entrenar modelos
Especificar las configuraciones de los modelos a entrenar y correr el siguiente comando:
```bash
./go.sh
```

### 3- TensorBoard

```bash
tensorboard --logdir runs
```
