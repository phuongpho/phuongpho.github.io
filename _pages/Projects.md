---
layout: single
title: "Projects"
permalink: /Projects/
toc: true
toc_label: "List of projects"
toc_icon: "archive"
---

## Journal papers and conference proceedings
### [Regularized Simple Graph Convolution (SGC) for improved interpretability of large datasets](https://journalofbigdata.springeropen.com/articles/10.1186/s40537-020-00366-x)

Attributed graph is a powerful tool to model many complex systems in our world. It contains two valuable sources of information, i.e the node feautures and the network strucutre, which can be analyzed efficiently by Graph Neural Networks (GNNs) to produce accurate inference for many downstream tasks such as node classification, link prediction, etc. The exponential growth of graph structured data drives the complexity of GNNs models causing concerns about processing time and interpretability of the results. This work extended a fast GNNs framework, namely the [Simple Graph Convolution (SGC)](https://proceedings.mlr.press/v97/wu19e.html) by incorporating a flexible shrinkage scheme to produce a sparser model whose fitted parameters are capable of highlighting key node features determining the class characteristics.

| ![sgc.png](/projects_img/regsgc_fig8a.png) |  ![reg-sgc.png](/projects_img/regsgc_fig8b.png)|
|Application of SGC on Cora citation dataset. The fitted weight vectors of each class is plotted as a heatmap| The proposed regularization significantly reduces the amount of weights and hightlights important features defining class membership|

### [Exploring the value of nodes with multicommunity membership for classification with graph convolutional neural networks](https://www.mdpi.com/2078-2489/12/4/170)
Sampling process plays an important role in machine learning pipeline as it provides quality training samples to build the model. However, the process of determining the best sampling method has been rarely studied in the context of graph neural networks. In this work, we evaluate the effect of multiple sampling strategies on node classification task using the [SGC](https://proceedings.mlr.press/v97/wu19e.html). Our discoveries include an indicative measure of sampling efficiency and a heuristic criterion based on network topology which can be utilized to suggest best sampling strategy for practitioners.

|Dataset | Predicted optimal strategy | Actual optimal strategy|
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

### [Exploring a link between network topology and active learning](https://ieeexplore.ieee.org/document/9528662)

Upon the findings of [*previous work*](https://www.mdpi.com/2078-2489/12/4/170) on the importance of network topology in the selection of training samples, we further study the proposed heuristic measure. We design a comprehensive set of synthetic datasets covering a wide range of network structures and input features. Utilize both synthetic and real life datasets, we then derive effective sampling approaches based on the proposed measure to facilitate the task of predicting node label.

| ![exp-link.png](/projects_img/exp_link.png) | 
| Simulation study suggests a threshold upon which optimal sampling strategy can be determined|

### [Exploring the Regularized SGC in application to social network data](http://workshop-proceedings.icwsm.org/abstract?id=2022_27)

Online social networks have a significant effect on human society and have become an important research topic for maintaining the integrity of the common social understanding. In this work, we study the application of [Simple Graph Convolution (SGC)](https://proceedings.mlr.press/v97/wu19e.html) and [our proposed extension (regularized SGC)](https://journalofbigdata.springeropen.com/articles/10.1186/s40537-020-00366-x) on a social network dataset as well as a comprehensive set of synthetic attributed graphs with varying network topologies. Our proposed framework has high predictive capability and also produces sparser model facilitating practitioner in investigation of important features relevant to class assignment.

| ![regsgc_graphtopo.png](/projects_img/regsgc_graphtopo.png) | ![regsgc_output.png](/projects_img/regsgc_output.png) |
| Simulation study covers a wide range of network topologies| Regularized framework has high predictive power and is capable of enhancing users understanding of features contribution to class assignment|

### [Link prediction with Simple Graph Convolution and regularized Simple Graph Convolution](http://www.icisdm.org/index.html)
Link prediction is an important task on attributed graph with a wide range of useful applications.In work, we adapt the flexible regularization mechanism of regularized SGC for link prediction with the goal of improving the interpretability of the fitted model.

|![link_pred_diagram.png](/projects_img/Link_pred_diagram.png)|

## Personal projects
### [OUC Meter Data Science Competition](https://sciences.ucf.edu/news/statistics-students-ouc-team-up-to-tackle-power-problems/)
The goal of this competition is to identify complex electric theft/tampering pattern in [Orlando Utilities Commission(OUC)](https://www.ouc.com/) meter reading database. We utilize temporal and spatial outlier detection approaches to discover potential suspects based on the montly ratio of water-to-electric usage. Next, the likelihood of daily tampering during a given month ia produced from the analysis of the variation of daily consumption trend.

| ![ouc_dashboard.png](/projects_img/ouc_dashboard.png)|

### 2019 Microsoft Scholarship - Predicting Major Depressive Disorder using genotyping data
In this project, we developed statistical models to classify patients’ disease status using over twenty thousand categorical biomarkers (SNPs). The data presented two major challenges: high dimensionality and large proportion of missing data. We designed a novel analytics process including effective treatment for missing information and automatic variable selection. The final model contained only a sparse set of tens of SNPs yet attained high predictive power. Simulation study validates our proposed approach under a wide range of missing rates and signal-to-noise ratios.

| ![snp_result.png](/projects_img/snp_result.png) |

### [Touring Plan – 2017 Big Data Competition](https://sciences.ucf.edu/news/predicting-wait-times-disney/)
The competition was held by Touring Plans Co. and the Department of Statistics, University of Central Florida with the goal of predicting wait times for 4 popular rides at Disney World (Splash Mountain, Kilimanjaro Safaris, Toy Story Mania, Soarin'). The real-life data span over a hundred of variables with more than half-million observations. By employing various feature engineering strategies and regularization techniques, we obtain final sparse models highlighting the impact of key features while achieving best predictive power.

