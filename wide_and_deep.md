- **Generalized linear models with nonlinear feature transformations**
- memorization of feature interactions are **effective and interpretable**, while **generalization** requires more **feature engineering**
- Deep learning can generalize better to unseen feature combinations through low-dimensional dense embedding learned for the sparse features with less feature engineering
- However deep neural networks with embeddings can over-generalize and recommend less relevant items when the user-item interactions are sparse and high-rank
- Jointly trained wide linear models and deep neural networks (This is why we call this model 'wide and deep')

* Generalized linear models such as logistic regression (often trained on binarized sparse features with one-hot encoding)
* Generalization can be added by using features that are less **granular** (require manual feature engineering)


It is difficult to learn effective low-dimensional presentations for queries and items when the underlying query-item matrix is sparse and high-rank, such as users with specific preferences or niche items with a narrow appeal. In such case, there should be no interactions between most query-item pairs, but dense embeddings will lead to nonzero predictions for all query-item pairs, and thus can over-generalize and make less  relevant recommendations. On the other hand, linear model with cross-product feature transformations can memorize these "exception rules" with much fewer parameters.
使用embedding这样的低维表示难以·学到稀疏的query-item交互矩阵, 在这种情况下, 大多数的query-item之间应该没有交互, 但是稠密的embedding表示会使得对于所有的query-item之间有非零的结果预测, 这样就会导致过度的泛化并且会导致推荐不相关的物品, 另一方面, 使用cross-product这样的特征转换的线性模型更能够使用少量参数记住这些异常规则.