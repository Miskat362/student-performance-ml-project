# End-to-End Student Performance Prediction Project 🎓

This repository contains a complete end-to-end machine learning project designed to predict student academic performance. The entire pipeline, from data ingestion and exploratory data analysis (EDA) to model training and deployment via a simple web application, is included.

---

### ✨ Key Features

- **Modular & Reproducible Pipeline:** The project is structured with a clear, modular pipeline in `src/pipeline` for training and prediction.
- **Experimentation Ready:** Jupyter notebooks are provided for detailed Exploratory Data Analysis (EDA) and model training experiments.
- **Web Application:** A simple Flask application (`app.py`) is included to demonstrate model inference through a user-friendly web interface.
- **Best Practices:** Incorporates logging, exception handling, and a clear project structure for maintainability and scalability.

### 🛠️ Tech Stack

- **Backend:** Python
- **ML Libraries:** Scikit-learn, CatBoost, Pandas, NumPy
- **Web Framework:** Flask
- **Experimentation:** Jupyter Notebook

---

### 🚀 Getting Started

Follow these steps to set up and run the project locally.

#### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/ml-project.git
cd ml-project
```

#### 2. Create a Virtual Environment and Install Dependencies

It is highly recommended to use a virtual environment.

**For Windows:**
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

**For macOS/Linux:**
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

---

### 📈 Usage

#### 1. Run the Training Pipeline

To train the model from scratch, run the training pipeline script. This will perform data ingestion, transformation, and model training, saving the resulting artifacts in the `artifacts/` directory.

```bash
python src/pipeline/train_pipeline.py
```

#### 2. Run the Web Application for Predictions

Once the model is trained, you can start the Flask web application to perform live predictions.

```bash
python app.py
```

Navigate to `http://127.0.0.1:5000` in your web browser. You will see a form where you can input student data and get a predicted performance score.

---

### 📂 Project Structure

```
ml-project/
├── artifacts/
│   ├── data.csv
│   ├── preprocessor.pkl
│   ├── model.pkl
│   ├── raw.csv
│   ├── test.csv
│   └── train.csv
├── catboost_info/
├── notebooks/
│   ├── EDA_student_performance.ipynb
│   └── Model_training.ipynb
├── src/
│   ├── __init__.py
│   ├── components/
│   │   ├── __init__.py
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   ├── pipeline/
│   │   ├── __init__.py
│   │   ├── predict_pipeline.py
│   │   └── train_pipeline.py
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
├── templates/
│   ├── home.html
│   └── index.html
├── app.py
├── requirements.txt
└── README.md
```

---

### 📓 Notebooks

The `notebooks/` directory contains two key Jupyter notebooks:
- **`EDA_student_performance.ipynb`**: For exploratory data analysis, visualization, and understanding the dataset.
- **`Model_training.ipynb`**: An experimental notebook for iterating on model training, hyperparameter tuning, and evaluation.

---

### 🤝 Contributing

Contributions are welcome! If you have suggestions for improvements, please open an issue or submit a pull request.

---

## 🌟 Connect & Collaborate

**👤 Author:** [ Miskat Ahmmed ]  
**👥 Connect:** [LinkedIn](https://www.linkedin.com/in/miskat-ahmmed)

---