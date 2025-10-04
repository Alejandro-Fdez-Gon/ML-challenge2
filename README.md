# False Political Claim Detection Challenge  

This repository contains my participation in a **Natural Language Processing (NLP) and Machine Learning competition** based on a real-world problem: predicting whether a **political claim** is **true or false**.  

The task simulates the role of a fact-checker who needs to assess the truthfulness of statements made by politicians or public figures.  

## 📌 Problem Statement  
Given a dataset of political claims, the goal is to **build a classifier that determines whether a claim is false or true**.  

As a fact-checker, the key question is:  
👉 *Is this political claim false? Why or why not?*  

This decision is made by analyzing historical claims and their context using NLP and ML techniques.  

## 📊 Evaluation Metric  
The competition is evaluated using **accuracy and classification metrics**, as it is a **binary classification problem** (True / False).  

- **Precision (p):** Ratio of true positives to all predicted positives.  
- **Recall (r):** Ratio of true positives to all actual positives.  
- **F1-Score:** Harmonic mean of precision and recall, useful for imbalanced classes.  

## 📂 Dataset Description  

The dataset consists of political claims with metadata about the speaker, topic, and context.  

**Files provided:**  
- `train.csv` → Training data with features + target (`label`).  
- `test.csv` → Test data (without target).  
- Metadata includes speaker, occupation, party affiliation, and geographic context.  

**Main Features:**  
- `id` → Unique identifier of the claim  
- `label` → **Target variable** (0 = True, 1 = False)  
- `statement` → Text of the claim  
- `subject` → Topic of the claim  
- `speaker` → Person making the claim  
- `speaker_job` → Occupation of the speaker  
- `state_info` → Geographic context  
- `party_affiliation` → Political party of the speaker  

## 🗂️ Project Structure  

The workflow has been divided into several Jupyter notebooks:  

1. **`1.1_Carga_limpieza_datos.ipynb`** → Data loading & initial cleaning  
2. **`1.2_Carga_limpieza_datos-LLM_Dataset_Completation.ipynb`** → Dataset completion using LLM techniques  
3. **`1.3_Carga_limpieza_datos-Transformers.ipynb`** → Text preprocessing with Transformers  
4. **`1.4_Carga_limpieza_datos-Dictionary-n-Onehot.ipynb`** → Encoding categorical variables  
5. **`2_Visualizacion_de_los_datos.ipynb`** → Exploratory Data Analysis (EDA)  
6. **`3_Model_Evaluation.ipynb`** → Model evaluation strategy & metrics  
7. **`4_Seleccion_caracteristicas_y_preprocesado.ipynb`** → Feature selection & preprocessing  
8. **`5_Entrenamiento_y_evaluacion_modelos_TF_IDF.ipynb`** → Model training & evaluation using TF-IDF features  
9. **`6_Entrenamiento_y_evaluacion_modelos_word2Vec.ipynb`** → Word2Vec-based models  
10. **`7_Entrenamiento_y_evaluacion_modelos_Hugging.ipynb`** → Hugging Face Transformers models  
11. **`8_Entrenamiento_y_evaluacion_modelos_Selectivo.ipynb`** → Selective model training experiments  
12. **`9_Visualización_de_resultados.ipynb`** → Visualization of results & performance metrics  
