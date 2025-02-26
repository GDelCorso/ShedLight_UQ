# ShedLight_UQ - WIP

This git is going to contain the (Python) software and utilities to implement several types of intrusive/semi-intrusive/non-intrusive Bayesian probabilistic neural networks.

The code is provided with a large number of comments and remarks about toy problems in the**Notebook_Jupyter** folder.

Generated data are saved in **Data** folder.


# Jupyter tutorials
## Introduction
The introduction includes several examples of model implementations on vanilla PyTorch of classic and state-of-the-art deep learning models.
In particular, it contains an implementation of:
- **Start:** How to install a Pytorch (GPU acceleration) environment using anaconda on Windows.
- **Numerical Data:** Introduction to multiple synthetic data sets for classification and regression used in the following tutorials
- **Deterministic Models Regression:** Full implementation of a DL model for regression
- **Deterministic Models Regression:** Full implementation of a DL model for classification
- **Autoencoder Reconstruction:** Full implementation of a DL convolutional autoencoder model for image compression

*TO-DO-LIST:*
- Adaptive learning rates and early stopping criterion
- Save and upload a pytorch model
- Track epochs
- Define cross validation strategies
- Hyperparameter tuning and nested cross validaton strategies
- Freeze layers and fine-tuning
- Few shot learning
- Classical ML methods as particular case of ANNs
- Convolutions and convolutional ANNs

## Intrusive
Intrusive methods are the most efficient approaches to deal with aleatoric/epistemic uncertainties. However, they require careful implementation of appropriate loss/network characteristics.
- **Multi-head model regression:** Definition of a proper NLL derived loss (variance attenuation loss) and full implementation of a multi-head regression model to capture aleatoric uncertainty

*TO-DO-LIST:*
- Multi-head model classification
- Deep Gaussian Process
- Non-gaussian output - NLL derived lossess
- Bayesian Neural Network with KL divergence
- Fully-bayesian multi-head Neural Network
- Variational Autoencoder

## Semi-intrusive
Semi-intrusive methods combine the ease of use of post-hoc methods with the strength of intrusive methodologies.
- **Deep Ensemble Model Regression:** Pytorch implementation of a Deep Ensemble for regression. 

*TO-DO-LIST:*
- Deep Ensemble Model Classification
- Mixture of expert models
- POLPO-Net
- Few-shot trust score


## Post-hoc/non-intrusive
Post hoc methods (also called non-intrusive techniques) provide a simple and computationally efficient approximation of the predictive posterior distribution without requiring complex model modifications.
- **MC Dropout Classification:** Monte Carlo (MC) Dropout implementation to approximate epistemic uncertainties for classification tasks on 2D numerical data.

*TO-DO-LIST:*
- Trust Score
- MC Dropout Refression


# Probabilistic Deep Learning Package:
The code seen in the Jupyter tutorials will be wrapped in a useful package to do Bayesian Deep Learning and Probabilistic Modelling implementations.

**WIP**

# Related theoretical framework:
The theory related to the implemented code can be found in the paper: 

[Shedding light on uncertainties in machine learning](https://www.researchgate.net/publication/388256801_Shedding_light_on_uncertainties_in_machine_learning_formal_derivation_and_optimal_model_selection?utm_content=spotlight&utm_source=spotlightDetails&rgutm_meta1=SPL%3A679202aa4a4e592f920d4791&_tp=eyJjb250ZXh0Ijp7ImZpcnN0UGFnZSI6Il9kaXJlY3QiLCJwYWdlIjoicHJvZmlsZSJ9fQ)

## Citation:
To cite this work, please use:

@article{del2025shedding,

  title={Shedding light on uncertainties in machine learning: formal derivation and optimal model selection},
  
  author={Del Corso, Giulio and Colantonio, Sara and Caudai, Claudia},
  
  journal={Journal of the Franklin Institute},
  
  pages={107548},
  
  year={2025},
  
  publisher={Elsevier}
  
}
