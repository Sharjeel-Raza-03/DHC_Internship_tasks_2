# 📰 News Topic Classification using BERT

## 📌 Project Overview

This project is part of the **DevelopersHub Corporation AI/ML Engineering Internship (Advanced Task 1)**.

The objective is to build a **News Topic Classification** system using a fine-tuned **BERT (`bert-base-uncased`)** transformer model. The model classifies news articles into four categories:

- 🌍 World
- 🏅 Sports
- 💼 Business
- 🔬 Sci/Tech

This project demonstrates the use of **Transfer Learning with Transformers** for real-world Natural Language Processing (NLP) classification tasks.

---

## 🎯 Objective

- Fine-tune a pre-trained BERT model on the AG News dataset.
- Classify news articles into four categories.
- Evaluate model performance using **Accuracy** and **F1-Score**.
- Generate predictions for unseen test data.
- Visualize performance using a confusion matrix.

---

## 📊 Dataset Information

**Dataset:** AG News Classification Dataset

### Dataset Statistics

| Split | Samples |
|--------|---------|
| Training | 120,000 |
| Testing | 7,600 |

### Classes

| Label | Category |
|-------|----------|
| 1 | 🌍 World |
| 2 | 🏅 Sports |
| 3 | 💼 Business |
| 4 | 🔬 Sci/Tech |

Each news sample contains:

- **Title**
- **Description**
- **Label**

---

## 🛠️ Technologies Used

- Python 🐍
- Hugging Face Transformers 🤗
- PyTorch 🔥
- Scikit-learn 📊
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 🧠 Model Details

| Parameter | Value |
|-----------|-------|
| Model | `bert-base-uncased` |
| Task | Text Classification |
| Approach | Transfer Learning (Fine-tuning) |
| Maximum Sequence Length | 128 Tokens |
| Loss Function | Cross-Entropy Loss |
| Optimizer | AdamW |
| Framework | Hugging Face Trainer API |

---

## ⚙️ Project Workflow

### 1. Data Preprocessing

- Loaded the AG News dataset.
- Cleaned labels and removed invalid rows.
- Combined the **Title** and **Description** into a single text field.

### 2. Tokenization

- Used the BERT tokenizer.
- Applied truncation and padding.
- Converted text into **Input IDs** and **Attention Masks**.

### 3. Model Training

- Fine-tuned the pre-trained BERT model.
- Used the Hugging Face Trainer API.
- Validated the model during training.

### 4. Model Evaluation

Performance was evaluated using:

- Accuracy Score
- Weighted F1-Score
- Confusion Matrix

---

## 📈 Results

The fine-tuned BERT model achieved strong performance on the AG News dataset.

| Metric | Performance |
|--------|-------------|
| ✅ Accuracy | **~90%+** *(varies depending on training configuration)* |
| ✅ Weighted F1-Score | **High performance across all classes** |

---

## 🚀 Key Features

- Fine-tuned BERT (`bert-base-uncased`)
- Transfer Learning for NLP
- Four-class News Topic Classification
- Automated training using Hugging Face Trainer API
- Performance evaluation with Accuracy and F1-Score
- Confusion Matrix visualization
- Supports prediction on unseen news articles

---

## 📂 Project Structure

```text
News-Topic-Classification-BERT/
│
├── data/
│   ├── train.csv
│   └── test.csv
│
├── notebook.ipynb
├── bert_news_classifier/
├── saved_model/
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 📌 Future Improvements

- Hyperparameter tuning
- Early stopping
- Learning rate scheduling
- Deploy using FastAPI or Flask
- Build a Streamlit web application
- Experiment with RoBERTa and DistilBERT

---

## 👨‍💻 Author

**Sharjeel Raza**

AI/ML Engineering Internship — DevelopersHub Corporation

---

## ⭐ Acknowledgements

- Hugging Face Transformers
- PyTorch
- Scikit-learn
- AG News Dataset
- DevelopersHub Corporation
