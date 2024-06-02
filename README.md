# Towards Sobolev Pruning

This repo collects relevant links for the paper: **Towards Sobolev Pruning** published in the Proceedings of PASC '24.

## Paper

https://doi.org/10.1145/3659914.3659915

## Code

The main code is written using [JAX](https://github.com/google/jax) and is currently located in [here](https://github.com/neilkichler/diff-ml/tree/main/notebooks/pruning).

## Citation

```bibtex
@inproceedings{kichler2024sobolevpruning,
author = {Kichler, Neil and Afghan, Sher and Naumann, Uwe},
title = {Towards Sobolev Pruning},
year = {2024},
isbn = {9798400706394},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3659914.3659915},
doi = {10.1145/3659914.3659915},
abstract = {The increasing use of stochastic models for describing complex phenomena warrants surrogate models that capture the reference model characteristics at a fraction of the computational cost, foregoing the potentially expensive Monte Carlo simulation. The predominant approach of fitting a large neural network and then pruning it to a reduced size has commonly neglected shortcomings. The produced surrogate models often will not capture the sensitivities and uncertainties inherent in the original model. In particular, the (higher-order) derivative information of such surrogates could differ drastically. Given a large enough network, we expect this derivative information to match. However, the pruned model will almost certainly not share this behaviour.In this paper, we propose to find surrogate models by using sensitivity information throughout the learning and pruning process. We build on work using Interval Adjoint Significance Analysis for pruning and combine it with the recent advancements in Sobolev Training to accurately model the original sensitivity information in the pruned neural network based surrogate model. We experimentally underpin the method on an example of pricing a multidimensional Basket option modelled through a stochastic differential equation with Brownian motion. The proposed method is, however, not limited to the domain of quantitative finance, which was chosen as a case study for intuitive interpretations of the sensitivities. It serves as a foundation for building further surrogate modelling techniques considering sensitivity information.},
booktitle = {Proceedings of the Platform for Advanced Scientific Computing Conference},
articleno = {1},
numpages = {11},
keywords = {surrogate modelling, model distillation, interval arithmetic, interval adjoint significance analysis, pruning, sobolev training, algorithmic differentiation, machine learning},
location = {<conf-loc>, <city>Zurich</city>, <country>Switzerland</country>, </conf-loc>},
series = {PASC '24}
}
```
