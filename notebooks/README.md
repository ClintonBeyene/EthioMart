# Amharic Telegram E-commerce NER Project

## Overview
This project aims to develop a Named Entity Recognition (NER) system to extract key entities such as products, prices, and locations from Amharic Telegram e-commerce messages. The project involves data ingestion, preprocessing, labeling, model fine-tuning, comparison, and interpretability.

## Table of Contents
- Task 1: Data Ingestion and Data Preprocessing
- Task 2: Label a Subset of Dataset in CoNLL Format
- Task 3: Fine Tune NER Model
- Task 4: Model Comparison & Selection
- Task 5: Model Interpretability

## Task 1: Data Ingestion and Data Preprocessing
Set up a data ingestion system to fetch messages from multiple Ethiopian-based Telegram e-commerce channels and prepare the raw data for entity extraction.

### Steps:
1. **Identify and connect to relevant Telegram channels** using a custom scraper.
2. **Implement a message ingestion system** to collect text, images, and documents in real-time.
3. **Preprocess text data** by tokenizing, normalizing, and handling Amharic-specific linguistic features.
4. **Clean and structure the data** into a unified format, separating metadata (e.g., sender, timestamp) from message content.
5. **Store preprocessed data** in a structured format for further analysis.

## Task 2: Label a Subset of Dataset in CoNLL Format
Label a portion of the dataset in the CoNLL format for NER tasks, identifying entities such as products, prices, and locations in Amharic text.

### CoNLL Format:
- Each token (word) is labeled on its own line.
- The token is followed by its entity label.
- Blank lines separate individual sentences/messages.

### Entity Types:
- **B-Product**: The beginning of a product entity (e.g., "Baby bottle").
- **I-Product**: Inside a product entity (e.g., the word "bottle" in "Baby bottle").
- **B-LOC**: The beginning of a location entity (e.g., "Addis Abeba", "Bole").
- **I-LOC**: Inside a location entity (e.g., the word "Abeba" in “Addis Abeba”).
- **B-PRICE**: The beginning of a price entity (e.g., "ዋጋ 1000 ብር", "በ 100 ብር").
- **I-PRICE**: Inside a price entity (e.g., the word "1000" in “ዋጋ 1000 ብር”).
- **O**: Tokens that are outside any entities.

### Steps:
1. Label at least 30-50 messages from the provided dataset.
2. Save your work in a plain text file in the CoNLL format.

## Task 3: Fine Tune NER Model
Fine-tune a Named Entity Recognition (NER) model to extract key entities from Amharic Telegram messages.

### Steps:
1. Use Google Colab or any other environment with GPU support for faster training.
2. Install necessary libraries.
3. Use a pre-trained model like amseg.amharicSegmenter, XLM-Roberta, bert-tiny-amharic, or afroxmlr.
4. Load the labeled dataset in CoNLL format.
5. Tokenize the data and align the labels with tokens produced by the tokenizer.
6. Set up training arguments (learning rate, number of epochs, batch size, evaluation strategy).
7. Use Hugging Face's Trainer API to fine-tune the model.
8. Evaluate the fine-tuned model on the validation set.
9. Save the model for future use.

## Task 4: Model Comparison & Selection
Compare different models and select the best-performing one for the entity extraction task.

### Steps:
1. Fine-tune multiple models (e.g., XLM-Roberta, DistilBERT, mBERT).
2. Evaluate the fine-tuned models on the validation set.
3. Compare models based on accuracy, speed, and robustness.
4. Select the best-performing model for production.

## Task 5: Model Interpretability
Use model interpretability tools to explain how the NER model identifies entities, ensuring transparency and trust in the system.

### Steps:
1. **Implement SHAP (SHapley Additive exPlanations)** and **LIME (Local Interpretable Model-agnostic Explanations)** to interpret the model’s predictions.
2. **Analyze difficult cases** where the model might struggle to identify entities correctly (e.g., ambiguous text, overlapping entities).
3. **Generate reports** on how the model makes decisions and identify areas for improvement.


