# 🧠 Named Entity Recognition (NER)
This project focuses on Named Entity Recognition, a key task in NLP that involves identifying and classifying entities in text into predefined categories. The main objective of this project is to explore and compare different approaches to NER, ranging from traditional rule-based systems to modern machine learning techniques.

## 📌 Overview

This project demonstrates **Named Entity Recognition (NER)** using three different approaches:

* 🔤 Lexicon-Based Method (spaCy)
* 📏 Rule-Based Method (custom patterns + context rules)
* 🤖 Machine Learning-Based Method (Scikit-learn models) with different ML models with evatuations

NER is a Natural Language Processing (NLP) task that identifies and classifies entities such as:

* 👤 Person names
* 🏢 Organizations
* 🌍 Locations
* 📅 Dates
* 💰 Money values

---

## 📖 Example

**Input:**

```
Barack Obama was born in Hawaii and worked at the University of Chicago.
```

**Output:**

```
Barack → B-PER
Obama → I-PER
Hawaii → B-LOC
University → B-ORG
Chicago → B-LOC
```
---

## ⚙️ Project Workflow

![Workflow](https://github.com/UpekshaIndeewari/-NER_Project/blob/main/Workflow.png)

1. **Text Processing**

   * Sentence segmentation
   * Tokenization

2. **Feature Engineering**

   * Word shape (uppercase, lowercase)
   * Prefix/suffix
   * Context (previous & next words)

3. **Model Training**

   * Train ML models on CoNLL dataset

4. **Prediction**

   * Classify each token into entity labels

5. **Evaluation**

   * Accuracy, Precision, Recall, F1-score

---

## 🧪 Methods Implemented

### 1️⃣ Lexicon-Based NER (spaCy)

* Uses pre-trained NLP models
* Quick and easy to use
* Limited customization

---

### 2️⃣ Rule-Based NER

* Pattern-based (regex)
* Context-based rules
* Example:

  * `"Mr John"` → Person
  * `"Google Inc"` → Organization

---

### 3️⃣ Machine Learning-Based NER

Models used:

* Logistic Regression
* Random Forest
* Gradient Boosting
* Linear SVM
* Naive Bayes

---

## 📊 Model Performance

| Model               | Accuracy          |
| ------------------- | ----------------- |
| Logistic Regression | 95.93%            |
| Random Forest       | 95.08%            |
| Gradient Boosting   | 92.23%            |
| Linear SVM          | **96.75% (Best)** |
| Naive Bayes         | 92.60%            |

---

## 🧠 Key Features

* Custom **feature engineering**
* Multiple ML model comparison
* Entity highlighting visualization
* Interactive user input prediction
* Clean CoNLL dataset parsing

---

## 📁 Dataset

* Format: CoNLL-2003 style
* Structure:

```
Word POS Chunk Tag
```

Example:

```
Barack NNP B-NP B-PER
Obama NNP I-NP I-PER
```

---

## 🛠️ Installation

```bash
pip install spacy nltk scikit-learn matplotlib
python -m spacy download en_core_web_sm
```

---

## ▶️ How to Run

1. Open the notebook in Google Colab
2. Upload dataset (`test.txt`)
3. Run all cells
4. Enter your own sentence for prediction

---

## 🎯 Sample Prediction

```
Enter a sentence:
Elon Musk founded SpaceX in California.
```

**Output:**

```
Elon → B-PER  
Musk → I-PER  
SpaceX → B-ORG  
California → B-LOC  
```

---

## 📈 Visualization

* Entity highlighting using HTML
* Model comparison using bar charts

---

## 🚀 Future Improvements

* Add Deep Learning models (BERT / DistilBERT)
* Improve feature engineering
* Add CRF layer for sequence labeling
* Deploy as a web app (Streamlit / Flask)

---

## 🤝 Contributing

Contributions are welcome!
Feel free to fork the repo and submit a pull request.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 🙌 Acknowledgements

* CoNLL-2003 Dataset
* spaCy
* Scikit-learn
* Hugging Face Transformers

---
