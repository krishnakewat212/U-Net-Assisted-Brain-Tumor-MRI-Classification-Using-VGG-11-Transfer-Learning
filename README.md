# U-Net–Assisted Spatial Feature Refinement for Interpretable Brain Tumor MRI Classification Using VGG-11 Transfer Learning

## Overview
This repository presents a deep learning–based framework for multi-class brain tumor MRI classification using VGG-11 transfer learning enhanced with spatial feature refinement. The approach improves class-discriminative localization by emphasizing informative convolutional feature maps prior to classification, leading to strong predictive performance and improved interpretability.
The model is evaluated on four classes: glioma, meningioma, pituitary tumor, and no tumor.

## Dataset
The dataset is sourced from a publicly available Brain Tumor MRI Dataset.
Note:
The dataset is not included in this repository due to size and licensing constraints.
Please download it separately and place it in the data/ directory.[https://github.com/<your-username>/unet-assisted-spatial-feature-refinement-vgg11-mri.git](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)

## Interpretability
The spatial refinement mechanism enhances interpretability by strengthening tumor-relevant feature activations in intermediate convolutional layers, allowing clearer differentiation between tumor and non-tumor regions during classification.
## Reproducibility
Fixed random seeds for training consistency
Standardized preprocessing pipeline
Clear dependency management via requirements.txt
## Future Improvements
Modular refactor into standalone Python scripts
Grad-CAM–based visualization for enhanced explainability
Cross-dataset generalization evaluation
Lightweight deployment (ONNX / TorchScript)
## License
This project is released under the MIT License.
## Acknowledgements
PyTorch & TorchVision
Open-source MRI datasets
Research community contributions in medical imaging

