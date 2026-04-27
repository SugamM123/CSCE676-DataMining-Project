# Amazon Review Analysis: Text Mining & Topic Modeling

## Overview
This repository contains the final project for CSCE 676: Data Mining. It provides an end-to-end pipeline for evaluating consumer feedback on the Amazon Product Reviews 2023 dataset (Cell Phones and Accessories). The project features:

*   **Classical Text Mining**: TF-IDF embeddings and standard clustering techniques.
*   **Neural Topic Modeling**: Implementation of BERTopic to uncover latent, highly specific product defects.
*   **Bias Analysis**: Statistical evaluation of verified versus unverified purchase ratings and temporal inflation.

This framework demonstrates how transformer-based models can complement standard token-level text analysis to yield actionable business intelligence from raw, spontaneous review data.

**Project Video:** https://youtu.be/fXdpQpzoazQ
**Main Deliverable:** `main_notebook.ipynb`

## Installation
Clone this repository and install the required dependencies:

```bash
git clone https://github.com/SugamM123/CSCE676-DataMining-Project.git
cd CSCE676-DataMining-Project
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

This will install all necessary packages including `pandas`, `scikit-learn`, and `bertopic`. 

## Quick Start

### 1. Add Amazon Review Data
Obtain the Amazon Reviews 2023 dataset (Cell Phones and Accessories) and place it in the `data/` directory. Due to size constraints, the data is not tracked in this repository.

### 2. Run the Analysis
Launch Jupyter Notebook to execute the primary analysis pipeline:

```bash
jupyter notebook main_notebook.ipynb
```

For previous iterations and early exploratory data analysis, refer to `checkpoint1.ipynb` and `checkpoint2.ipynb` located in the `checkpoints/` directory.

## Key Findings
Our analysis yielded several distinct insights regarding product satisfaction:

*   **Topic Coherence**: BERTopic significantly outperformed classical LDA in identifying nuanced product defects (e.g., specific battery drain issues vs. general "bad phone" clusters).
*   **Rating Biases**: Verified purchases exhibited statistically less temporal inflation compared to unverified reviews, providing a more reliable signal of true product quality.
*   **Defect Correlation**: A strong correlation was identified between isolated battery-related vocabulary and extreme 1-star ratings.

## Key Features
*   **BERTopic Integration**: Utilizes transformer embeddings to group semantically similar reviews into highly interpretable topics.
*   **Bias Diagnostics**: Breaks down review distributions across temporal and verification axes.
*   **Curated Data Pipeline**: Preprocessing methods designed to handle large-scale, messy e-commerce textual data.

## Notes
*   This project was originally developed and executed in Google Colab (Python 3.11). The `requirements.txt` reflects the exact environment used for full reproducibility.
*   The raw dataset is sourced from the McAuley Lab at UCSD.

## Citation
If referencing the dataset used in this analysis, please cite:

```bibtex
@article{hou2024bridging,
  title={Bridging Language and Items for Retrieval and Recommendation},
  author={Hou, Yupeng and Li, Jiacheng and He, Zhankui and Yan, An and Chen, Xiusi and McAuley, Julian},
  journal={arXiv preprint arXiv:2403.03952},
  year={2024}
}
```
