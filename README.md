# SkinLesionClassifier

# Benign_vs_Malignant_Predictor

A Streamlit-based web application to detect and classify skin lesions as **Benign** or **Malignant** using PCA and SVM models.

## Features
- Upload an image of a skin lesion to predict its classification.
- Provides visual recommendations and actionable insights based on predictions.
- Explore data analytics through an interactive dashboard displaying dataset distribution, model accuracy, and confusion matrix.

---

## Getting Started

### Prerequisites
- Python 3.7 or higher
- Required Python libraries:
  - `numpy`
  - `matplotlib`
  - `Pillow`
  - `joblib`
  - `streamlit`
  - `pandas`
  - `seaborn`

Install the dependencies using the following command:

```bash
pip install -r requirements.txt

Clone the Repository
```bash
git clone https://github.com/your-username/Benign_vs_Malignant_Predictor.git
cd Benign_vs_Malignant_Predictor
## Usage
Start the Streamlit App:

```bash
streamlit run app.py
Navigate to the App: Open your browser and go to http://localhost:8501.

Choose an Option:

🔍 Image Prediction: Upload a skin lesion image to classify it as benign or malignant.
📊 Data Insights Dashboard: Analyze dataset distribution and visualize model performance.
Dataset
The dataset used for training and testing the model is available on Kaggle:
Skin Cancer: Malignant vs. Benign

Project Structure:

Benign_vs_Malignant_Predictor/
├── app.py                 # Main application file
├── svm_skin_cancer_model.pkl  # Pre-trained SVM model
├── pca_skin_cancer.pkl    # PCA model for dimensionality reduction
├── confusion_matrix.pkl   # Saved confusion matrix for visualization
├── svm_skin_cancer_accuracy.pkl  # Model accuracy metric
├── train/                 # Folder containing training images
│   ├── benign/
│   └── malignant/
├── test/                  # Folder containing testing images
│   ├── benign/
│   └── malignant/
└── requirements.txt       # Required Python packages

Model Description:

PCA: Principal Component Analysis is used to reduce the dimensionality of images for efficient processing.
SVM: Support Vector Machine is utilized for classification of skin lesions.

How It Works
Image Prediction:
The uploaded image is preprocessed and normalized.
Dimensionality reduction is applied using PCA.
The SVM model predicts the image as either Benign or Malignant.
Displays results with additional recommendations.
Data Insights Dashboard:

Visualizes the training and testing dataset distributions.
Displays model accuracy and confusion matrix.
