#🧠 U-Net–Assisted Spatial Feature Refinement for Interpretable Brain Tumor MRI Classification Using VGG-11 Transfer Learning
📌 Overview
This repository presents a deep learning–based framework for multi-class brain tumor MRI classification using VGG-11 transfer learning enhanced with spatial feature refinement. The approach improves class-discriminative localization by emphasizing informative convolutional feature maps prior to classification, leading to strong predictive performance and improved interpretability.
The model is evaluated on four classes: glioma, meningioma, pituitary tumor, and no tumor.
🎯 Key Highlights
Transfer learning using VGG-11 pre-trained on ImageNet
Spatial refinement of intermediate convolutional feature maps
End-to-end classification without external annotations
Strong and balanced performance across all tumor classes
Research-oriented yet beginner-friendly implementation
🧠 Model Architecture






4
Pre-trained VGG-11 convolutional layers extract hierarchical spatial features
Intermediate feature maps are refined to emphasize tumor-relevant regions
Refined representations are passed to fully connected layers for classification
📊 Results & Performance
Overall Accuracy: 98.17%
Classification Report
Class	Precision	Recall	F1-score
Glioma	0.9966	0.9767	0.9865
Meningioma	0.9671	0.9608	0.9639
No Tumor	0.9829	0.9951	0.9890
Pituitary	0.9802	0.9900	0.9851
🗂 Project Structure
├── notebooks/
│   └── brain-tumor-mri-vgg11-unet-feature-refinement.ipynb
├── src/                # (optional) modularized components
├── assets/             # figures, plots, diagrams
├── docs/               # extended documentation
├── data/               # dataset (excluded from repo)
├── models/             # trained weights (not included)
├── reports/            # metrics and evaluation outputs
├── requirements.txt
├── .gitignore
└── README.md
📦 Dataset
The dataset is sourced from a publicly available Brain Tumor MRI Dataset.
⚠️ Note:
The dataset is not included in this repository due to size and licensing constraints.
Please download it separately and place it in the data/ directory.
⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/<your-username>/unet-assisted-spatial-feature-refinement-vgg11-mri.git
cd unet-assisted-spatial-feature-refinement-vgg11-mri
2️⃣ Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
3️⃣ Install dependencies
pip install -r requirements.txt
▶️ How to Run
Open the Jupyter notebook:
notebooks/brain-tumor-mri-vgg11-unet-feature-refinement.ipynb
Execute cells sequentially:
Dataset loading
Model initialization
Training
Evaluation
🔍 Interpretability
The spatial refinement mechanism enhances interpretability by strengthening tumor-relevant feature activations in intermediate convolutional layers, allowing clearer differentiation between tumor and non-tumor regions during classification.
🧪 Reproducibility
Fixed random seeds for training consistency
Standardized preprocessing pipeline
Clear dependency management via requirements.txt
📈 Future Improvements
Modular refactor into standalone Python scripts
Grad-CAM–based visualization for enhanced explainability
Cross-dataset generalization evaluation
Lightweight deployment (ONNX / TorchScript)
📜 License
This project is released under the MIT License.
🙌 Acknowledgements
PyTorch & TorchVision
Open-source MRI datasets
Research community contributions in medical imaging
