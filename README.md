# Evaluate effects of different kind of prior knowledge in causal structure learning from data
## The proposed project
The goal of this project is to examine on how the prior knowledge affect the result of learning causal structure from a given dataset. In specific, the incorrect edges are added to the blacklist and white list as prior knowledge for the examination of the result.

> Experiments are performed to understand the relationship between informativeness of the prior and dataset sample size. From the survey of the previous works, one consistent finding was that if prior beliefs are closer to the true model, then they improve the learning process but if priors are misleading or incorrect, they harm the learning process. The thought is to further understand this phenomenon by doing various experiments which systematically vary dataset size and prior correctness. The project will also focus on understanding the relationship between how complicated the prior is (expressiveness of prior e.g. edge orientation vs path) and learning accuracy.

> - Vary the correctness of the prior provided by the user of the algorithm and run algorithm for fixed dataset size. This can be done by providing arguments to the structure learning algorithm in the form of blacklists and whitelists.
> - Vary the size of the dataset and keep the correctness of the prior fixed. 



## Dataset
The project mainly used the [*alarm*](https://www.bnlearn.com/documentation/man/alarm.html) Dataset.

## The ground truth Causal Structure
![ground_truth_dag](figures/alarm_ground_truth_dag.png)

## Learn a causal structure
F1 score is used as the scorer function to compare the learned network with ground truth

## Figures
![F1 score given 1 incorrect blacklist edge](figures/blacklist_1_f1.png)
![F1 score given n random incorrect blacklist edge](figures/blacklist_n_f1.png)
![F1 score given 1 correct whitelist edge](figures/whitelist_c1_f1.png)
![F1 score given n random correct whitelist edge](figures/whitelist_cn_f1.png)
![F1 score given 20 random incorrect blacklist edge](figures/blacklist_size_20_f1.png)
