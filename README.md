# Plant Leaf Image Classification Project
![Uploading image.png…]()


## Project Description
This project aims to classify plant leaf conditions into three categories:
- healthy
- stressed
- diseased

The main model used is a Custom CNN based on Sequential architecture with Conv2D and Pooling layers.

---

## Dataset
The dataset consists of plant leaf images that have been categorized into three main classes:
- healthy
- stressed
- diseased

---

## Model Architecture
The model uses:
- Conv2D
- MaxPooling2D
- BatchNormalization
- GlobalAveragePooling
- Dense
- Dropout

---

## Project Stages

### 1. Preprocessing
- Resize images to 224x224
- Normalize pixel values to the range of 0–1

### 2. Training
- Optimizer: Adam
- Loss Function: Categorical Crossentropy (with label smoothing)
- Epochs: 10

### 3. Evaluation
The model evaluation uses:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 4. Inference
The trained model is tested using new images to evaluate its generalization capability.

---

## Results
The Custom CNN model achieved strong performance with high accuracy and stable training results.

---

## Folder Structure
```plaintext
submission/
├── tfjs_model/
├── tflite/
├── saved_model/
├── notebook.ipynb
├── README.md
├── requirements.txt
```

---  
## How to Run

Install the dependencies:

- pip install -r requirements.txt

Run the notebook:

- jupyter notebook notebook.ipynb

---  
## Deployment

The trained model was converted into:

SavedModel
TensorFlow Lite
TensorFlow.js

---  
## Conclusion

The model successfully classifies plant leaf conditions and can be further implemented for real-world agricultural applications.
