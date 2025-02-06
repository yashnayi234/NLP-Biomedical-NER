# Biomedical Named Entity Recognition (NER) Using Transformer-Based Models

## Overview
This project aims to perform **Biomedical Named Entity Recognition (NER)** by identifying and classifying entities like diseases and chemicals from unstructured biomedical text. This task plays a critical role in applications such as clinical decision support, drug discovery, and building biomedical knowledge bases. 

We leverage pre-trained transformer-based models, such as **BioBERT** and **BERT**, combined with sequence modeling techniques to improve accuracy and consistency in recognizing complex biomedical entities. The project is evaluated using the **BC5CDR** dataset, which provides annotations for two entity types: chemicals and diseases.

### Key Features:
- Utilizes state-of-the-art transformer models.
- Includes training, testing, and qualitative evaluations.
- Runs seamlessly on **Google Colab** with GPU acceleration.
- Supports standard metrics for comprehensive evaluation.

---

## Running the Project on Google Colab
Follow these steps to execute the files:

### 1. Download the Project Files:
Clone or download the repository:
```bash
git clone https://github.com/yashnayi234/NLP-Biomedical-NER
```
Alternatively, download the files manually.

### 2. Upload Files to Google Colab:
- Open Google Colab.
- Upload the necessary `.ipynb` files to your Colab workspace.

### 3. Enable GPU in Colab:
- Go to **Runtime > Change Runtime Type**.
- Set the **Hardware Accelerator** to **GPU**.

### 4. Install Dependencies:
Run the following command to install required libraries:
```bash
!pip install transformers torch scikit-learn numpy pandas seqeval
```

### 5. Execute the Notebooks:
- Run the cells sequentially in the provided `.ipynb` files.
- The scripts handle preprocessing, training, and evaluation with outputs logged directly in the notebook.

---

## Project Files
### 1. **NER_BERT_BiLSTM.ipynb**
   - Implementation of Clinical BERT with a BiLSTM layer for sequence tagging.

### 2. **NER_BIOBERT_BiLSTM.ipynb**
   - Implementation of BioBERT with a BiLSTM layer for improved sequential dependency modeling.

### 3. **NER_BIOBERT_without_LSTM.ipynb**
   - A simpler BioBERT model without additional sequence modeling layers.

### 4. **NER_BIOBERT_WITHCRF.ipynb**
   - BioBERT model integrated with a CRF layer for structured prediction.

---

## Evaluation Metrics
- **Precision**: Proportion of correctly identified entities out of all predicted entities.
- **Recall**: Proportion of correctly identified entities out of all actual entities.
- **F1-Score**: Harmonic mean of precision and recall for balanced evaluation.
- **Token-Level Accuracy**: Proportion of correctly classified tokens in the dataset.

---

## How to Test the Models
### Evaluate on Test Set:
- Each notebook includes code to evaluate the model on the **BC5CDR** test set.

### Test on Sample Sentences:
- Provide custom sample sentences in the input cells of the notebooks. 
- The models will generate predictions for real-world performance testing.

---

## Future Work
- **Reinforcement Learning**: Optimize sequence-level predictions.
- **Multilingual Support**: Extend models to handle biomedical texts in multiple languages.
- **Hybrid Approaches**: Combine transformers with graph-based methods for entity linking and overlapping entity recognition.

---

## Team 60 Members:
- **Yash Raythatha**
- **Parin Patel**
- **Yash Nayi**
