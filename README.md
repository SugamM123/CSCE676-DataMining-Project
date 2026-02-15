# CSCE 676: Data Mining Project

## Amazon Cell Phones & Accessories Reviews — Text Mining & Topic Modeling

### Overview
This project applies data mining techniques to the **Amazon Product Reviews 2023** dataset (Cell Phones and Accessories category) to uncover patterns in consumer feedback. We combine **course techniques** (text mining, TF-IDF embeddings, clustering) with **beyond-course methods** (BERTopic neural topic modeling, transformer-based embeddings) to analyze how review language relates to product satisfaction.

### Research Questions
1. What latent topics exist in Cell Phones and Accessories reviews, and how do they correlate with star ratings?
2. Does BERTopic produce more coherent and actionable topic clusters than classical LDA?
3. Can we identify systematic rating biases (verified vs. unverified, temporal inflation) that distort product quality signals?

### Dataset
- **Source:** [Amazon Reviews 2023](https://amazon-reviews-2023.github.io/) (McAuley Lab, UCSD)
- **Category:** Cell Phones and Accessories
- **Sample Size:** 500,000 reviews (sampled from ~10M+)
- **Features:** Review text, star ratings (1–5), timestamps, user IDs, product IDs, verified purchase flags, helpful votes

### Project Structure
```
├── checkpoint1.ipynb        # Checkpoint 1: Dataset Selection & EDA
├── requirements.txt         # Python dependencies
├── README.md                # This file
├── .gitignore               # Git ignore rules
└── data/                    # Downloaded data (not tracked in git)
```

### Setup
```bash
# Clone the repository
git clone <your-repo-url>
cd <your-repo-name>

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook checkpoint1.ipynb
```

### Checkpoints
| Checkpoint | Description | Date |
|---|---|---|
| 1 | Dataset Selection & EDA | Feb 3, 2026 |
| 2 | Initial Research Question | Mar 5, 2026 |
| 3 | Deep Dive | Apr 2, 2026 |
| 4 | Project Showcase | Week of Apr 20, 2026 |
| 5 | Final Deliverable | Apr 27, 2026 |

### References
- Hou, Y., Li, J., He, Z., Yan, A., Chen, X., & McAuley, J. (2024). Bridging Language and Items for Retrieval and Recommendation. *arXiv preprint arXiv:2403.03952*.

### License
This project is for academic purposes (CSCE 676, Texas A&M University).
