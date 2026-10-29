# Student Feedback Sentiment Analysis

**An NLP and Machine Learning Application for Automated Student Feedback Analysis**

<p align="center">
  A Python-based web application that analyzes student feedback using Natural Language Processing and Machine Learning.
</p>

---

## Overview

The **Student Feedback Sentiment Analysis** project is designed to process textual feedback and predict the sentiment expressed by students. It combines text preprocessing, Term Frequency–Inverse Document Frequency (TF-IDF) feature extraction, and a trained Logistic Regression classifier to transform unstructured feedback into meaningful sentiment predictions.

The application uses Flask to provide a web interface through which users can submit feedback and view the model's prediction.

## Key Features

- **Automated Sentiment Classification:** Predicts sentiment from submitted feedback.
- **Text Preprocessing:** Prepares textual input for machine learning.
- **TF-IDF Feature Extraction:** Converts text into numerical representations.
- **Machine Learning Model:** Uses a trained Logistic Regression classifier.
- **Web-Based Interface:** Provides an accessible interface powered by Flask.
- **Reusable Model Artifacts:** Loads the trained model and vectorizer without requiring model training on every application launch.

## Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Python |
| Web Framework | Flask |
| Machine Learning | Scikit-learn |
| Natural Language Processing | Text preprocessing |
| Feature Extraction | TF-IDF |
| Classification Algorithm | Logistic Regression |
| Data Handling | Pandas |
| Frontend | HTML, CSS, JavaScript (as implemented) |
| Dataset | Excel |

## System Workflow

```text
Student Feedback
       |
       v
Text Preprocessing
       |
       v
TF-IDF Feature Extraction
       |
       v
Trained Logistic Regression Model
       |
       v
Sentiment Prediction
       |
       v
Display Result in Web Interface
```

## Project Structure

```text
Sentiment_Analysis_Project/
├── app.py
├── preprocessing.py
├── train_model.py
├── requirements.txt
├── Sentiment_Analysis__final.ipynb
├── Aditya_University_Sentiment_Final_Dataset.xlsx
├── sentiment_model.pkl
├── sentiment_model_metadata.json
├── tfidf_vectorizer.pkl
├── templates/
├── static/
├── .gitignore
└── README.md
```

### Core Components

- **`app.py`** — Initializes the Flask application and handles feedback submissions and predictions.
- **`preprocessing.py`** — Provides text preprocessing functionality.
- **`train_model.py`** — Contains the model training workflow.
- **`Sentiment_Analysis__final.ipynb`** — Notebook for experimentation and analysis.
- **`sentiment_model.pkl`** — Serialized trained classification model.
- **`tfidf_vectorizer.pkl`** — Serialized fitted TF-IDF vectorizer.
- **`sentiment_model_metadata.json`** — Stores model-related metadata.
- **`requirements.txt`** — Specifies the Python packages required by the project.
- **`templates/`** — Contains the application's HTML templates.
- **`static/`** — Contains static frontend assets.

## Getting Started

### Prerequisites

Install the following before running the project:

- Python 3
- Git
- A terminal or command prompt
- A web browser

### 1. Clone the Repository

```bash
git clone https://github.com/123lakshmi-majji/Sentiment-Analysis.git
cd Sentiment-Analysis
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

### 3. Activate the Environment

**Windows PowerShell**

```powershell
.\venv\Scripts\Activate.ps1
```

**Windows Command Prompt**

```bat
venv\Scripts\activate.bat
```

### 4. Install Dependencies

```bash
python -m pip install -r requirements.txt
```

### 5. Launch the Application

```bash
python app.py
```

Open the following address in your browser:

`http://127.0.0.1:5000`

> **Note:** The trained model and TF-IDF vectorizer files must be available in the locations expected by the application.

## Model Pipeline

The application follows a standard text-classification workflow:

1. **Input Collection:** Accepts textual student feedback.
2. **Preprocessing:** Applies the text-cleaning operations implemented in the project.
3. **Feature Representation:** Transforms the processed text into TF-IDF features.
4. **Classification:** Passes the feature vector to the trained Logistic Regression model.
5. **Result Presentation:** Displays the predicted sentiment through the web interface.

The preprocessing and feature extraction steps used during inference should remain consistent with those used during model training.

## Dataset

The project uses an Excel dataset named `Aditya_University_Sentiment_Final_Dataset.xlsx`.

The dataset supports the model development and evaluation workflow. Dataset size, input columns, target labels, class distribution, and evaluation results should be documented here after verification.

## Future Enhancements

- Evaluate additional classification algorithms and compare their performance.
- Improve generalization using a larger and more diverse feedback dataset.
- Add sentiment distribution charts and trend analysis.
- Support multilingual feedback.
- Develop a dashboard for summarizing student feedback.
- Deploy the application to a cloud hosting platform.
- Add automated testing and model-performance monitoring.

## Limitations

- Prediction quality depends on the dataset and model training process.
- Sarcasm, ambiguous expressions, spelling variations, and context-dependent language may affect predictions.
- The model's output should be treated as a prediction rather than a definitive interpretation of a student's opinion.

## Author

**Lakshmi Majji**

GitHub: [@123lakshmi-majji](https://github.com/123lakshmi-majji)

## License

No license has been specified yet. Add a license file if you intend to define how others may use, modify, or distribute this project.

---

*Developed as an academic project to explore Natural Language Processing, machine learning-based text classification, and web application development.*
