# Transparent Extraction of Renal Tumor Characteristics from Pathology Reports Using LLMs

## Overview
This repository contains the project "Transparent Extraction of Renal Tumor Characteristics from Pathology Reports Using LLMs," undertaken by Anna Dominic and Chen Chen. The project aims to leverage Large Language Models (LLMs) to extract and interpret complex data from pathology reports, specifically focusing on renal tumor characteristics. Due to the sensitive nature of the medical data, the code and data are not shared publicly.

## Team Members
- Anna Dominic (amd9200@nyu.edu)
- Chen Chen (cc4865@nyu.edu)

## Project Structure

### 1. Introduction
- **Objective**: To accurately identify renal tumor characteristics such as tumor margin status, lymph node staging, and the presence of multiple tumors using LLMs.
- **Significance**: Enhances clinical decision-making by providing transparent and accurate extraction of critical features from pathology reports, thereby fostering trust among clinicians.

### 2. Data Privacy
- **Data Source**: Electronic Health Records (EHRs) from NYU Langone Health, specifically pathology reports for nephrectomies from 2000 to 2024.
- **Data Handling**: All LLMs are employed within NYU Langone’s secured virtual desktop infrastructure and via NYUTron, ensuring secure and encrypted interactions. Synthetic data is used for demonstrations, and only aggregate performance statistics are shared.

### 3. Objectives
- **Use BERTViz**: Validate model predictions by visualizing attention mechanisms.
- **Chain-of-Thought Prompt Engineering**: Iteratively refine input text to generate accurate responses and minimize hallucination errors.
- **Interactive Confusion Matrix**: Compare performance metrics across different prompt engineering approaches and patient demographics.

### 4. Methods
#### Open-sourced Models
- **GPT-2, BERT, and BioBERT**: Used for analyzing and classifying EHRs, with BERTViz employed to visualize attention mechanisms.
- **Preprocessing**: Tokenization, normalization, and truncation to manage input text length and focus on relevant information.

#### Close-sourced Models: Chain-of-Thought Prompting
- **Brute Force Prompt**: Baseline approach requesting all three features simultaneously.
- **Chain-of-Thought Prompt**: Sequentially narrows down input text to relevant sections, reducing hallucination errors and improving accuracy.

### 5. Performance Comparison
- **Interactive Confusion Matrix**: Created using D3.js and TensorFlow, it allows dynamic comparisons of performance across different approaches, races, and features of interest.

### 6. Evaluation
#### Open-sourced Models
- **GPT-2**: Showed potential for generating narrative responses but struggled with lengthy texts.
- **BERT and BioBERT**: Demonstrated robust classification capabilities, especially with effective preprocessing.
- **BERTViz**: Provided valuable insights into model focus and decision-making processes.

#### Close-sourced Models
- **Chain-of-Thought vs. Brute Force**: Chain-of-thought approach consistently outperformed brute force in accuracy, false positive rate, and false negative rate across all metrics.

### 7. Conclusion
- **Open-sourced Models**: Further research needed to enhance performance with domain-specific pre-training and better handling of long texts.
- **Close-sourced Models**: Chain-of-thought interactive confusion matrix establishes a framework for using LLMs to extract clinical features from pathology reports.

### 8. Future Work
- **Expanded Analysis**: With more labeled data, a comprehensive analysis of model performance across different demographics such as gender and age group will be conducted.
- **Enhanced Tools**: Development of advanced visualization tools to increase transparency and trust in automated classification systems.

## Acknowledgements
We are grateful to Dr. Madhur Nayan for his mentorship and to NYU Langone Health for providing access to the data. We also thank the teaching staff for their support.

## Files
Due to the sensitive nature of the data, the code and data used in this project are not shared publicly.

## Contact
For further information, please contact the team members via their provided email addresses.
