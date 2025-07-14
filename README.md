
# Human Activity Recognition using Random Forest

This project implements a **Human Activity Recognition (HAR)** system using a **Random Forest Classifier** trained on the **UCI HAR Dataset**. It identifies six types of human activities based on smartphone sensor data.

---

## 📁 Repository Structure

```
Human-Activity-Recognition-RF/
│
├── Code/
│    ├── human_activity_recognition.ipynb
│    ├── human_activity_recognition.py 
├── data/
│    ├── features.txt
│    ├── X_train.txt
│    ├── y_train.txt
│    ├── X_test.txt
│    ├── y_test.txt   
├── README.md                        
├── requirements.txt                  
```

- **data/**: Contains all necessary dataset files from the UCI HAR Dataset.
- **human_activity_recognition.py**: Complete implementation including:
  - Data loading
  - Preprocessing
  - Feature selection (top 100 features using Random Forest importance)
  - Hyperparameter tuning with GridSearchCV
  - Model evaluation (Classification Report & Confusion Matrix)
- **requirements.txt**: Python libraries needed to run the project.
- **README.md**: Project overview, usage instructions, and structure.

---

## 📦 Dataset

- Dataset Source: [UCI HAR Dataset](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones)
- Activities Recognized:
  - WALKING
  - WALKING_UPSTAIRS
  - WALKING_DOWNSTAIRS
  - SITTING
  - STANDING
  - LAYING

---

## 🚀 How to Run

1. Clone or download this repository.
2. Place all dataset files inside the `data/` directory.
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the main script:
   ```bash
   python human_activity_recognition.py
   ```

---

## ✅ Sample Output

### Top 100 Selected Features:
A printed list of top 100 features based on Random Forest feature importance.

### Classification Report:
```
              precision    recall  f1-score   support

         LAYING       1.00      1.00      1.00       537
        SITTING       0.89      0.82      0.86       491
       STANDING       0.85      0.91      0.88       532
        WALKING       0.85      0.96      0.91       496
WALKING_DOWNSTAIRS 0.97      0.82      0.89       420
WALKING_UPSTAIRS   0.85      0.86      0.86       471

    accuracy                           0.90      2947
   macro avg       0.90      0.90      0.90      2947
weighted avg       0.90      0.90      0.90      2947
```

### Confusion Matrix:
A heatmap will be displayed showing the confusion matrix of actual vs predicted activities.

---

## 🔧 Dependencies

```
numpy
pandas
matplotlib
seaborn
scikit-learn
```

Install them using:
```bash
pip install -r requirements.txt
```

---

## 📌 Author

- **Swapnil Dave**
- GitHub: https://github.com/swapnil625

---

> ⭐ **Feel free to fork, contribute, or raise issues!**
