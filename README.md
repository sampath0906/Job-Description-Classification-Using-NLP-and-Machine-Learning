# Job Description Classification Using NLP and Machine Learning

## 📌 Project Overview

This project focuses on automatically classifying job descriptions into their respective job categories using Natural Language Processing (NLP) and Machine Learning techniques.

Job descriptions contain important information about job responsibilities, required skills, qualifications, and experience. Manually categorizing large volumes of job descriptions can be time-consuming and inefficient.

To overcome this challenge, this project develops a machine learning-based classification system that analyzes textual job descriptions and predicts their corresponding job categories.

The trained model is also deployed using **Gradio**, allowing users to enter a job description and receive a predicted category.

---

## 🎯 Business Objective

- Automate the classification of job descriptions.
- Identify important keywords and textual patterns associated with different job categories.
- Reduce manual effort in organizing job-related information.
- Compare multiple machine learning algorithms to identify the best-performing model.
- Build an interactive application for predicting job categories.

---

## 📂 Dataset

The project uses a job description dataset containing textual descriptions and their corresponding job category labels.

**Dataset Features:**

| Column | Description |
|---|---|
| `jobdescription` | Contains the textual job description |
| `label` | Represents the corresponding job category |

**Target Variable:** `label`

**Input Feature:** `jobdescription`

---

## 🔄 Project Workflow

The project follows an end-to-end Data Science workflow.

### 1. Data Collection
- Imported the job description dataset.
- Loaded the dataset using Pandas.

### 2. Data Understanding
- Examined the dataset structure and dimensions.
- Analyzed job category distribution.
- Checked missing values and duplicate records.
- Analyzed the average text length across job categories.

### 3. Text Preprocessing
- Converted text into lowercase.
- Removed HTML tags and URLs.
- Removed special characters and unnecessary spaces.
- Tokenized the text.
- Removed English stopwords.
- Applied lemmatization using NLTK.

### 4. Train-Test Split
- Separated input features and target labels.
- Divided the dataset into training and testing sets.
- Used stratified sampling to maintain class distribution.

### 5. Feature Engineering
- Applied TF-IDF (Term Frequency-Inverse Document Frequency) vectorization.
- Converted textual job descriptions into numerical feature representations.

### 6. Model Building

Implemented and trained the following classification algorithms:

- Multinomial Naive Bayes
- Logistic Regression
- Linear Support Vector Classifier (Linear SVM)

### 7. Model Evaluation
- Evaluated the trained models using accuracy score.
- Compared model performance.
- Selected Linear SVM for the prediction application.

### 8. Model Deployment
- Saved the trained TF-IDF vectorizer and Linear SVM model using Pickle.
- Developed an interactive application using Gradio.
- Enabled users to enter new job descriptions and obtain predicted job categories.

---

## 🛠️ Technologies and Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| NLTK | Natural Language Processing |
| Scikit-learn | Machine Learning algorithms |
| TF-IDF | Text feature extraction |
| Pickle | Model serialization |
| Gradio | Application deployment |
| Jupyter Notebook | Development environment |

---

## 🤖 Machine Learning Models

Three classification algorithms were implemented:

**1. Multinomial Naive Bayes**

A probabilistic classification algorithm commonly used for text classification tasks.

**2. Logistic Regression**

A supervised classification algorithm used to predict the probability of a job description belonging to a particular category.

**3. Linear Support Vector Classifier (Linear SVM)**

A classification algorithm that identifies an optimal decision boundary to distinguish between different job categories.

---

## 🚀 Installation and Execution

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/Job-Description-Classification.git
```

### Step 2: Navigate to the Project Directory

```bash
cd Job-Description-Classification
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the Jupyter Notebook

Open the notebook and execute the cells sequentially to understand the complete workflow.

### Step 5: Run the Gradio Application

If the deployment code is available in a separate `app.py` file:

```bash
python app.py
```

If deployment is implemented directly in the notebook, execute the Gradio launch cell.

---

## 💾 Saved Model Files

The project uses Pickle to save the trained components:

- `tfidf_vectorizer.pkl` – Saved TF-IDF vectorizer.
- `svm_model.pkl` – Saved Linear SVM classification model.

These files are used to transform new job descriptions and generate predictions without retraining the model.

---

## 💻 Application Features

- User-friendly Gradio interface.
- Accepts job descriptions as text input.
- Performs automatic text cleaning and preprocessing.
- Converts text into TF-IDF features.
- Predicts the corresponding job category.
- Displays the prediction interactively.

---

## 🔮 Future Enhancements

- Experiment with advanced NLP techniques and transformer-based models.
- Improve classification performance through hyperparameter tuning.
- Add additional job categories and training data.
- Display prediction confidence or class-wise probabilities where supported by the model.
- Deploy the application on Hugging Face Spaces or another cloud platform.

---

## 📌 Conclusion

This project demonstrates an end-to-end application of Natural Language Processing and Machine Learning for automated job description classification.

By combining text preprocessing, TF-IDF feature extraction, and machine learning algorithms, the system can identify patterns in job descriptions and predict their corresponding categories.

The integration of Pickle and Gradio makes the trained model accessible through an interactive application, demonstrating how machine learning solutions can be developed and deployed for practical use cases.

---

## 👨‍💻 Author

**K Sai Sampath**

B.Tech Graduate | Aspiring Data Analyst

**Skills:** Python | SQL | Statistics | Pandas | NumPy | Machine Learning | NLP | Power BI
