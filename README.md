
This project implements a Deep Learning model to predict whether a bank customer is likely to leave (churn) based on their demographics and financial behavior. It includes a trained Artificial Neural Network (ANN), data preprocessing pipelines, and an interactive web interface built with Streamlit.

## 📁 Repository Structure

* `app.py`: The Streamlit web application script.
* `model.h5`: Trained Keras/TensorFlow neural network model.
* `experiments.ipynb`: Jupyter notebook containing data exploration, feature engineering, and model training.
* `prediction.ipynb`: Notebook for testing the model on new data.
* `label_encoder_gender.pkl` & `onehot_encoder_geo.pkl`: Pickled preprocessing objects to ensure consistent data transformation.
* `Churn_Modelling.csv`: The dataset used for training and testing.
* `requirements.txt`: List of Python dependencies.

---

## 🚀 Getting Started

### Prerequisites
Ensure you have Python 3.8+ installed. You can install the necessary dependencies using pip:

```bash
pip install -r requirements.txt
```

### Running the Web App
To launch the interactive prediction dashboard locally, run:

```bash
streamlit run app.py
```

---

## 🧠 Model & Preprocessing

The project uses an **Artificial Neural Network (ANN)** to classify customers. Key preprocessing steps included:

1.  **Categorical Encoding**: 
    * `Gender` was encoded using a Label Encoder.
    * `Geography` (France, Germany, Spain) was encoded using One-Hot Encoding to avoid ordinal bias.
2.  **Feature Scaling**: Input features were scaled to ensure the neural network converges efficiently.
3.  **Deployment**: The final model is exported as an `h5` file for real-time inference in the Streamlit app.

---

## 🛠️ Built With

* **TensorFlow/Keras** - For building and training the Deep Learning model.
* **Streamlit** - For the front-end web interface.
* **Scikit-Learn** - For data preprocessing and encoders.
* **Pandas & NumPy** - For data manipulation.

---

## 📈 Future Improvements
* Implement SMOTE to handle class imbalance in the churn dataset.
* Add Hyperparameter tuning using Keras Tuner.
* Deploy the app to Streamlit Cloud or AWS.

---

**Author:** [akku-0908](https://github.com/akku-0908)
