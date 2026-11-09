# CMPE-255 Data Mining Process Assignment — CRISP-DM, SEMMA, KDD

Author: Weihao Fu
Course: FA26 CMPE-255 Sec 49 - Data Mining, San Jose State University
Assignment: Data Mining process Assignment - crisp-dm etc. (due November 3, 2026)

## Overview

Three projects, one per data mining methodology, each with its own dataset,
each in its own directory, each as a fully executed Colab notebook
(all code cells run, outputs embedded, no errors).

## Projects

### 1. CRISP-DM — Titanic survival prediction (`CRISP-DM/`)

- Dataset: Titanic passenger data, 891 rows × 12 columns —
  https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
- Goal: predict survival from boarding-time information.
- Phases: Business Understanding, Data Understanding, Data Preparation,
  Modeling, Evaluation, Deployment.
- Models (held-out test set, 179 passengers):
  - Logistic Regression: accuracy 0.8045, ROC-AUC 0.8505
  - Random Forest: accuracy 0.8156, ROC-AUC 0.8267
- Both models beat the 0.6145 majority-class baseline.
- Video walkthrough: https://youtu.be/OCHYE5o2AhA
- Medium article: https://medium.com/@fuweihao101/predicting-titanic-survival-step-by-step-a-crispdm-walkthrough-880324138795

### 2. SEMMA — Student performance (`SEMMA/`)

- Dataset: UCI Student Performance, `student-mat.csv` (mathematics course),
  395 rows × 33 columns —
  https://archive.ics.uci.edu/ml/machine-learning-databases/00320/student.zip
- Goal: predict pass/fail, defined as final grade G3 >= 10 (pass rate 67.1%).
- Phases: Sample, Explore, Modify, Model, Assess.
- Models (held-out test set, 79 students):
  - Logistic Regression: accuracy 0.873, ROC-AUC 0.948
  - Random Forest: accuracy 0.873, ROC-AUC 0.936
  - Gradient Boosting: accuracy 0.886, ROC-AUC 0.940
- Video walkthrough: https://youtu.be/EGoO6iJ_ZAQ
- Medium article: https://medium.com/@fuweihao101/predicting-student-performance-with-semma-can-we-flag-at-risk-students-before-the-final-exam-57c54ec509e7

### 3. KDD — Pima Indians diabetes prediction (`KDD/`)

- Dataset: Pima Indians Diabetes, 768 rows × 9 columns —
  https://raw.githubusercontent.com/jbrownlee/Datasets/master/pima-indians-diabetes.data.csv
- Goal: predict diabetes diagnosis (Outcome).
- Phases: the full 9-step KDD process, from understanding the application
  domain through to using the discovered knowledge.
- Models (held-out test set, 154 patients):
  - Logistic Regression: accuracy 0.708, ROC-AUC 0.813
  - Random Forest: accuracy 0.734, ROC-AUC 0.817
- Top drivers (Random Forest): Glucose, BMI, DiabetesPedigreeFunction.
- Video walkthrough: https://youtu.be/iqpkoNZ62ro
- Medium article: https://medium.com/@fuweihao101/finding-diabetes-risk-in-data-a-full-kdd-walkthrough-db0733bb253b

## How to run

Open any notebook in Google Colab (or Jupyter). Each notebook loads its
dataset from the source URL at runtime and runs top to bottom with no extra
setup beyond pandas, scikit-learn, matplotlib, and seaborn.

## Notes

- All code was executed end-to-end with outputs embedded; no notebook
  contains errors.
- AI assistance, as invited by the assignment brief, was used for drafting
  and critique; all code was manually verified by execution.
