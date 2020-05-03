# NYU // AI // Project 03 // CodeSearchNet

This is an extension of the [CodeSearchNet](https://app.wandb.ai/github/codesearchnet/benchmark) competition. 

## A brief overview of the project
[CodeSearchNet](https://arxiv.org/abs/1909.09436)  is a collection of datasets and benchmarks that explore the problem of code retrieval using natural language. This research is a continuation of some ideas presented in this  [blog post](https://githubengineering.com/towards-natural-language-semantic-code-search/)  and is a joint collaboration between GitHub and the  [Deep Program Understanding](https://www.microsoft.com/en-us/research/project/program/)  group at  [Microsoft Research - Cambridge](https://www.microsoft.com/en-us/research/lab/microsoft-research-cambridge/). We aim to provide a platform for community research on semantic code search via the following:

1.  Instructions for obtaining large corpora of relevant data
2.  Open source code for a range of baseline models, along with pre-trained weights
3.  Baseline evaluation metrics and utilities
4.  Mechanisms to track progress on a  [shared community benchmark](https://app.wandb.ai/github/CodeSearchNet/benchmark)  hosted by  [Weights & Biases](https://www.wandb.com/)

We hope that CodeSearchNet is a step towards engaging with the broader machine learning and NLP community regarding the relationship between source code and natural language. We describe a specific task here, but we expect and welcome other uses of our dataset.

More context regarding the motivation for this problem is in this  [technical report](https://arxiv.org/abs/1909.09436).

## Intended Structure of documentation
1. Discuss BoW generally
2. Discuss BoW NN
3. Discuss BoW implementation in CodeSearchNet

4. Go into how the testing is done, metrics used, methodology. 
	a. How is testing is done?
	b. What is MRR, why does MRR need to be used here
	c. Discuss why leaderboard uses NDCG .


## 1. Some Notes on Bag of Words Model
* [https://machinelearningmastery.com/deep-learning-bag-of-words-model-sentiment-analysis/](https://machinelearningmastery.com/deep-learning-bag-of-words-model-sentiment-analysis/) This is a good article discussing generally what BoW is. 
* It really isn't a NN structure per say, it is a feature engineering pre processing step (BoW) that is then fed into a neural net. 
* The purpose of Bag of Words is to represent written sentences and phr



## I need to discuss what exactly is being tested.
* Really unsure right now.
* [https://arxiv.org/pdf/1909.09436.pdf](https://arxiv.org/pdf/1909.09436.pdf) This is a paper regarding the project in general, might offer some good insight. 
* Ok so testing is interesting. The test set consists of 99 queries. For each query, we are given 1000 code snippets. Of the 1000 code snippets, only one is relevant and 999 are distractors, so the evaluation task is to rank them.  

## I'm going to need to discuss MRR and the other evaluation metrics used. I think this resource will be good. 
[https://medium.com/swlh/rank-aware-recsys-evaluation-metrics-5191bba16832](https://medium.com/swlh/rank-aware-recsys-evaluation-metrics-5191bba16832)
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTM1Mzg1ODEzNSwxOTgzMzczODk5LC0xNj
k1NDkwMTA3LC0zMzMyNTQ4OTIsLTE1NDI3MzgyOTQsLTcxNjc2
NjQ1NiwtMTM3MDc3MDk2NywxNzAwOTEwMDg4LC02NjYxNzY1ND
UsLTIwMjMzODE4ODVdfQ==
-->