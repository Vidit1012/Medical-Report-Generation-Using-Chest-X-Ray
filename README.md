# Medical Report Generation Using Chest X-Ray

> BE Final Year Project · Don Bosco Institute of Technology, Mumbai  
> **Team:** Vidit Prabhu · Varun Gokarn · Ashutosh Rane · Nikhit Rapelli

---

## Overview

An attention-based encoder-decoder model that automatically generates diagnostic text reports from chest X-ray images — aimed at reducing radiologist workload and minimizing missed diagnoses.

---

## What It Does

- Preprocessed the **IU Chest X-ray dataset** (7,471 images, ~3,955 reports) with EDA, tokenization, and CheXNet feature extraction
- Built a baseline **Encoder-Decoder** model using LSTM
- Improved results with a **Bahdanau Additive Attention** model using Beam Width Search for better report generation
- Evaluated using BLEU and ROUGE metrics

## Results

| Model | BLEU-1 | BLEU-4 | ROUGE-L (F1) |
|---|---|---|---|
| Encoder-Decoder | 0.165 | 0.127 | 0.166 |
| Attention Model | 0.299 | 0.259 | 0.391 |

The Attention model significantly outperformed the baseline across all metrics.

---

## Tech Stack

Python · TensorFlow · Keras · PyTorch · NLTK · OpenCV · CheXNet · Matplotlib · Seaborn

---

## Published Paper

See [`Group10_PubTech_Paper.pdf`](./Group10_PubTech_Paper.pdf) for the full published paper.
