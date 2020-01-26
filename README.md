[![HitCount](http://hits.dwyl.io/LCS2-IIITD/TIST-2019-DiffQue.svg)](http://hits.dwyl.io/LCS2-IIITD/TIST-2019-DiffQue)

# DiffQue: Estimating Relative Difficulty of Questions in Community Question Answering Services

This is the code of the paper accepted at [ACM Transactions on Intelligent Systems and Technology (TIST)](https://tist.acm.org/).

## Motivation
![Alt text](Images/moti.png?raw=true "Title")

A toy example showing how DiffQue can be utilised in different scenarios: (a) Question Routing: Experts are presented with tougher questions as opposed to amateurs to save time and speed of the respective users; (b) Incentive Mechanism:  If a user answers a tougher question, he should be provided more incentive in terms of reputation in the system.

## Abstract
Automatic estimation of relative difficulty of a pair of questions is an important and challenging problem in community question answering (CQA) services. There are limited studies which addressed this problem. Past studies mostly leveraged expertise of users answering the questions and barely considered other properties of CQA services such as metadata of users and posts, temporal information and textual content.  

In this paper,  we propose DiffQue, a novel system that maps this problem to a network-aided edge directionality prediction problem. DiffQue starts by constructing a novel network structure that captures different notions of difficulties among a pair of questions. It then measures the relative difficulty of two questions by predicting the direction of a (virtual) edge connecting these two questions in the network.  It leverages features extracted from the network structure, metadata of users/posts and textual description of questions and answers. Experiments on datasets obtained from two CQA sites (further divided into four datasets) with human annotated ground-truth show that DiffQue outperforms four state-of-the-art methods by a significant margin (28.77\% higher F1 score and 28.72\% higher AUC than the best baseline). 

As opposed to the other baselines,  
(i) DiffQue appropriately responds to the training noise,  
(ii) DiffQue is capable of adapting multiple domains (CQA datasets), and  
(iii) DiffQue can efficiently handle cold start problem which may arise due to the lack of information for newly posted questions or newly arrived users.  