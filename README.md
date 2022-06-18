<div id="top"></div>

[![Contributors][contributors-shield]][contributors-url]

<div align="center">
  <h3 align="center">Clustering for Semi-Supervised Learning on Disasters Tweets</h3>
</div>

<!-- ABOUT THE PROJECT -->
## About The Project

Cluster analysis as an unsupervised learning technique is widely implemented throughout many fields of data analytics. When applied to data suited for hierarchical or partitional clustering, it can provide valuable insights into latent groups of the dataset and further improve your understanding of key features that can describe and classify individuals into meaningful clusters for your use case. In this project, we explore an alternative application of partitional clustering to improve the performance of supervised learning classification tasks of text samples when the resources to label training data are limited. By introducing what we call “representative labeling” with K-Means clustering, we show a consistent improvement in classification metrics of Logistic Regression and K-Nearest Neighbors algorithms when compared to naively labeled instances.

### Aim
- Propose "representative labeling" as a tool for possible improvement on the efficiency of annotating tasks of unstructured text data.

- Adapt the method introduced by Géron, A. (2019). Chapter 9. Unsupervised Learning Techniques. In Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow (2nd Edition) to text data, and evaluate the results.

- Investigate clustering techniques as a tool to segment a Twitter dataset into labeling sample candidates.

### Results

Representative labeling with K-Means clustering as a semi-supervised approach to classification tasks, as initially introduced by Géron, A. 2019 in the MNIST dataset, shows promising results also on text data. The metric scores for the optimum number of training samples on Logistic Regression and KNN Classifier shows a substantial increase in performance with the proposed method. It can, therefore, be suggested as a solid alternative to select the best samples for labeling when the resources for data annotation are limited.

## About this Repository

This repository contains the source code for the above-mentioned tasks, with an extended view of the results, including a more in-depth look at the clusters obtained through the proposed method. The dataset is originally available at the [Kaggle Competition page](https://www.kaggle.com/c/nlp-getting-started/overview)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/erich-hs/Elderly-Wellbeing.svg?style=for-the-badge
[contributors-url]: https://github.com/erich-hs/Elderly-Wellbeing/graphs/contributors
