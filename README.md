# Phishing Website Detection by Machine Learning Techniques

## Objective
A phishing website is a common social engineering method that mimics trusted uniform resource locators (URLs) and webpages.  
The objective of this project is to train **machine learning models** and **deep neural networks** on a custom dataset to predict phishing websites.  

Both **phishing** and **benign** URLs are collected to form the dataset, from which URL and content-based features are extracted.  
The performance of each model is measured and compared.

---

## Data Collection
- **Phishing URLs**:  
  Collected from [PhishTank](https://www.phishtank.com/developer_info.php), an open-source service that updates hourly.  
  → 5,000 random phishing URLs are selected.

- **Legitimate URLs**:  
  Collected from [University of New Brunswick Dataset](https://www.unb.ca/cic/datasets/url-2016.html).  
  → 5,000 random benign URLs are selected.  

Both datasets are uploaded to the **`DataFiles`** folder of this repository.

---

## Feature Extraction
A total of **17 features** are extracted from the 10,000 URLs.  
The features fall into the following categories:

- **Address Bar Based Features** → 9 features  
- **Domain Based Features** → 4 features  
- **HTML & JavaScript Based Features** → 4 features  

Details of feature extraction can be found in **`URL Feature Extraction.ipynb`**.  
The features are referenced from the [UCI Phishing Websites Dataset](https://archive.ics.uci.edu/ml/datasets/Phishing+Websites).

All extracted features are stored in **`5.urldata.csv`** inside the `DataFiles` folder.

---

## Models & Training
The dataset is split into **80-20**:
- **Training set**: 8,000 samples  
- **Testing set**: 2,000 samples  

This is a **supervised machine learning classification problem**, where input URLs are classified as:  
- **1 → Phishing**  
- **0 → Legitimate**  

The following models are trained and evaluated:

- Decision Tree  
- Random Forest  
- Multilayer Perceptrons (MLP)  
- XGBoost  
- Autoencoder Neural Network  
- Support Vector Machines (SVM)  

Elaborate details of training and evaluation are in **`Phishing Website Detection_Models & Training.ipynb`**.

---

## Presentation
- 🎥 [Video Presentation](https://youtu.be/I1refTZp-pg)  
- 📑 Slide Deck: **Phishing Website Detection by Machine Learning Techniques Presentation.pdf**

---

## End Results
- Among all models, the **XGBoost Classifier** achieved the highest performance: **86.4% accuracy**.  
- The trained model is saved as **`XGBoostClassifier.pickle.dat`**.

---

## Next Steps
Future extensions of this project include:
- Developing a **browser extension** to classify URLs in real-time.  
- Creating a **GUI application** for URL classification.  

Further updates will be shared in this repository.

---
