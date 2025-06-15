Animal Skin Disease Detection Using Machine Learning
Project Overview
This project is focused on detecting skin diseases in animals such as dogs, cats, and cows using images and machine learning techniques. It uses MobileNetV2 for feature extraction and traditional ML models for classification. The final output includes a simple Gradio UI where users can upload an image and get an instant disease prediction.

---

Models Used

•	Feature Extractor: MobileNetV2 (pre-trained on ImageNet)
•	Classifiers
o	Random Forest
o	Logistic Regression
o	Support Vector Machine (SVM)
o	Additional Scikit-learn models (can be tested)

---

Dataset Structure
The project uses 3 separate datasets:
•	Dog Dataset
•	Cat Dataset
•	Cow Dataset
Each dataset includes:
/train/
    /Healthy/
    /Diseased/
/test/
    /Healthy/
    /Diseased/
There is also an Excel file for the dog dataset with binary columns representing multiple conditions:
•	bacteriadermatosis_dog
•	flea_allergy
•	fungalinfection_dog
•	healthy
•	ringworm
•	scabies, etc.

---

Workflow
1.	Preprocess and load all images
2.	Extract features using MobileNetV2
3.	Train classifiers using extracted features
4.	Evaluate models (Accuracy, Precision, Recall)
5.	Save the best performing model and label encoder
6.	Build a Gradio UI for predictions

---

Gradio UI Functionality
•	Upload animal skin image
•	Click "Submit"
•	Get prediction: e.g., Healthy, Scabies, Fungal Infection, etc.

---

How to Run the Project
pip install -r requirements.txt
# Run the Jupyter notebook in Google Colab or Jupyter Lab
To launch the Gradio UI:
interface.launch()

---

Requirements
•	Python 3.x
•	TensorFlow / Keras
•	Scikit-learn
•	Gradio
•	Pandas / NumPy
•	OpenCV (optional)

---

Author
Sania Kaleem
MS Data Science (In Progress)
GitHub: github.com/saniakaleem


