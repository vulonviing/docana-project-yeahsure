# Unmasking Sarcasm on Reddit

_Group members: Emrecan, Flora_

## Introduction

Sarcasm is a nuanced linguistic phenomenon that often relies on context, sentiment incongruity, and emphatic expressions. In this project, we aim to uncover the thematic and linguistic patterns of sarcasm in Reddit posts, particularly from the r/yeahsure subreddit. Building on the TLDR dataset, our goal is to detect sarcasm using NLP techniques and explore its underlying structure.

## Dataset

We utilize the [Webis-TLDR-17 dataset](https://huggingface.co/datasets/webis/tldr-17), which contains user-generated Reddit posts and summaries. This dataset enables fine-grained analysis of sarcasm signals and is well-suited for classification tasks involving short-form text.

[🔍 Click here to view the Term Rank Visualization](index.html) 

## Methods

### Setup

Our project is built using Python 3.x and the following key libraries:

- `transformers` (Hugging Face)
- `scikit-learn`
- `matplotlib`, `seaborn`
- `pandas`, `numpy`
- `nltk`, `spacy`

To set up the environment:

```bash
conda create --name sarcasm_env python=3.10
conda activate sarcasm_env
pip install -r requirements.txt
```

### Experiments

We performed:

- **Text Embedding & Clustering**: Extracted contextual embeddings using RoBERTa and applied HDBSCAN for topic discovery.
- **Sarcasm Classification**: Fine-tuned a RoBERTa model on labeled Reddit posts using the "/s" tag for supervision.
- **Linguistic Analysis**: Identified sarcasm markers such as sentiment polarity mismatches, overuse of punctuation, and exaggerated expressions using TF-IDF and sentiment scoring.

## Results and Discussion

Our results show that sarcasm can be detected with reasonable accuracy. Key indicators include sentiment flips and excessive punctuation. Clustering revealed recurring sarcastic themes related to politics, health, and social norms.

## Conclusion

We successfully demonstrated that sarcasm carries detectable linguistic patterns. Model granularity, expression density, and contextual clues are critical for identifying sarcasm in online discourse.

## Contributions

| Team Member     | Contributions                                                  |
|------------------|---------------------------------------------------------------|
| Flora            | Embedding extraction, topic clustering, visualization         |
| Flora            | Data cleaning, model training, fine-tuning, evaluation        |

## References

- Work in progress
