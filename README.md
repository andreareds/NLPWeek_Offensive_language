# NLP Week -  Offensive language in Social Media
Offensive language in social media

This project is based on SemEval-2019 Task 6: Identifying and Categorizing
Offensive Language in Social Media. The project focuses on subtasks A and B. In
sub-task A, the goal is to discriminate between offensive and non-offensive posts. In
sub-task B, the focus is on identifying the type of offensive content in the post.
For more information about the task, datasets and evaluation check out:
task website:
https://sites.google.com/site/offensevalsharedtask/offenseval2019

paper: https://www.aclweb.org/anthology/S19-2010/


# NLP week - NUIG - SFI Centre for Research Training in Artificial Intelligence
http://crt-ai.cs.ucc.ie/
## 24-28 May 2021
**Group 1 - Cohort 1**
- Duy Nguyen (DCU) - manh.nguyen5@mail.dcu.ie
- Andrew Neary (NUIG) - A.Neary6@nuigalway.ie
- Alberto Castagna (TCD) - acastagn@tcd.ie
- Andrea Rossi (UCC) - a.rossi@cs.ucc.ie
- Enda O'Shea (UL) - Enda.OShea@ul.ie
- Priya Rani (NUIG) - priya.rani@insight-centre.org

# Models

**ML approaches**
- Logistic Regression
- Random Forest
- XGB

**DL approaches**
- LSTM+CNN
- BERT

# Evaluation Metrics
- Accuracy
- F1
- Precision
- Recall

# Results - TASK A

|  |  | **OFF** |  |  | **NOT** |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Model** | **Precision** | **Recall** | **F1** | **Precision** | **Recall** | **F1** | **F1 Macro** | **Accuracy** |
| LR/TF\_IDF | 0.72 | **0.99** | 0.83 | 0.25 | 0.008 | 0.02 | 0.425 | 0.72 |
| LR/Word2Vec | 0.80 | 0.97 | 0.88 | 0.83 | 0.36 | 0.50 | 0.69 | 0.80 |
| RF/TF\_IDF | 0.7152 | 0.8870 | 0.7919 | 0.2307 | 0.0875 | 0.1269 | 0.4527 | 0.66395 |
| RF/Word2Vec | 0.7916 | 0.9806 | 0.8760 | **0.8695** | 0.3333 | 0.4819 | 0.6789 | 0.8 |
| XGB/TF\_IDF | 0.7197 | 0.9774 | 0.8290 | 0.2222 | 0.0166 | 0.0310 | 0.43 | 0.7093 |
| XGB/Word2Vec | 0.8147 | 0.95 | 0.8771 | 0.7737 | 0.4416 | 0.5623 | 0.7197 | 0.8081 |
| LSTM+CNN | 0.75 | 0.91 | 0.82 | 0.68 | 0.41 | 0.51 | 0.67 | 0.74 |
| BERT | **0.8752** | 0.9387 | **0.9058** | 0.8051 | **0.6542** | **0.7218** | **0.8138** | **0.8593** |

# Results - TASK B

|  |  | **OFF** |  |  | **NOT** |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Model** | **Precision** | **Recall** | **F1** | **Precision** | **Recall** | **F1** | **F1 Macro** | **Accuracy** |
| LR/TF\_IDF | 0.0 | 0.0 | 0.0 | 0.8875 | **1.0** | 0.9404 | 0.4792 | 0.8875 |
| LR/Word2Vec | **0.75** | 0.1111 | 0.1935 | 0.90 | 0.9953 | 0.9443 | 0.5689 | 0.8958 |
| RF/TF\_IDF | 0.0 | 0.0 | 0.0 | 0.8861 | 0.9859 | 0.9333 | 0.4667 | 0.875 |
| RF/Word2Vec | 0.6666 | 0.0741 | 0.1333 | 0.8945 | 0.9953 | 0.9422 | 0.5378 | 0.8917 |
| XGB/TF\_IDF | 0.0 | 0.0 | 0.0 | 0.8875 | 1.0 | 0.9404 | 0.4702 | 0.8875 |
| XGB/Word2Vec | 0.6666 | 0.0741 | 0.1333 | 0.8945 | 0.9953 | 0.9422 | 0.5378 | 0.8917 |
| LSTM+CNN | 0.39 | 0.26 | 0.31 | 0.77 | 0.86 | 0.81 | 0.58 | 0.70 |
| BERT | 0.625 | **0.5555** | **0.5882** | **0.9444** | 0.9577 | **0.951** | **0.7696** | **0.9125** |
