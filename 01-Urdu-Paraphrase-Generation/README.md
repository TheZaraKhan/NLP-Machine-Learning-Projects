# Automatic Paraphrase Generation for the Urdu Language

**MSc Research | Natural Language Processing | Neural Sequence-to-Sequence Models**

## Research Overview

This project presents selected experiments from my master's research, *Automatic Paraphrase Generation for the Urdu Language*, conducted at COMSATS University Islamabad, Lahore Campus (2018–2020).

The research investigated neural approaches to automatic paraphrase generation for Urdu, a relatively low-resource language in Natural Language Processing (NLP).

The objective was to explore methods for generating alternative linguistic expressions while preserving the meaning of the original text.

My broader research involved four Urdu paraphrase datasets. This folder contains original experimental notebooks from the **lexical paraphrase generation** component, covering data preparation, neural model training, and automatic evaluation.

## 1. Dataset Preparation

**Notebook:** `data_prepration.ipynb`

This notebook documents additional preprocessing performed on the Urdu lexical paraphrase data before model training and evaluation.

The processing steps include:

- Loading existing Urdu lexical paraphrase pairs.
- Handling missing values in selected dataset columns.
- Removing punctuation and numerical characters.
- Filtering text containing Latin alphabet characters.
- Removing incomplete records.
- Selecting source and target text pairs.
- Preparing and exporting training and test files.

The experiments use data stored in CSV, TSV, and Excel formats.

This notebook represents additional processing after the original dataset preparation, rather than the complete dataset creation pipeline.

## 2. Neural Lexical Paraphrase Generation

**Notebook:** `Neural lexical paraphrase generation for Urdu language - EPOCHS 15.ipynb`

The lexical paraphrase generation model uses a neural encoder-decoder architecture based on Long Short-Term Memory (LSTM) networks.

The implementation uses TensorFlow and Keras to learn mappings between source and target Urdu text sequences.

### Model Architecture

The model consists of:

- **Encoder:** An embedding layer followed by an LSTM network to encode the input sequence.
- **Decoder:** An embedding layer and LSTM network initialized using the encoder's final hidden and cell states.
- **Output layers:** Fully connected layers with ReLU and Softmax activations to generate target tokens.
- **Regularization:** Dropout applied in the decoder's dense layers.
- **Teacher forcing:** Target sequences are provided to the decoder during training.
- **Inference:** Separate encoder and decoder models are constructed to generate predictions.

### Training Configuration

| Parameter | Configuration |
|---|---|
| Architecture | Encoder-Decoder Seq2Seq |
| Recurrent network | CuDNNLSTM |
| Embedding dimension | 256 |
| LSTM units | 1,024 |
| Batch size | 64 |
| Training epochs | 15 |
| Validation split | 10% |
| Optimizer | Adam |
| Loss function | Sparse categorical cross-entropy |
| Training metric | Sparse categorical accuracy |
| Maximum selected examples | 200,000 |
| Decoder dropout | 0.4 |

The training notebook includes vocabulary indexing, sequence preparation, data shuffling, model training, and inference.

Generated paraphrases are exported alongside their source and reference text for subsequent evaluation.

## 3. Automatic Evaluation

**Notebook:** `BLEU and ROUGE score for lexical paraphrases 15 EPOCHS`

The evaluation notebook compares generated lexical paraphrases with reference text using automatic NLP evaluation metrics.

### BLEU Evaluation

The notebook includes calculations for:

- BLEU-1
- BLEU-2
- BLEU-3
- BLEU-4

It uses NLTK's BLEU functions and smoothing methods to calculate scores for generated text.

### ROUGE Evaluation

The notebook calculates:

- ROUGE-1
- ROUGE-2
- ROUGE-L

The ROUGE evaluation includes precision, recall, and F1-score calculations.

The notebook processes up to 10,000 prediction records and exports individual and aggregate evaluation results.

**Evaluation note:** The BLEU calculations are preserved from the original experiment. Their argument formatting and tokenization should be reviewed before treating the resulting scores as independently validated or directly comparable with other published results.

## Experimental Workflow

The three notebooks document the following stages:

**Urdu Lexical Paraphrase Data**

↓

**Data Preparation and Cleaning**

↓

**Sequence Encoding and Vocabulary Construction**

↓

**LSTM Encoder-Decoder Training**

↓

**Paraphrase Generation**

↓

**BLEU and ROUGE Evaluation**

## Technologies Used

| Category | Technologies |
|---|---|
| Programming | Python |
| Deep Learning | TensorFlow, Keras |
| Neural Architecture | LSTM, Seq2Seq, Encoder-Decoder |
| Data Processing | Pandas, NumPy |
| NLP Evaluation | NLTK, BLEU, ROUGE |
| Development Environment | Google Colab, Jupyter Notebook |

## Related Research Publication

**Automatic Paraphrase Generation at Phrasal, and Sentence Level for Urdu Language: Data and Methods**

Zara Khan et al.  
Published in SAGE Journals, 2025.

This publication is associated with my broader research on Urdu paraphrase generation. The notebooks included here document selected lexical paraphrase experiments and should not be interpreted as the complete experimental implementation of the published study.

## Reproducibility Notes

These notebooks are preserved in their original experimental form.

- The implementation uses an earlier TensorFlow/Keras environment, including GPU-specific LSTM layers.
- Dataset files and generated predictions were originally stored in Google Drive.
- The complete datasets, trained model weights, and other experimental configurations are not included in this folder.
- Additional setup and compatible library versions may be required to rerun the experiments.

## Author

**Zara Khan**  

