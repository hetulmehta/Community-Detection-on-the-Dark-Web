
# Community Detection on the Dark Web

This project explores community detection algorithms for analyzing Dark Web networks, providing valuable insights into the structure and organization of hidden online communities.

## Overview

We implemented and compared three popular community detection algorithms:
- Leiden
- Louvain 
- Label Propagation

Our analysis uncovered multiple distinct and meaningful community structures within Dark Web networks, shedding light on the organization of various activities and interests in this hidden part of the internet.

## Key Features

- Data collection from Dark Web sources using a crawler
- Implementation of Leiden, Louvain, and Label Propagation algorithms
- Comparative analysis of algorithm performance
- Visualization of detected communities
- Categorization and labeling of Dark Web URLs
- Evaluation metrics including modularity, coverage, and conductance

## Datasets

- Original dataset: 9386 nodes
- Subset dataset: 2722 nodes

## Results

### Louvain Algorithm
- On the original dataset (9386 nodes):
  - Identified 103 distinct communities
  - 92 communities had more than 50% of their nodes belonging to the same category
- On the subset dataset (2722 nodes):
  - Formed 128 communities
  - 123 communities had over 50% of nodes belonging to the same category

### Leiden Algorithm
- On the original dataset:
  - Performance similar to Louvain
- On the subset dataset (2722 nodes):
  - Formed 128 communities
  - 123 communities had more than 50% of nodes belonging to the same category

### Label Propagation Algorithm
- On the original dataset:
  - Used to predict categories of 3000 unlabeled nodes
  - Achieved 68% accuracy in predicting URL categories
- On the subset dataset:
  - Used to predict categories of 875 unlabeled nodes
  - Achieved 76% accuracy in predicting URL categories

### Comparison of Louvain and Leiden Algorithms

| Algorithm | Dataset  | Modularity | Coverage | Conductance |
|-----------|----------|------------|----------|-------------|
| Louvain   | Original | 0.941      | 0.987    | 0.01        |
| Leiden    | Original | 0.942      | 0.987    | 0.011       |
| Louvain   | Subset   | 0.58       | 0.99     | 0.005       |
| Leiden    | Subset   | 0.581      | 0.995    | 0.005       |

## Potential Applications

- Cybersecurity threat intelligence
- Law enforcement investigations
- Academic research on online communities
- Understanding the structure of hidden networks

## Future Work

- Incorporate temporal analysis to study community evolution
- Explore overlapping community detection methods
- Enhance URL categorization with machine learning techniques
- Investigate the role of key nodes in community formation


