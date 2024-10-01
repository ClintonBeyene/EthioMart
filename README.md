**Amharic Telegram E-commerce NER Project 🛍️**
=====================================

**Overview**
------------

This project aims to develop a robust Named Entity Recognition (NER) system to extract key entities such as products, prices, and locations from Amharic Telegram e-commerce messages. The project involves data ingestion, preprocessing, labeling, model fine-tuning, comparison, and interpretability.

**Table of Contents**
-----------------

1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Model](#model)
4. [Results](#results)
5. [Usage](#usage)
6. [Future Work](#future-work)
7. [Team](#team)
8. [License](#license)
9. [Acknowledgments](#acknowledgments)

**Introduction**
---------------

This project aims to develop a robust Named Entity Recognition (NER) system for the Ethiopian e-commerce market 🛍️. The system is designed to extract key business entities from Amharic text data, including product names, prices, and locations.

**Dataset**
------------

* **Source**: Telegram e-commerce channels (e.g. @mertteka)
* **Language**: Amharic
* **Format**: Text data in conll format
* **Size**: 10,000+ messages

**Model**
------------

* **Model Type**: XLM-Roberta
* **Task**: Named Entity Recognition (NER)
* **Entity Types**: Product names, prices, locations
* **Training Data**: Labeled dataset in CoNLL format

**Results**
------------

* **Accuracy**: 99.99%
* **Precision**: 1.00
* **Recall**: 1.00
* **F1-score**: 1.00

**Usage**
------------

1. Clone the repository: `git clone https://github.com/ClintonBeyene/EthioMart.git`
2. Install required libraries: `pip install -r requirements.txt`
3. Train the model: `jupyter notebook fine_Tune_XLM-Roberta.ipynb`
4. Evaluate the model: `jupyter notebook Fine_tuned_DistillBERT_1.ipynb `

**Future Work**
----------------

* Expand the model to handle images and documents
* Explore the use of NER technology in other domains
* Improve the model's performance on out-of-vocabulary words

**Team**
----------

* Beabsira Yenezer(https://github.com/Beabsira94) 🤖
* Clinton Beyene(https://github.com/ClintonBeyene) 🤖
* Seifegebriel Mosisa (https://github.com/Seife1) 🤖

**License**
----------

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

**Acknowledgments**
------------------

* Special thanks to Kifiya aim Team: 
* **Tutors**: 
* **Elias**
* **Kerod**
* **Mahlet**
* **Rediet**