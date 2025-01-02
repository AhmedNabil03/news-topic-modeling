# News Topic Modeling with BERTopic

This repository contains a project for topic modeling on a news dataset using BERTopic, a framework for extracting interpretable topics from large datasets.

## Features

- Preprocessing news data for tokenization, cleaning, and length constraints.
- Sentence embeddings using **LaBSE**.
- Dimensionality reduction with **UMAP**.
- Clustering using **HDBSCAN**.
- Arabic stopword removal with a custom list.
- Topic representation using **KeyBERTInspired**.
- Advanced visualizations for topic analysis:
  - Topic heatmaps
  - Hierarchical clustering
  - Topics over time
  - Topics per class.

## Workflow

1. **Preprocessing**: 
   - Combine title and content into a single text field.
   - Clean the text by removing URLs, replacing digits, handling punctuation, and tokenizing.
   - Remove duplicates and filter text based on token length.

2. **Embedding**: 
   - Generate sentence embeddings using the **LaBSE** model.

3. **Clustering and Dimensionality Reduction**:
   - Reduce embedding dimensionality with UMAP.
   - Cluster the embeddings with HDBSCAN.

4. **Topic Modeling**:
   - Represent topics using `KeyBERTInspired`.
   - Visualize topics with BERTopic’s built-in tools.

5. **Inference**:
   - Infer topics for new text samples.

## Visualizations

The following visualizations are included in the project:

- **Topic Distribution**: Overview of topics in the dataset.
- **Topics Over Time**: Track how topics evolve over time.
- **Topics Per Class**: Explore topic distributions per source domain.
- **Hierarchical Topics**: Visualize topic hierarchies.
