![GitHub](https://img.shields.io/badge/License-MIT-lightgrey.svg)

# Awesome Reference in Learning-to-Rank

This repository contains a curated list of awesome references for learning-to-rank.

## Tags

| | | |
|-|-|-|
| :golf: Methodology (METH) | :blue_book: Learning Theory (LT) | :dart: Optimization (OPT) | 
| :computer: Software (SW) | :duck: Kaggle Competition (Kaggle) | :keyboard: Empirical Studies (ES) |
| :bar_chart: Dataset (DATA) | :goal_net: Loss Function (Loss) | :globe_with_meridians: Deep Learning (DL) | 
<!-- | :mag_right: Statistical Inference (INF) | :computer: Software (SW) | :unlock: Explainable AI (XAI) | 
| :cherries: Biostatistics (BIO) | :keyboard: Empirical Studies (ES) | :globe_with_meridians: Deep Learning (DL) | 
| :bar_chart: Dataset (DATA) | :arrow_right: Causal Inference (CI) | -->

## Must-Read-Refs

[DATA][ES] Chapelle, O., & Chang, Y. (2011, January). [Yahoo! learning to rank challenge overview](http://proceedings.mlr.press/v14/chapelle11a). In Proceedings of the learning to rank challenge (pp. 1-24). PMLR.

- **keywords**: Yahoo dataset, query, document
- **summary**: The paper provides overview of Yahoo Learning to Rank Challenge. Winning methods: LambdaMART boosted tree models, LambdaRank neural nets, LogitBoost, ... (most of them are boosting methods)


[METH][OPT][LT][Loss] Clémençon, S., Lugosi, G., & Vayatis, N. (2008). [Ranking and empirical minimization of U-statistics](https://projecteuclid.org/journals/annals-of-statistics/volume-36/issue-2/Ranking-and-Empirical-Minimization-of-U-statistics/10.1214/009052607000000910.full). The Annals of Statistics, 36(2), 844-874.

- **keywords**: ranking, U-statistics, convex loss, pairwise
- **summary**: The paper formulates the ranking problem in a *pairwise classification* framework, consistency of empirical risk minimizers is established.


## Reading

[Loss][LT] Kotlowski, W., Dembczynski, K., & Huellermeier, E. (2011, January). [Bipartite ranking through minimization of univariate loss](https://icml.cc/2011/papers/567_icmlpaper.pdf). In ICML.

- **keywords**: pairwise, consistency, scoring approach, bipartite ranking
- **summary**: (i) The paper points out the difference between *scoring approaches* and *ranking approaches* in learning-to-rank; (ii) the paper indicates that `log-loss` and `exp-loss` are consistent with `pairwise 0-1 loss` in ranking, yet the regret are upper bounded by square root (would reduce the convergence rate by half); 

[METH][Loss][LT] Narasimhan, H., & Agarwal, S. (2013, January). [On the Relationship Between Binary Classification, Bipartite Ranking, and Binary Class Probability Estimation](http://clweb.csa.iisc.ac.in/harikrishna/Papers/Classification-ranking-cpe/nips-13-relationship-classification-ranking-cpe.pdf). In NIPS (pp. 2913-2921).

- **keywords**: pairwise, scoring approach, bipartite ranking, probability estimation
- **summary**: The paper investigates the relation among `binary class probability estimation`, `binary classification`, and `bipartite ranking`. 


[Loss][LT][METH] Ravikumar, P., Tewari, A., & Yang, E. (2011, June). [On NDCG consistency of listwise ranking methods]. In Proceedings of the Fourteenth International Conference on Artificial Intelligence and Statistics (pp. 618-626). JMLR Workshop and Conference Proceedings.

- **keywords**: listwise, NDCG, Fisher-consistency
- **summary**: The paper investigates the Fisher-consistency (but not regret consistency) of NDCG. 
