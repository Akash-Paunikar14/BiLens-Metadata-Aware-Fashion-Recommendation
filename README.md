# Metadata-Aware and Robust Multimodal Fashion Recommendation

A multimodal fashion recommendation system integrating visual, textual, and structured product metadata using deep learning and similarity-based retrieval.

## 📌 Project Overview

This project develops an intelligent fashion product recommendation system that combines computer vision and natural language processing techniques to recommend visually and semantically similar fashion products.

Inspired by the BiLens research approach, the system uses product images, automatically generated image descriptions, and structured product metadata to create rich multimodal product representations.

The proposed approach extends the baseline multimodal recommendation pipeline by incorporating product metadata as an additional modality and investigating recommendation robustness under degraded image quality.

## 🎯 Objectives

- Develop a multimodal fashion product recommendation system.
- Extract visual features from product images using Vision Transformer (ViT).
- Generate image descriptions using Florence-2.
- Convert generated descriptions into semantic embeddings using BERT.
- Incorporate structured product metadata as a third modality.
- Combine multimodal representations using feature fusion.
- Retrieve similar products using cosine similarity.
- Evaluate recommendation consistency and robustness under degraded image quality.

## 🏗️ System Architecture and Methodology

The proposed system uses three different modalities to represent fashion products.

### 1. Visual Modality

- Input: Fashion product image.
- Model: Vision Transformer (ViT).
- Output: Visual feature embedding.

### 2. Textual Modality

- Input: Fashion product image.
- Caption generation: Florence-2.
- Text embedding: BERT.
- Output: Semantic text embedding.

### 3. Metadata Modality

Structured product information is used to provide additional contextual information.

Metadata features include:
- Category
- Subcategory
- Article Type
- Colour
- Usage

These features provide information that may not be completely captured by visual and textual representations.

### 4. Multimodal Feature Fusion

The extracted visual, textual, and metadata representations are combined to generate a unified product representation.

The baseline approach combines visual and textual features, while the proposed approach additionally incorporates structured metadata.

### 5. Similarity-Based Recommendation

- Cosine similarity is used to calculate similarity between product representations.
- Products are ranked according to their similarity scores.
- The system retrieves the Top-K most similar products.

## 📂 Dataset

**Fashion Product Images (Small)**

Dataset Source: Kaggle – Param Aggarwal

Dataset link: https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small

The dataset contains fashion product images along with structured product metadata.

Main dataset components:

- `images/` – Contains fashion product images.
- `styles.csv` – Contains product information and metadata.

The dataset includes different fashion categories such as apparel, footwear, accessories, and personal care.

## 🛠️ Technologies and Tools

- Python
- Google Colab
- PyTorch
- Hugging Face Transformers
- Florence-2
- Vision Transformer (ViT)
- BERT
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

## 📊 Experimental Evaluation

The system is evaluated through experiments focusing on recommendation consistency and robustness.

The evaluation includes:

- Multi-query recommendation consistency.
- Top-K recommendation overlap.
- Recommendation stability under degraded image quality.
- Comparison between baseline and proposed multimodal approaches.

The experiments help investigate how incorporating product metadata affects multimodal product representation and recommendation behaviour.

## 🚀 Implementation

The project was implemented using Python in Google Colab.

The Jupyter Notebook containing the complete implementation, model pipeline, and experiments is available in this repository.

To reproduce the experiments:

1. Open the project notebook.
2. Open it using Google Colab.
3. Install the required dependencies.
4. Download or connect the Fashion Product Images dataset.
5. Execute the notebook cells in sequence.

## 🔮 Future Scope

- Scale the recommendation system to larger product collections.
- Explore advanced multimodal fusion techniques.
- Improve recommendation relevance using additional evaluation metrics.
- Investigate more robust visual feature extraction methods.
- Develop an interactive fashion recommendation application.

## ✅ Project Status

**Completed**

The project implementation and planned experimental evaluation have been completed. The system demonstrates a metadata-aware multimodal approach to fashion product recommendation by combining visual, textual, and structured product information.

## 👨‍💻 Project Information

**Project Title:** Metadata-Aware and Robust Multimodal Fashion Recommendation

**Research Inspiration:** BiLens – Multimodal Fashion Product Recommendation

**Domain:** Machine Learning | Computer Vision | Natural Language Processing

**Implementation Platform:** Google Colab

---

*This project is developed for academic and research purposes.*
