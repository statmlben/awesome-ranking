![GitHub](https://img.shields.io/badge/License-MIT-lightgrey.svg)

# Awesome Reference in Learning-to-Rank

This repository contains a curated list of awesome references for learning-to-rank.

## Tags

| | | |
|-|-|-|
| :golf: Methodology (METH) | :blue_book: Learning Theory (LT) | :dart: Optimization (OPT) | 
| :computer: Software (SW) | :duck: Kaggle Competition (Kaggle) | :keyboard: Empirical Studies (ES) |
| :bar_chart: Dataset (DATA) | :goal_net: Loss Function (Loss) | :globe_with_meridians: Deep Learning (DL) | 
| :arrows_counterclockwise: Ranking Aggregation or Synchronization (RA) |


## Reference

[DATA][ES] Chapelle, O., & Chang, Y. (2011, January). [Yahoo! learning to rank challenge overview](http://proceedings.mlr.press/v14/chapelle11a). In Proceedings of the learning to rank challenge (pp. 1-24). PMLR. 

- **keywords**: Yahoo dataset, query, document; [chapelle2011yahoo]
- **memo**: The paper provides overview of Yahoo Learning to Rank Challenge. Winning methods: LambdaMART boosted tree models, LambdaRank neural nets, LogitBoost, ... (most of them are boosting methods)

[METH][Loss][LT] Herbrich, R., Graepel, T., & Obermayer, K. (2000). [Large margin rank boundaries for ordinal regression](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Large+margin+rank+boundaries+for+ordinal+regression&btnG=). Advances in large margin classifiers, 88(2), 115-132.

- **keywords**: RankSVM, hinge loss, ordinal regression, pairwise approach, univariate scoring function; [herbrich2000large]
- **memo**: (i) formulation of RankSVM and ordinal regression with a univariate scoring function.

[METH][OPT] Freund, Y., Iyer, R., Schapire, R. E., & Singer, Y. (2003). [An efficient boosting algorithm for combining preferences](https://www.jmlr.org/papers/volume4/freund03a/freund03a.pdf). Journal of machine learning research, 4(Nov), 933-969.

- **keywords**: RankBoost, pairwise approach, univariate scoring function; [herbrich2000large]
- **memo**: (i) formulation of RankBoost under pairwise approach with a univariate scoring function. 


[METH][OPT][LT][Loss] Clémençon, S., Lugosi, G., & Vayatis, N. (2008). [Ranking and empirical minimization of U-statistics](https://projecteuclid.org/journals/annals-of-statistics/volume-36/issue-2/Ranking-and-Empirical-Minimization-of-U-statistics/10.1214/009052607000000910.full). The Annals of Statistics, 36(2), 844-874. 

- **keywords**: ranking, U-statistics, convex loss, pairwise, bivariate ranking function; [clemenccon2008ranking]
- **memo**: The paper formulates the ranking problem in a *pairwise classification* framework, consistency of empirical risk minimizers is established.

[METH][OPT] Burges, C., Shaked, T., Renshaw, E., Lazier, A., Deeds, M., Hamilton, N., & Hullender, G. (2005, August). (Learning to rank using gradient descent)[https://dl.acm.org/doi/pdf/10.1145/1102351.1102363?casa_token=j1eFCUL99SUAAAAA:LslBnjJ_iEXthdsANyIMBOooIlKo5ZO73bMi4YlFXnhoasIohj04IOghY7BRSc4QINzWS4nvrl92wA]. In Proceedings of the 22nd international conference on Machine learning (pp. 89-96).

- **keywords**: RankNet [burges2005learning]
- **memo**: RankNet is a pairwise probabilistic model based on the scoring approach: sigmoid function of difference between two scores.

[METH][OPT] Burges, C. J. (2010). (From ranknet to lambdarank to lambdamart: An overview)[https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.634&rep=rep1&type=pdf]. Learning, 11(23-581), 81.

- **keywords**: RankNet, LambdaRank, LambdaMART [burges2010ranknet]

[SW][DL][METH] Pasumarthi, R. K., Bruch, S., Wang, X., Li, C., Bendersky, M., Najork, M., ... & Wolf, S. (2019, July). [Tf-ranking: Scalable tensorflow library for learning-to-rank](https://dl.acm.org/doi/abs/10.1145/3292500.3330677). In Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining (pp. 2970-2978). [ [slides](https://github.com/tensorflow/ranking) + [GitHub](https://github.com/tensorflow/ranking) ] 

- **keywords**: neural learning-to-rank, handcrafted features; [pasumarthi2019tf]
- **memo**: Neural learning-to-rank software based on TensorFlow is developed, instead of learning with Handcrafted features (dense features), the proposed software is able to directly learn from textual data (sparse features).


[Loss][LT] Kotlowski, W., Dembczynski, K., & Huellermeier, E. (2011, January). [Bipartite ranking through minimization of univariate loss](https://icml.cc/2011/papers/567_icmlpaper.pdf). In ICML. 

- **keywords**: pairwise, consistency, scoring approach, bipartite ranking; [kotlowski2011bipartite]
- **memo**: (i) The paper points out the difference between *scoring approaches* and *ranking approaches* in learning-to-rank; (ii) the paper indicates that `log-loss` and `exp-loss` are consistent with `pairwise 0-1 loss` in ranking, yet the regret are upper bounded by square root (would reduce the convergence rate by half); 

[METH][Loss][LT] Narasimhan, H., & Agarwal, S. (2013, January). [On the Relationship Between Binary Classification, Bipartite Ranking, and Binary Class Probability Estimation](http://clweb.csa.iisc.ac.in/harikrishna/Papers/Classification-ranking-cpe/nips-13-relationship-classification-ranking-cpe.pdf). In NIPS (pp. 2913-2921). 

- **keywords**: pairwise, scoring approach, bipartite ranking, probability estimation; [narasimhan2013relationship]
- **memo**: The paper investigates the relation among `binary class probability estimation`, `binary classification`, and `bipartite ranking`. 


[Loss][LT][METH] Ravikumar, P., Tewari, A., & Yang, E. (2011, June). [On NDCG consistency of listwise ranking methods](http://proceedings.mlr.press/v15/ravikumar11a.html). In Proceedings of the Fourteenth International Conference on Artificial Intelligence and Statistics (pp. 618-626). JMLR Workshop and Conference Proceedings. 

- **keywords**: listwise, NDCG, Fisher-consistency; [ravikumar2011ndcg]
- **memo**: The paper investigates the Fisher-consistency (but not regret consistency) of NDCG. 

[Loss][LT][METH] Gao, W., & Zhou, Z. H. (2015, June). [On the consistency of AUC pairwise optimization](https://www.aaai.org/ocs/index.php/IJCAI/IJCAI15/paper/viewPDFInterstitial/11320/10793). In Twenty-Fourth International Joint Conference on Artificial Intelligence. 

- **keywords**: pairwise, zero-one loss, Fisher-consistency, consistency, AUC, Bipartite ranking; [gao2015consistency]
- **memo**: (i) AUC can be formulated by zero-one pairwise ranking problem; (ii) For ranking regret consistency, log loss (yes), exponential loss (yes), hinge loss (no), squared hinge loss (yes). (iii) convergence rate, log loss (square root of 0-1 loss), exponential loss (square root of 0-1 loss), hinge loss (no), squared hinge loss (??).

[JDSH][Loss][LT][METH] Dai, B., Shen, X., Wang, J., & Qu, A. (2019). [Scalable collaborative ranking for personalized prediction](https://doi.org/10.1080/01621459.2019.1691562). Journal of the American Statistical Association, 1-9. 

- **keywords**: pairwise, zero-one loss, Fisher-consistency, consistency, Bipartite ranking; [dai2019scalable]
- **memo**: (i) The regrets of MAP, DCG, Sum-Loss are all upper bounded by the pairwise 0-1 loss. That is, good performance in pairwise 0-1 loss imply good performance in all mentioned losses; (ii) convergence rate, truncated hinge loss (linear of 0-1 loss).

[RA][METH][LT] Fanuel, M., & Suykens, J. A. (2019). [Deformed Laplacians and spectral ranking in directed networks](https://arxiv.org/pdf/1511.00492.pdf). Applied and Computational Harmonic Analysis, 47(2), 397-422. 

- **keywords**: discrete laplacians, directed graphs, random walks, synchronization; [fanuel2019deformed]
- **memo**: (i) dilation Laplacians are shown to be useful tools for ranking in directed networks of pairwise comparisons; (ii) An eformation parameter enabling the emphasis of the top-k objects in the ranking.

[Loss][LT] Uematsu, K., & Lee, Y. (2017). [On theoretically optimal ranking functions in bipartite ranking](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.452.2387&rep=rep1&type=pdf). Journal of the American Statistical Association, 112(519), 1311-1322. 

- **keywords**: hinge loss, Bipartite ranking, negative example; [uematsu2017theoretically]
- **memo**: (i) Hinge loss is Fisher-consistency wrt pairwise zero-one loss in Bipartite ranking (Theorem 5).

[Loss][LT][METH][RA] Waegeman, W., Pahikkala, T., Airola, A., Salakoski, T., Stock, M., & De Baets, B. (2012). [A kernel-based framework for learning graded relations from data](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6179986). IEEE Transactions on Fuzzy Systems, 20(6), 1090-1101.

- **keywords**: kernel, synchronization, weak stochastic transitivity, linear stochastic transitivity, pairwise approach, bivariate ranking function; [waegeman2012kernel]
- **memo**: (i) a bivariate kernel presenting a sufficient condition of weak stochastic transitivity, the linear stochastic transitivity (LST; see Definition IV.3), in its associated reproducing kernel Hilbert space (RKHS).

[RA][METH][LT] Shah, N. B., & Wainwright, M. J. (2017). [Simple, robust and optimal ranking from pairwise comparisons](https://www.jmlr.org/papers/volume18/16-206/16-206.pdf). Journal of Machine Learning Research, 18(1), 7246-7283.

- **keywords**: pairwise approach, Borda counting; [shah2017simple]
- **memo**: (i) Borda counting based method to generate scores to all items based on pairwise comparison. (ii) define and analyze the difficulty of Top-k ranking for the proposed method.

[METH][LT] Chen, Y., Fan, J., Ma, C., & Wang, K. (2019). [Spectral method and regularized MLE are both optimal for top-K ranking](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6785035/). Annals of statistics, 47(4), 2204.

- **keywords**: top-K ranking; pairwise comparisons; spectral method; regularized MLE; entrywise perturbation; leave-one-out analysis; reversible Markov chains; [chen2019spectral]
- **memo**: scoring approach to ranking (model-based on (1.1)); minimax rate for ranking; gap assumption between top-k and top-(k+1).

[LT][Loss] Xia, F., Liu, T. Y., Wang, J., Zhang, W., & Li, H. (2008, July). Listwise approach to learning to rank: theory and algorithm. In Proceedings of the 25th international conference on Machine learning (pp. 1192-1199). 

- **keywords**: ranking loss; listwise; consistency; order sentitve; [xia2008listwise]
- **memo**: Ranking losses for listwise learning-to-rank, and their theoretical consistency.