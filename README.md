# Task Extractor from Unannotated Texts using NLP

## 📌 Overview
This project automatically extracts **task-related sentences** from raw, unannotated text using **Natural Language Processing (NLP)** techniques.  
It identifies sentences that indicate obligations, deadlines, or actions (e.g., *"You must submit the report by tomorrow"*) and extracts key entities and deadlines.

## ⚙️ Features
- Sentence tokenization and preprocessing (stopword removal, punctuation cleanup)
- Identification of task-related sentences using pattern-based matching
- Extraction of entities (e.g., person or subject) and deadlines
- Built purely using **Python + NLTK**

## 🧩 Project Workflow
1. **Preprocessing:**  
   - Split text into sentences  
   - Clean sentences and remove stopwords  
   - Tokenize each sentence

2. **Task Detection:**  
   - Uses regular expressions to detect obligation words like “must”, “should”, or “have to”  
   - Detects deadline-related terms such as “by 5pm”, “today”, “tomorrow”, etc.

3. **Information Extraction:**  
   - Extracts entities (proper nouns or pronouns)  
   - Identifies deadlines or time-related expressions in sentences

4. **Output:**  
   Returns a structured list of detected task sentences along with associated entities and deadlines.
   Example:
    Task 1:
    Description: John has to deliver a package by 9pm.
    Entity: John
    Deadline: by 9pm
    ---
    Task 2:
    Description: Rahul should clean the room by 5 pm today.
    Entity: Rahul
    Deadline: by 5 pm
    ---

## 🧰 Technologies Used
- **Python 3**
- **NLTK (Natural Language Toolkit)**
- **Regex (re)**
- **NumPy**

## 📦 Installation

To set up the environment and run the project, follow these steps:

```bash
# Clone the repository
git clone https://github.com/AjayG1026/Extracting-Tasks-from-Unannotated-Text-using-NLP.git

# Navigate into the project folder

# Install required dependencies
pip install -r requirements.txt
```

Once installed, you can open and run the Jupyter notebook or use the functions directly in a Python script.

## 📁 File Structure

```
├── main.ipynb          # Main notebook containing all preprocessing, detection, and extraction code
├── README.md           # Project documentation (you are reading this file)
├── requirements.txt    # Python dependencies
```


