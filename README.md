# Online Limited Memory Neural-Linear Bandits with Likelihood Matching #
<p align="center">
 <img src="scheme2.png" alt="alt text" width="512">
</p>

This library corresponds to the [Online Limited Memory Neural-Linear Bandits with Likelihood Matching](https://arxiv.org/abs/2102.03799) paper, ICML 2021.

The code is based on the "Deep Bayesian Bandits Showdown: An Empirical Comparison of Bayesian Deep Networks for Thompson Sampling" [github repository](https://github.com/tensorflow/models/tree/archive/research/deep_contextual_bandits).

### Datasets ###

All the datasets can be found in [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php), and should be placed under  contextual_bandtis/datasets folder. 

### How to run the code? ###
Run at terminal:
```
 python3 main.py 
```
### How to configure the experiment? ###
At the main.py, set the method into:
1. neural-linear-lm (Our method)
2. neural-linear (full memory NeuralTS)
3. linear (LinearTS)
4. neural-linear-ntk (NTK version of limited memory NeuralTS)

At dataset sepcify the wanted dataset (an unknown dataset will cause an error).
For amazon dataset, LinearTS do not work. 

### Requirements ###

* tensorflow-gpu 1.15
* absl-py 0.11
* scipy 1.5.4

