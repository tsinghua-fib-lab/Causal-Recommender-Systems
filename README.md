# Causal-Recommender-Systems
An index of causal inference based recommendation algorithms.

Our survey **Causal Inference in Recommender Systems: A Survey and Future Directions** is available on arxiv: [link](https://arxiv.org/pdf/2208.12397.pdf)

Please cite our survey paper if this index is helpful.
```
@article{gao2021causal,
  title={Causal Inference in Recommender Systems: A Survey and Future Directions},
  author={Gao, Chen and Zheng, Yu and Wang, Wenjie and Feng, Fuli and He, Xiangnan and Li, Yong},
  journal={arXiv preprint arXiv:2208.12397},
  year={2022}
}
```
```
Gao, C., Zheng, Y., Wang, W., Feng, F., He, X., & Li, Y. (2022). Causal Inference in Recommender Systems: A Survey and Future Directions. arXiv preprint arXiv:2208.12397.
```

# Table of Contents

- [Causal Inference-based Recommendation for Addressing Data Bias](#Causal-Inference-based-Recommendation-for-Addressing-Data-Bias)
   - [Popularity Bias](#Popularity-Bias)
   - [Clickbait Bias, Bias Amplification, Conformity Bias](#Clickbait-Bias-Bias-Amplification-Conformity-Bias)
   - [Exposure Bias](#Exposure-Bias)
- [Causal Inference-based Recommendation for Addressing Data Missing and Noise](#Causal-Inference-based-Recommendation-for-Addressing-Data-Missing-and-Noise)
   - [Data Missing](#Data-Missing)
   - [Data Noise](#Data-Noise)
- [Beyond-accuracy RecSys with Causal Inference](#Beyond-accuracy-RecSys-with-Causal-Inference)
   - [Explainability](#Explainability)
   - [Diversity](#Diversity)
   - [Fairness](#Fairness)

## Causal Inference-based Recommendation for Addressing Data Bias
### Popularity Bias
| **Name** | **Paper** | **Causal Inference Method** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- | --- |
| PD | [Zhang, Y., Feng, F., He, X., Wei, T., Song, C., Ling, G., & Zhang, Y. (2021, July). Causal intervention for leveraging popularity bias in recommendation. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 11-20).](https://arxiv.org/pdf/2105.06067.pdf) | Backdoor Adjustment | SIGIR | 2021 | [Python/TF](https://github.com/zyang1580/PDA) |
| MACR | [Wei, T., Feng, F., Chen, J., Wu, Z., Yi, J., & He, X. (2021, August). Model-agnostic counterfactual reasoning for eliminating popularity bias in recommender system. In Proceedings of the 27th ACM SIGKDD Conference on Knowledge Discovery & Data Mining (pp. 1791-1800).](https://arxiv.org/pdf/2010.15363) | Counterfactual Inference | KDD | 2021 | [Python/TF](https://github.com/weitianxin/MACR) |

### Clickbait Bias, Bias Amplification, Conformity Bias
| **Name** | **Paper** | **Causal Inference Method** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- | --- |
| CR | [Wang, W., Feng, F., He, X., Zhang, H., & Chua, T. S. (2021, July). Clicks can be cheating: Counterfactual recommendation for mitigating clickbait issue. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 1288-1297).](https://arxiv.org/pdf/2009.09945) | Counterfactual Inference | SIGIR | 2021 | [Python/Torch](https://github.com/WenjieWWJ/Clickbait/) |
| DecRS | [Wang, W., Feng, F., He, X., Wang, X., & Chua, T. S. (2021, August). Deconfounded recommendation for alleviating bias amplification. In Proceedings of the 27th ACM SIGKDD Conference on Knowledge Discovery & Data Mining (pp. 1717-1725).](https://arxiv.org/pdf/2105.10648) | Backdoor Adjustment | KDD | 2021 | [Python/Torch](https://github.com/WenjieWWJ/DecRS) |
| DICE | [Zheng, Y., Gao, C., Li, X., He, X., Li, Y., & Jin, D. (2021, April). Disentangling user interest and conformity for recommendation with causal embedding. In Proceedings of the Web Conference 2021 (pp. 2980-2991).](https://arxiv.org/pdf/2006.11011) | Disentangled Causal Embeddings | WWW | 2021 | [Python/Torch](https://github.com/tsinghua-fib-lab/DICE) |

### Exposure Bias
| **Name** | **Paper** | **Causal Inference Method** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- | --- |
| IPS | [Schnabel, T., Swaminathan, A., Singh, A., Chandak, N., & Joachims, T. (2016, June). Recommendations as treatments: Debiasing learning and evaluation. In international conference on machine learning (pp. 1670-1679). PMLR.](https://arxiv.org/pdf/1602.05352) | IPW | ICML | 2016 | [Python](https://www.cs.cornell.edu/~schnabts/mnar/) |
| Rel-MF | [Saito, Y., Yaginuma, S., Nishino, Y., Sakata, H., & Nakata, K. (2020, January). Unbiased recommender learning from missing-not-at-random implicit feedback. In Proceedings of the 13th International Conference on Web Search and Data Mining (pp. 501-509).](https://arxiv.org/pdf/1909.03601) | IPW | WSDM | 2020 | [Python/TF](https://paperswithcode.com/paper/relevance-matrix-factorization) |
| Multi-IPW/DR | [Zhang, W., Bao, W., Liu, X. Y., Yang, K., Lin, Q., Wen, H., & Ramezani, R. (2020, April). Large-scale causal approaches to debiasing post-click conversion rate estimation with multi-task learning. In Proceedings of The Web Conference 2020 (pp. 2775-2781).](https://arxiv.org/pdf/1910.09337.pdf) | IPW, DR | WWW | 2020 | N/A |
| MF-DR-JL | [Wang, X., Zhang, R., Sun, Y., & Qi, J. (2019, May). Doubly robust joint learning for recommendation on data missing not at random. In International Conference on Machine Learning (pp. 6638-6647). PMLR.](http://proceedings.mlr.press/v97/wang19n/wang19n.pdf) | DR | ICML | 2019 |  N/A |
| DR | [Saito, Y. (2020, September). Doubly robust estimator for ranking metrics with post-click conversions. In Fourteenth ACM Conference on Recommender Systems (pp. 92-100).](https://usaito.github.io/files/RecSys2020_DRMetric.pdf) | DR | RecSys | 2020 | N/A |
| MRDR | [Guo, S., Zou, L., Liu, Y., Ye, W., Cheng, S., Wang, S., ... & Chang, Y. (2021, July). Enhanced doubly robust learning for debiasing post-click conversion rate estimation. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 275-284).](https://arxiv.org/pdf/2105.13623) | DR | SIGIR | 2021 | [Python/TF](https://github.com/guosyjlu/MRDR-DL) |
| LTD | [Wang, X., Zhang, R., Sun, Y., & Qi, J. (2021, March). Combating selection biases in recommender systems with a few unbiased ratings. In Proceedings of the 14th ACM International Conference on Web Search and Data Mining (pp. 427-435).](https://dl.acm.org/doi/10.1145/3437963.3441799) | RCT, DR | WSDM | 2021 | N/A |
| AutoDebias | [Chen, J., Dong, H., Qiu, Y., He, X., Xin, X., Chen, L., ... & Yang, K. (2021, July). AutoDebias: Learning to debias for recommendation. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 21-30).](https://arxiv.org/pdf/2105.04170) | RCT | SIGIR | 2021 | [Python/Torch](https://github.com/DongHande/AutoDebias) |
| USR | [Wang, Z., Shen, S., Wang, Z., Chen, B., Chen, X., & Wen, J. R. (2022, April). Unbiased Sequential Recommendation with Latent Confounders. In Proceedings of the ACM Web Conference 2022 (pp. 2195-2204).](https://dl.acm.org/doi/10.1145/3485447.3512092) | IPW | WWW | 2022 | N/A |
| InvPref | [Wang, Z., He, Y., Liu, J., Zou, W., Yu, P. S., & Cui, P. (2022, August). Invariant Preference Learning for General Debiasing in Recommendation. In Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (pp. 1969-1978).](https://dl.acm.org/doi/abs/10.1145/3534678.3539439) | Invariant Learning | KDD | 2022 | [Python/Torch](https://github.com/AIflowerQ/InvPref_KDD_2022) |

## Causal Inference-based Recommendation for Addressing Data Missing and Noise
### Data Missing
| **Name** | **Paper** | **RecSys Task** | **Causal Inference Method** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- | --- | --- |
| CauseRec | [Zhang, S., Yao, D., Zhao, Z., Chua, T. S., & Wu, F. (2021, July). Causerec: Counterfactual user sequence synthesis for sequential recommendation. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 367-377).](https://arxiv.org/pdf/2109.05261.pdf) | Sequential | Counterfactual | SIGIR | 2021 | N/A |
| CASR | [Wang, Z., Zhang, J., Xu, H., Chen, X., Zhang, Y., Zhao, W. X., & Wen, J. R. (2021, July). Counterfactual data-augmented sequential recommendation. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 347-356).](http://yongfeng.me/attach/wang-sigir2021.pdf) | Sequential | Counterfactual | SIGIR | 2021 | N/A |
| CF<sup>2</sup> | [Xiong, K., Ye, W., Chen, X., Zhang, Y., Zhao, W. X., Hu, B., ... & Zhou, J. (2021, October). Counterfactual Review-based Recommendation. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (pp. 2231-2240).](https://librahu.github.io/data/cikm2021-CFCF-paper.pdf) | Feature-based | Counterfactual | CIKM | 2021 | N/A |
| ASCKG-CG | [Mu, S., Li, Y., Zhao, W. X., Wang, J., Ding, B., & Wen, J. R. (2022, July). Alleviating Spurious Correlations in Knowledge-aware Recommendations through Counterfactual Generator. In Proceedings of the 45th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 1401-1411).](https://dl.acm.org/doi/abs/10.1145/3477495.3531934) | KG-based | Counterfactual | SIGIR | 2022 | [Python/Torch](https://github.com/RUCAIBox/CGKR) |
| CPR | [Yang, M., Dai, Q., Dong, Z., Chen, X., He, X., & Wang, J. (2021, October). Top-N Recommendation with Counterfactual User Preference Simulation. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (pp. 2342-2351).](https://arxiv.org/pdf/2109.02444.pdf) | Collaborative Filtering | SCM, Counterfactual | CIKM | 2021 | N/A |
| ULO | [Sato, M., Singh, J., Takemori, S., Sonoda, T., Zhang, Q., & Ohkuma, T. (2019, September). Uplift-based evaluation and optimization of recommenders. In Proceedings of the 13th ACM Conference on Recommender Systems (pp. 296-304).](https://dl.acm.org/doi/10.1145/3298689.3347018) | Collaborative Filtering | Uplift, IPW | RecSys | 2019 | N/A |
| DLCE | [Sato, M., Takemori, S., Singh, J., & Ohkuma, T. (2020, September). Unbiased learning for the causal effect of recommendation. In Fourteenth ACM Conference on Recommender Systems (pp. 378-387).](https://arxiv.org/pdf/2008.04563.pdf) | Collaborative Filtering | IPW | RecSys | 2020 | N/A |
| CBI | [Sato, M. (2021, September). Online Evaluation Methods for the Causal Effect of Recommendations. In Fifteenth ACM Conference on Recommender Systems (pp. 96-101).](https://arxiv.org/pdf/2107.06630.pdf) | Collaborative Filtering | Interleaving, IPW | RecSys | 2021 | [Python/R](https://github.com/masatoh73/causal-interleaving)
| CausCF | [Xie, X., Liu, Z., Wu, S., Sun, F., Liu, C., Chen, J., ... & Ding, B. (2021, October). CausCF: Causal Collaborative Filtering for Recommendation Effect Estimation. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (pp. 4253-4263).](https://arxiv.org/pdf/2105.13881.pdf) | Collaborative Filtering | Uplift, RDD | CIKM | 2021 | N/A |
| DRIB | [Xiao, T., & Wang, S. (2022, February). Towards unbiased and robust causal ranking for recommender systems. In Proceedings of the Fifteenth ACM International Conference on Web Search and Data Mining (pp. 1158-1167).](https://dl.acm.org/doi/abs/10.1145/3488560.3498521) | Collaborative Filtering | Doubly-Robust, IPW | WSDM | 2022 | N/A |
| COR | [Wang, W., Lin, X., Feng, F., He, X., Lin, M., & Chua, T. S. (2022, April). Causal Representation Learning for Out-of-Distribution Recommendation. In Proceedings of the ACM Web Conference 2022 (pp. 3562-3571).](http://staff.ustc.edu.cn/~hexn/papers/www22-ood-rec.pdf) | CTR | Counterfactual | WWW | 2022 | N/A |
| CausPref | [He, Y., Wang, Z., Cui, P., Zou, H., Zhang, Y., Cui, Q., & Jiang, Y. (2022, April). CausPref: Causal Preference Learning for Out-of-Distribution Recommendation. In Proceedings of the ACM Web Conference 2022 (pp. 410-421).](https://arxiv.org/pdf/2202.03984.pdf) | Collaborative Filtering | Invariant Learning | WWW | 2022 | [Python/Torch](https://github.com/HeYueThu/CausPref) |

### Data Noise
| **Name** | **Paper** | **RecSys Task** | **Causal Inference Method** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- | --- | --- |
| CBDF | [Zhang, X., Jia, H., Su, H., Wang, W., Xu, J., & Wen, J. R. (2021, July). Counterfactual reward modification for streaming recommendation with delayed feedback. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 41-50).](https://dl.acm.org/doi/abs/10.1145/3404835.3462892) | Streaming | Importance Sampling | SIGIR | 2021 | [Python](https://github.com/hnjia00/Delayed-Feedback) |

## Beyond-accuracy RecSys with Causal Inference
### Explainability
| **Name** | **Paper** | **RecSys Task** | **Causal Inference Method** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- | --- | --- |
| PGPR | [Xian, Y., Fu, Z., Muthukrishnan, S., De Melo, G., & Zhang, Y. (2019, July). Reinforcement knowledge graph reasoning for explainable recommendation. In Proceedings of the 42nd international ACM SIGIR conference on research and development in information retrieval (pp. 285-294).](https://arxiv.org/pdf/1906.05237) | KG-enhanced | Causal Discovery | SIGIR | 2019 | [Python/Torch](https://github.com/orcax/PGPR) |
| CountER | [Tan, J., Xu, S., Ge, Y., Li, Y., Chen, X., & Zhang, Y. (2021, October). Counterfactual explainable recommendation. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (pp. 1784-1793).](https://arxiv.org/pdf/2108.10539.pdf) | Collaborative Filtering | Counterfactual, Causal Discovery | CIKM | 2021 | [Python/Torch](https://github.com/chrisjtan/counter) |
| MCT | [Tran, H. X., Le, T. D., Li, J., Liu, L., Liu, J., Zhao, Y., & Waters, T. (2021, August). Recommending the Most Effective Intervention to Improve Employment for Job Seekers with Disability. In Proceedings of the 27th ACM SIGKDD Conference on Knowledge Discovery & Data Mining (pp. 3616-3626).](https://dl.acm.org/doi/abs/10.1145/3447548.3467095) | CTR | Couterfactual | KDD | 2021 | [Python/R](https://github.com/trxuanha/maximumcausaltree)
| CLSR | [Zheng, Y., Gao, C., Chang, J., Niu, Y., Song, Y., Jin, D., & Li, Y. (2022, April). Disentangling Long and Short-Term Interests for Recommendation. In Proceedings of the ACM Web Conference 2022 (pp. 2256-2267).](https://arxiv.org/pdf/2202.13090.pdf) | Sequential | Disentangled Embedding | WWW | 2022 | [Python/TF](https://github.com/tsinghua-fib-lab/CLSR) |
| IV4Rec | [Si, Z., Han, X., Zhang, X., Xu, J., Yin, Y., Song, Y., & Wen, J. R. (2022, April). A Model-Agnostic Causal Learning Framework for Recommendation using Search Data. In Proceedings of the ACM Web Conference 2022 (pp. 224-233).](https://arxiv.org/pdf/2202.04514.pdf) | CTR | Decomposed Embeddings | WWW | 2022 | [Python/Torch](https://github.com/ethan00si/instrumental-variables-for-recommendation) |

### Diversity
| **Name** | **Paper** | **RecSys Task** | **Causal Inference Method** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- | --- | --- |
| DecRS | [Wang, W., Feng, F., He, X., Wang, X., & Chua, T. S. (2021, August). Deconfounded recommendation for alleviating bias amplification. In Proceedings of the 27th ACM SIGKDD Conference on Knowledge Discovery & Data Mining (pp. 1717-1725).](https://arxiv.org/pdf/2105.10648) | Collaborative Filtering | Backdoor Adjustment | KDD | 2021 | [Python/Torch](https://github.com/WenjieWWJ/DecRS) |
| UCRS | [Wang, W., Feng, F., Nie, L., & Chua, T. S. (2022). User-controllable Recommendation Against Filter Bubbles. arXiv preprint arXiv:2204.13844.](https://dl.acm.org/doi/10.1145/3477495.3532075) | CTR | Counterfactual | SIGIR | 2022 | [Python/Torch](https://github.com/wenjiewwj/ucrs) |


### Fairness
| **Name** | **Paper** | **RecSys Task** | **Causal Inference Method** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- | --- | --- |
| CBDF | [Zhang, X., Jia, H., Su, H., Wang, W., Xu, J., & Wen, J. R. (2021, July). Counterfactual reward modification for streaming recommendation with delayed feedback. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 41-50).](https://dl.acm.org/doi/abs/10.1145/3404835.3462892) | Streaming | Importance Sampling | SIGIR | 2021 | [Python](https://github.com/hnjia00/Delayed-Feedback) |
