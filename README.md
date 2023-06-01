# GNN-fb-friend-recommendation
Given Social circles (Facebook) Dataset Use Graph Neural Network To Build Friend Recommendation System

## Team Members:
Jinji SHEN: jinji.shen@student-cs.fr  
Mengyu LIANG: mengyu.liang@student-cs.fr  
Nhat Mai NGUYEN: nhatmai.nguyen@student-cs.fr  
Yanjie REN: yanjie.ren@student-cs.fr  
Taolue CHEN: taolue.chen@student-cs.fr

## Project Description
Friend recommendation is a key component for social media. This project defines the friend recommendation as a two-step problem that first predicts possible links among users using current social networks, and then selects k users with highest linking probability. 

The problem addressed in this project is to develop an efficient and accurate friend recommendation engine using Graph Neural Networks (GNN) on the Stanford Social Circle Facebook dataset. The goal of the system is to provide personalized and relevant friend recommendations to users of social media platforms, thus enhancing user engagement and retention. 

## Dataset
The dataset used in this project i.e. Social Circles (Facebook) dataset consists of 'circles' or 'friends lists' obtained from survey participants through a Facebook app. It includes node features (profiles), circles, and ego networks. To preserve user privacy, the Facebook-internal ids for each user have been replaced with new values, and the feature vectors have been obscured. For example, a feature like "political=Democratic Party" in the original dataset would be replaced with "political=anonymized feature 1" in the anonymized data. Therefore, while it is possible to determine if two users share the same political affiliations, the actual meaning of individual political affiliations cannot be inferred from the anonymized data.

The summary statistics of the dataset is as follows:

<img width="200" alt="image" src="https://github.com/SJinji/GNN-fb-friend-recommendation/assets/103330181/213d42ac-9591-4baf-b0dd-5f26cbb25796">

## Modeling
To build the Friend Recommendation System, this project designs 5 different architectures based on Graph Neuron Network(GNN), namely Graph Convolutional Networks (GCN), GraphSAGE, Graph Attention Networks (GAT), Graph Isomorphism Networks (GIN), and Deep Linker, which are popular and effective choices for learning node representations in graph data.

We also implemented hyperparameter tunings for GNN models to find the best combination of hyperparameters that produce the best performance for friend suggestions. The tuned hyperparameters are as follows:

<img width="330" alt="image" src="https://github.com/SJinji/GNN-fb-friend-recommendation/assets/103330181/b50e4260-940e-4266-a0b5-a27124dc59d2">


## Results
In classic GNN models, GCN is able to best distinguish negative and positive samples, while GAT achieves the highest accuracy score. Meanwhile, Deep Linker provides a state-of-the-art result for both accuracy and AUC score, suggesting its expertise in link prediction tasks.

<img width="613" alt="image" src="https://github.com/SJinji/GNN-fb-friend-recommendation/assets/103330181/bb925e3e-be92-4385-a854-56b9d7648c26">

