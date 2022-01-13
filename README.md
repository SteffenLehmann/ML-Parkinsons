# Parkinson's disease Mini-project

### Steffen Lehmann


## Parkinson's disease Mini-project

22 features

Status:

```
● (one) - Parkinson's
● (zero) - Healthy
```
A detection problem


## Feature selection - Correlation check
![image info](./images/image.png)
Removed labels + names

Removed > 0.9 correlated
features

Top down approach

11 features


## Standardizing the data

z = (x - u) / s

u = mean of the samples
s = SD of the samples


## Normality check and distributions

MDVP:Fhi(Hz) - Maximum vocal fundamental frequency
has outliers

Shapiro-Wilk test of normality

Means and Covariance


## Dimensionality reduction: PCA - unsupervised

Before removing > 0.9 correlated
features

Features = 22


## Dimensionality reduction: PCA - unsupervised

After removing > 0.9 correlated
features

Features = 11


## Dimensionality reduction: PCA - unsupervised

After removing > 0.9 correlated
features

Features = 11

Retained 0.95 of the variance

7 PCs


## Principal Component Analysis - unsupervised

```
● N is the number of scores in each set of data
● X, Y are the mean of the N in the each data set
● X i, Y i are the raw observation in each set
● x i, y i is the i th deviation score in each set
```
Covariance Matrix

```
Variance
```

## Principal Component Analysis

Covariance Matrix

A = covariance matrix

v = eigenvector

λ = scaler (EigenValues)

I = identity matrix


## Principal Component Analysis

Covariance Matrix

EigenValues

EigenVector


## Principal Component Analysis

The most important features
in the covariance matrix

Biggest contributors to
eigenvalue (scaler)


## Detection Problem using supervised methods

K fold (interactions): 5

80/20 split

```
● Gaussian naive bayes
● Support vector Machine
● Random forest
● Neural network
```
On 11 and 7 features


## Gaussian Naive Bayes

Priors

```
● 0.25 for Healthy
● 0.75 for Parkinson’s
```
Variance and mean

```
● P(h): the probability of hypothesis h being true
(regardless of the data). This is known as the
prior probability of h.
● P(D): the probability of the data (regardless of
the hypothesis). This is known as the evidence.
● P(h|D): the probability of hypothesis h given
the data D. This is known as posterior
probability.
● P(D|h): the probability of data d given that the
hypothesis h was true. This is known as
posterior probability.
```


## Support Vector Machine Classifier - Supervised

Cn= Parkinson’s and healthy

Not the actual model


## Support Vector Machine Classifier - Supervised

Cn= Parkinson’s and healthy

Not the actual model

Margins


## Was the sample Healthy or not?

## The SVM model

T threshold

FP better than FN?

```
TP
```
```
FN
```
```
FP
```
```
TN
```
## Park

## Healthy

## Healthy

## Park


## Healthy Parkinson’s

## Was the sample Healthy or not?

● Recall
● Precision
● Accurarry



## Accuracy scores

Worse accuracy with 22 features

```
SVC RFC NN GNB
Standard (11) 82% (0.06) 79% (0.07) 79% (0.02) 74 % (0.05)
PCA (7) 80% (0.06) 83% (0.08) 81% (0.04) 77% (0.03)
```

