# OCT Multiclass Classification

Multiclass classification of **Optical Coherence Tomography (OCT)** retinal images into four classes:
- CNV (Choroidal Neovascularization)
- DME (Diabetic Macular Edema)
- DRUSEN
- NORMAL

## Project Overview
This project implements deep learning models for OCT image classification.  
It includes:
- Training with **ResNet50** baseline (extendable to other architectures such as EfficientNet, ConvNeXt, ViT).
- Metrics logging with **MLflow**.
- Model interpretability with **Grad-CAM**.
- Loss surface visualization.
- Final evaluation on the test dataset.

## Results
| Model     | Accuracy | F1 Macro | F1 Weighted | Training Time |
|-----------|----------|----------|-------------|---------------|
| ResNet50  | ~0.99    | ~0.99    | ~0.99       | ~87 min       |

## Repository Structure
oct-multiclass-classification/
├── Practice_CNN.ipynb # Binary classification (prototype)
├── Practice_full.ipynb # Multiclass classification (final version)
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE

## Installation
```bash
git clone https://github.com/YOUR_USERNAME/oct-multiclass-classification.git
cd oct-multiclass-classification
pip install -r requirements.txt

## Usage
Run the notebooks step by step:
```bash
jupyter notebook Practice_full.ipynb

## For the initial binary classification prototype:
```bash
jupyter notebook Practice_CNN.ipynb

## License
This project is licensed under the MIT License

## Topics
deep-learning pytorch computer-vision medical-imaging oct classification cnn grad-cam mlflow