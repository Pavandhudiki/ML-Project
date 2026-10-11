# 🎓 Student Placement Prediction Using Machine Learning

## 📌 Project Overview

This project uses **Machine Learning to predict student placement outcomes** based on academic performance and skill-related factors.

A **Decision Tree Classifier** is trained using a sample dataset of 30 students. The model learns patterns from the training data and predicts whether a student is likely to be placed or not placed based on selected features.

The project demonstrates the basic workflow of a Machine Learning classification problem using Python and Scikit-learn.

## 🎯 Objectives

- Understand the fundamentals of Machine Learning.
- Create and process a student dataset using Pandas.
- Select relevant features and a target variable.
- Split the dataset into training and testing sets.
- Train a Decision Tree Classification model.
- Evaluate model predictions using accuracy.
- Predict the placement outcome for a new student.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and DataFrame creation
- **Scikit-learn** — Model training, dataset splitting, and evaluation
- **Jupyter Notebook** — Development and experimentation

## 📊 Dataset Description

The project uses a sample dataset containing information about 30 students.

The following features are used to make predictions:

| Feature | Description |
|---|---|
| `CGPA` | Student's academic performance |
| `Skills` | Student's skills score |
| `Projects` | Number of projects completed |
| `Internships` | Number of internships completed |
| `Certifications` | Number of certifications |
| `DSA_Score` | Data Structures and Algorithms score |

**Target variable: `Placed`**

- `1` — Placed
- `0` — Not placed

The student's roll number and name are included in the original dataset but are not used as prediction features.

**Note:** The dataset is created directly in the notebook for demonstration purposes; it is not an external real-world placement dataset.

## ⚙️ Project Workflow

1. Import the required Python libraries.
2. Create a sample student dataset.
3. Convert the dataset into a Pandas DataFrame.
4. Select the input features (`X`).
5. Select the target variable (`y`).
6. Split the data into training and testing sets using `train_test_split`.
7. Create a `DecisionTreeClassifier`.
8. Train the model using `model.fit()`.
9. Predict outcomes for the test dataset.
10. Evaluate the model using `accuracy_score`.
11. Create a new student's input data.
12. Predict the new student's placement outcome.
13. Display the prediction as **Placed** or **Not Placed**.

## 🧠 Machine Learning Algorithm

### Decision Tree Classifier

A Decision Tree Classifier is a supervised Machine Learning algorithm used for classification tasks.

In this project, it learns from the training data using student features and their corresponding placement labels. It then predicts the placement category for unseen input records.

### Training and Testing

The dataset is divided using an 80:20 training-to-testing ratio:

- **Training data:** 80% — 24 students
- **Testing data:** 20% — 6 students

The `random_state=42` parameter is used to make the data split reproducible.

### Model Evaluation

The model's predictions are compared with the actual test labels using `accuracy_score`.

Accuracy is calculated as:

\[
\text{Accuracy} =
\frac{\text{Correct Predictions}}{\text{Total Predictions}}
\]

The actual accuracy should be obtained by running the notebook. Since the dataset is small and manually created, the measured accuracy should not be treated as evidence of real-world placement prediction performance.

## 🔍 Prediction for a New Student

The notebook tests the trained model with a new student whose details are:

| Feature | Value |
|---|---:|
| CGPA | 7.7 |
| Skills | 2 |
| Projects | 1 |
| Internships | 1 |
| Certifications | 2 |
| DSA Score | 30 |

The model predicts the student's placement category and displays one of the following:

- `Prediction: Placed`
- `Prediction: Not Placed`

The output depends on the trained model and the dataset.

## 📂 Project Structure

```text
Student-Placement-Prediction/
│
├── myprojectmodel.ipynb
└── README.md
```

## 🚀 How to Run the Project

### Prerequisites

Install Python and Jupyter Notebook, or use an environment such as Anaconda or Google Colab.

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
```

### Step 2: Navigate to the Project Folder

```bash
cd Student-Placement-Prediction
```

### Step 3: Install the Required Libraries

```bash
pip install pandas scikit-learn notebook
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Notebook

1. Open `myprojectmodel.ipynb`.
2. Run the cells in order, from top to bottom.
3. Observe the dataset, training and testing results, accuracy, and new-student prediction.

## 📈 Results

The project successfully demonstrates the workflow of building a classification model, from dataset preparation to making a prediction for a new student.

The notebook produces:
- Training and testing dataset sizes.
- Actual and predicted test labels.
- Model accuracy.
- A placement prediction for a new student.

Run the notebook to obtain the actual accuracy and prediction output.

## 🔮 Future Improvements

- Use a larger, real-world student placement dataset.
- Include additional relevant academic and professional features.
- Compare Decision Tree performance with other classification algorithms.
- Evaluate the model using precision, recall, F1-score, and a confusion matrix.
- Build a simple web application to accept student details and display predictions.
- Validate the model on independent data before considering real-world use.

## ⚠️ Disclaimer

This project is intended for educational purposes and Machine Learning practice. The sample dataset is small and manually created. Predictions are experimental and should not be used to make actual student recruitment or placement decisions.

## 👨‍💻 Author

**Your Name**

GitHub: [Your GitHub Profile](https://github.com/your-username)

## 📄 License

This project is available for educational and learning purposes. Add a license file if you want to specify the terms under which others may use, modify, or distribute the project.

