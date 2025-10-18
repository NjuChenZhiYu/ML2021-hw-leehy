# Hong Yi Li's 2021 Machine Learning Homework Ideas

## Homework Code Update Overview
- **HW01**: Added related code for Adam, Momentum, Normalization, L2 regularization, Feature selection, K-fold cross-validation, etc., and used the Optuna library for automatic hyperparameter search.
- **HW02**: Fixed minor bugs in the original code, added TensorBoard and scheduler usage. The default execution is the strong baseline. You can check the TODO options in the code to achieve the Boss baseline (using BiLSTM).
- **HW03**: The code is divided into three parts (Medium, Strong, ) based on the baseline, making it easier for everyone to view. Future code will follow this structure. The code is only trained based on the sample code infrastructure and has not reached the Boss baseline. Currently, the score is 0.85200. This is shared as a reference, and a follow-up on the Boss baseline will be done later.
- **HW04**:
  - **Medium**: Modified the transformer module parameters after searching through dozens of parameter combinations with grid search.
  - **Strong**: Based on Medium, changed the architecture to use the ConformerBlock from the Conformer paper.
  - **Boss**: Added Self-Attention Pooling and Additive Margin Softmax modules as described in hints. In practice, simply changing the pred_layer in the Classifier part of Strong to a single fully-connected layer, just like the Conformer itself, can easily achieve the Boss baseline.
- **HW05**:
  - **Medium**: Increased the learning rate scheduler and extended training duration.
  - **Strong**: Transformed the model architecture into a Transformer and adjusted hyperparameters based on [Attention is All You Need](https://arxiv.org/abs/1706.03762).
  - **Boss**: Applied back-translation.

