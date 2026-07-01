# Hostile-Content-Detection-in-Hindi
Hindi Hostile Content Detection using IndicBERT v2 and Transformer-based Deep Learning
# Hostile Content Detection in Hindi using Deep Learning

## Overview

This project presents a deep learning-based framework for detecting hostile content in Hindi social media text. The proposed system aims to automatically identify harmful online content and classify it into hostile and non-hostile categories while also supporting fine-grained classification of different hostile content types.

The model leverages IndicBERT v2, Convolutional Neural Networks (CNN), and Transformer Encoder layers to effectively capture both local textual patterns and long-range contextual dependencies. The system is specifically designed to handle the linguistic diversity, code-mixing, transliteration, and informal writing styles commonly found in Hindi social media posts.

---

## Problem Statement

The rapid growth of social media platforms has resulted in a significant increase in hostile online content, including:

- Hate Speech
- Offensive Language
- Fake News
- Defamation

Manual moderation of millions of posts generated daily is impractical. Therefore, an automated hostile content detection system is required to identify and mitigate harmful content efficiently.

---

## Objectives

- Develop an efficient deep learning framework for Hindi hostile content detection.
- Utilize IndicBERT v2 for contextual representation learning.
- Enhance feature extraction using CNN and Transformer Encoder layers.
- Improve contextual understanding through emoji-aware preprocessing.
- Perform both coarse-grained and fine-grained classification.
- Compare multiple architectures and identify the most effective model.

---

## Dataset

The project uses the CONSTRAINT 2021 Hindi Hostile Content Dataset.

### Dataset Statistics

| Category | Samples |
|-----------|----------|
| Non-Hostile | 4358 |
| Hostile | 3834 |
| Fake News | 1638 |
| Hate Speech | 1132 |
| Offensive | 1071 |
| Defamation | 810 |

The dataset contains Hindi social media posts annotated for hostile content detection.

---

## Hostile Categories

### Fake News
False or misleading information intended to deceive users.

### Hate Speech
Content targeting individuals or groups based on religion, ethnicity, race, or other protected characteristics.

### Offensive
Posts containing abusive, vulgar, or insulting language.

### Defamation
Content aimed at damaging the reputation of an individual or organization.

---

## Methodology

### 1. Data Preprocessing

The following preprocessing steps were applied:

- Emoji to text conversion (Emoji-aware preprocessing)
- URL removal
- Special character removal
- Extra whitespace normalization
- Label encoding

### 2. Feature Extraction

The cleaned text is processed using:

- IndicBERT v2 Tokenizer
- IndicBERT v2 Embeddings

### 3. Deep Learning Architecture

The proposed architecture consists of:

Input Text
→ IndicBERT v2 Embeddings
→ CNN Layers
→ Transformer Encoder Layers
→ Adaptive Average Pooling
→ Fully Connected Layer
→ Classification Output

### Architecture Components

- IndicBERT v2
- CNN Layers
- Multi-Head Self Attention
- Transformer Encoder Blocks
- Adaptive Average Pooling
- Fully Connected Classification Layer

---

## Model Features

### IndicBERT v2

- Designed specifically for Indian languages.
- Generates contextual embeddings for Hindi text.
- Handles multilingual and code-mixed content effectively.

### CNN Layers

- Extract local phrase-level features.
- Detect hostile keywords and patterns.

### Transformer Encoder Layers

- Capture long-range contextual dependencies.
- Improve semantic understanding through self-attention.

### Emoji-Aware Processing

Instead of removing emojis, they are converted into textual descriptions to preserve sentiment and contextual information.

---

## Classification Tasks

### Coarse-Grained Classification

Binary Classification:

- Hostile
- Non-Hostile

### Fine-Grained Classification

Multi-label Classification:

- Fake News
- Hate Speech
- Offensive
- Defamation



Department of Computer Science & Engineering  
Haldia Institute of Technology
