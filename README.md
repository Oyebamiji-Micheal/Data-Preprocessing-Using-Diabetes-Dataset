# Data Preprocessing

<p align='justify'>
This repository aims to provide an understanding of common data preprocessing techniques, such as data rescaling, which include data standardization, normalization, etc., and when to use them.
</p>

## Normalization
<p align='justify'>
Normalization is a technique used to rescale numeric variables to a common range of values, typically between 0 and 1. This technique is useful when the scale of the variables varies widely, and we want to compare variables on equal footing. The formula for normalization is:

```
X_normalized = (X - X_min) / (X_max - X_min)
```

Normalization is particularly useful when the data has a varying scale, and the algorithms used do not make assumptions about the distribution of the data, such as k-nearest neighbors and artificial neural networks.
</p>

## Standardization

<p align='justify'>
Standardization, on the other hand, is a technique used to rescale variables to have a mean of 0 and a standard deviation of 1. This technique is useful when comparing variables that have different units or scales. The formula for standardization is:

```
X_standardized = (X - mean(X)) / std(X)
```

Standardization is also useful when using algorithms that assume normally distributed data, such as linear regression, logistic regression, or neural networks.


In general, datasets that are out of scale need to be rescaled before algorithms which involve measuring distance or gradient descent are applied to them. However, datasets which will be trained using algorithms such as decision trees, random forest, XGBoost, and others need not be rescaled.

</p>


## Reference Materials
- [How, When, and Why Should You Normalize / Standardize / Rescale Your Data? - TowardsAI](https://towardsai.net/p/data-science/how-when-and-why-should-you-normalize-standardize-rescale-your-data-3f083def38ff)
