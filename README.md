# 🌿 Plant Species Classification using Traditional Machine Learning

*Achieved 92.06% test accuracy without using transfer learning or CNNs*

---

## 🚀 Overview

This project focuses on classifying plant species using handcrafted features and traditional machine learning techniques like Random Forests. It avoids transfer learning or deep CNNs to demonstrate the power of classical approaches in solving image classification problems.

---
## 📦 Dataset Used
This project utilizes the *Plant Type Datasets* from Kaggle.

🔗 [View on Kaggle](https://www.kaggle.com/datasets/yudhaislamisulistya/plants-type-datasets)  
  📁 Downloaded file: plants-type-datasets.zip (~1 GB)

---
## 🔧 Tech Stack

- *Frontend*: HTML, CSS, JavaScript
- *Backend*: Python (Streamlit)
- *ML Libraries*: scikit-learn, OpenCV, NumPy, Matplotlib
- *Model Trained*:Random Forest

---

## 🔍 Techniques Used

### 🎨 Feature Extraction

1. *Color Features*
   - RGB Histogram
   - HSV Histogram
   - LAB Histogram  
   (Each with 512 bins)

2. *Texture Features*
   - Local Binary Patterns (LBP)
   - Statistical descriptors: Mean, Std Deviation

3. *Shape Features*
   - Contour-based features: Area, Perimeter, Circularity

4. *HOG Features*
   - Histogram of Oriented Gradients  
   (3,780 dimensions)

---

## 🧠 ML Pipeline

- *Preprocessing*:
  - Handling missing values using SimpleImputer
  - Feature scaling using StandardScaler

- *Model*:  
  - RandomForestClassifier with n_estimators=200, max_depth=15

---

## 📊 Results

| Metric            | Score     |
|-------------------|-----------|
| *Test Accuracy* | 92.06%    |
| Precision (Avg)   | 92.1%     |
| Recall (Avg)      | 91.8%     |

---

## 🌐 Frontend + Backend Integration

created a fully *dynamic frontend* using:
- *📊 Streamlit Frontend*: Built for faster local development and testing. It allows image uploads, live predictions, and visualization of feature maps or probabilities.

---

## 📁 Repository Structure


├── feature_extraction.py        # Extracts color, texture, shape, HOG features
├── model_training.py            # Trains and saves the RandomForestClassifier
├── prediction.py                # Loads model and performs predictions
├── app.py                       # Flask backend to serve predictions
├── streamlit_app.py             # For real-time visualization/testing
├── static/
│   └── styles.css               # CSS for frontend
├── templates/
│   └── index.html               # HTML + JS interface for image upload
├── dataset/
│   ├── train/                   # Training images
│   ├── test/                    # Testing images
│   └── labels.csv               # Label metadata
├── model/
│   └── classifier.pkl           # Trained RandomForest model
└── README.md


---

## ▶ How to Run

## 1. Clone the repository
```bash
git clone https://github.com/Gargi-Goyal/Project_on_PlantSpecies_ClassificationUsingML.git
cd Project_on_PlantSpecies_ClassificationUsingML

##2.Install dependencies
pip install -r requirements.txt

##3.Run the Streamlit app
streamlit run Frontend/streamlit_app/app.py

---

## 🙋 Author

*Gargi Goyal*  
Linkedin:[🔗 GargiGoyal-LinkedIn](https://www.linkedin.com/in/gargi-goyal-047888249/)
EmailId:Gargigoyl2712dec@gmail.com

---

## 🤝 Contributions

Contributions, issues, and feature requests are welcome!  
Feel free to fork this repository and submit a pull request.

---

## ⭐ If You Found This Helpful

Please consider giving this repo a ⭐  
It motivates me to grow and share more helpful and beginner-friendly projects like this!
