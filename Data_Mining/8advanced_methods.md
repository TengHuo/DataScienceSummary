# Advanced Methods

## Advanced Methods for Classification and Regression

### 1. Ensemble Methods

**Ensemble methods** combine predictions from **multiple classifiers** using some type of function, such as a weighted average of their predictions.

- **Statistical reasons**: each classifier produces an hypothesis, $h_i$ , about the data. The average over all the hi ’s is better than any of them alone.
- **Computational reasons**: learning methods use techniques like gradient descent and can get stuck in local optima. Multiple searchers would be less likely to all end up in the same local optima.
- **Representional reasons**: each classifier can only represent some aspects of the true hypothesis. By combining representations from multiple classifiers, we represent more aspects.

#### 1. Bayesian voting

Given data point x and training data D, the problem of computing our hypothesis f (x) is the problem of computing:
$$
Pr(f(x) = y|D,x)
$$

which can be computed as a weighted sum over all the hypotheses:
$$
PR(f(x) = y|D,x) = \sum_{h\in H}h(x)Pr(h|D)
$$

#### 2. Bagging (or Bootstrap Aggregation)

In each training run, a sample of m < M instances are drawn from the full training set (of size M), with **replacement**. The training set is called a bootstrap replicate of the original training set.

The method helps improve results when a learning algorithm is **not very stable** and is sensitive to **small variations in the training data**.

#### 3. Boosting

This works like **Bagging**. But also maintains a set of weights over the training examples.

### 2. Kernel Methods

**Kernel methods** means **transforming data into another dimension** that has a clear dividing margin between classes of data (classification), or **smoothing out** the contribution of a single observation over a local neighbourhood (regression).

A **parametric** model is appropriate if we make assumptions about the distribution of the **population** from which the data set (considered a **sample** or subset of the population) is drawn.

A **non-parametric** model is needed if we cannot make any assumptions about how the data is distributed.

#### Support-vector Machine (SVM)




## Advanced Methods for Sequence Analysis

### 1. Hidden Models

When there is no direct correlation between variables, then it is possible that **hidden** or **latent** variables may exist.

### 2. HMMs (Hidden Markov Models)

A **Markov chain** is a common model where all information relevant to $x_i$ is contained in $x_{i−1}$.

## Mehods for Dimensionality Reduction

### 1. Feature Extraction

Reduce multiple related observations (instances) to one observation. But this can result in a loss of information, possibly crucial information.

### 2. Derving Variables

1. Single-variable transformations
  1. **Standardise** numeric variables: 1. **Centering**, 2. **Rescaling**
  2. Turn. numerica values into percetiles
  3. Turn absolute numbers into relative measures
  4. Turn counts into rates
  5. Replace categorical variables with numeric variables
2. Combining variables
3. Extracting features from ...
4. Handling sparse data

### 3. Reducing Variables

1. Variable selection
2. Variable transformation: Looking for $\chi'$ where $|\chi'| \ll |\chi|$
  1. Projection Pursuit Regression
  2. Principal Components Analysis (PCA)
  3. Singular-Value Decomposition (SVD)
  4. Latent Semantic Indexing (LSI)
3. Variable clustering
















