---
layout: page
title: "Projects"
permalink: /projects
---

### [Regularized Simple Graph Convolution (SGC) for improved interpretability of large datasets](https://journalofbigdata.springeropen.com/articles/10.1186/s40537-020-00366-x)

Attributed graph is a powerful tool to model many complex systems in our world. It contains two valuable sources of information, i.e the node feautures and the network strucutre, which can be analyzed efficiently by graph neural networks (GNNs) to produce accurate inference for many downstream tasks such as node classification, link prediction, etc. The exponential growth of graph structured data drives the complexity of GNNs models causing concerns about processing time and interpretability of the results. This work extended a fast GNNs framework, namely the [Simple Graph Convolution (SGC)](https://proceedings.mlr.press/v97/wu19e.html) by incorporating a flexible shrinkage scheme to produce a sparser model whose fitted parameters are capable of highlighting key node features determining the class characteristics.

| ![sgc.png](/projects_img/regsgc_fig8a.png) |  ![reg-sgc.png](/projects_img/regsgc_fig8b.png)|
|Application of SGC on Cora citation dataset. The fitted weight vectors of each class is plotted as a heatmap| The proposed regularization significantly reduces the amount of weights and hightlights important features defining class membership|

### [Exploring the value of nodes with multicommunity membership for classification with graph convolutional neural networks](https://www.mdpi.com/2078-2489/12/4/170)
Sampling process plays an important role in machine learning pipeline as it provides quality training samples to build the model. However, the process of determining the best sampling method has been rarely studied in the context of graph neural networks. In this work, we evaluate the effect of multiple sampling strategies on node classification task using the [SGC](https://proceedings.mlr.press/v97/wu19e.html). Our discoveries include an indicative measure of sampling efficiency and a heuristic criterion based on network topology which can be utilized to suggest best sampling strategy for practitioners.

|Dataset | Prediction | Actual |
|:-------|:-----------|:-------|
| Cora | Descending | Descending |
| Citeseer | Descending | Descending |
| Pubmed | Ascending | Ascending |
| Amazon-pc | Descending | Ascending |
| Amazon-photo | Ascending | Ascending|
| Coauthor-cs | Descending | Descending|
| Coauthor-physics | Ascending | Descending|
| Lastfm\_Asia | Ascending | Ascending |
| Deezer\_Europe | Descending | Descending|

