<div id="top"></div>

[![Contributors][contributors-shield]][contributors-url]

<div align="center">
  <h1 align="center">Clustering for Semi-Supervised Learning on Disasters Tweets</h1>
</div>

<!-- ABOUT THE PROJECT -->
## About The Project

Cluster analysis as an unsupervised learning technique is widely implemented throughout many fields of data analytics. When applied to data suited for hierarchical or partitional clustering, it can provide valuable insights into latent groups of the dataset and further improve your understanding of key features that can describe and classify individuals into meaningful clusters for your use case. In this project, we explore an alternative application of partitional clustering to improve the performance of supervised learning classification tasks of text samples when the resources to label training data are limited. By introducing what we call “representative labelling” with K-Means clustering, we show a consistent improvement in classification metrics of Logistic Regression and K-Nearest Neighbors algorithms when compared to naively labelled instances.

## Aim

- Propose "representative labeling" as a tool for possible improvement on the efficiency of annotating tasks of unstructured text data.

- Adapt the method introduced by Géron, A. (2019). Chapter 9. Unsupervised Learning Techniques. In Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow (2nd Edition) to text data, and evaluate the results.

- Investigate clustering techniques as a tool to segment a Twitter dataset into labeling sample candidates.

## Results

Representative labeling with K-Means clustering as a semi-supervised approach to classification tasks, as initially introduced by Géron, A. 2019 in the MNIST dataset, shows promising results also on text data. The metric scores for the optimum number of training samples on Logistic Regression and KNN Classifier shows a substantial increase in performance with the proposed method, when compared to naively selected training samples. **For these baseline classification algorithms the results shows comparable metric scores using up to twenty time less data.** It can, therefore, be suggested as a solid alternative to select the best samples for labeling when the resources for data annotation are limited.

### Future research

Topics to be explored that can improve clustering performance and potentially lead to better results.
1. Implement pre-trained word embeddings to capture semantic representations. As an alternative to the proposed LSA for dimensionality reduction, word embeddings can vectorize the text into a dense geometric representation that can leverage the semantics of words.
2. Introduce a topic modeling algorithm as a feature engineering task. By assigning samples to topics, they can be compared to clustering results to better assess how effectively your clustering method segmented the dataset.

### Considerations

Important aspects to consider when implementing the proposed method.
1. Representative labeling might induce bias in the classification model if K is too low for the diversity present in the original dataset.
2. Overfitting might occur earlier during the training and validation process when using representative labeled samples since the concept sets aside hard-to-define, diffuse, and less representative samples.
3. Some of the K-Means assumptions for an accurate clustering are not proved during this method due to the high dimensionality and number of clusters. Hence, unequal variance and anisotropicity problems might result in inappropriate cluster centers (and, therefore, inappropriate representative samples).

## About this Repository

This repository contains the source code for the above-mentioned tasks, with an extended view of the results, including a more in-depth look at the clusters obtained through the proposed method. The dataset is originally available at the [Kaggle Competition page](https://www.kaggle.com/c/nlp-getting-started/overview).

For a more in-depth look into the method and results, please refer to the [report](https://github.com/erich-hs/Tweets-Semi-Supervised/blob/master/report/Tweets_Semi_Supervised_Report.pdf).

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/erich-hs/Elderly-Wellbeing.svg?style=for-the-badge
[contributors-url]: https://github.com/erich-hs/Elderly-Wellbeing/graphs/contributors
