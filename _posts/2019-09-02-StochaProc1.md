---
title: 'Stochastic Process Lecture 1'
date: 2019-09-03
permalink: /posts/2019/09/blog-post-1/
tags:
  - course note
  - stochastic process
---

# Lecture 1

Terms
1. axioms: 
2. lemma: 
3. moment
4. corollaries: a proposition (see proposition entry 1 sense 1c) inferred immediately from a proved proposition with little or no additional proof.

## 1. Basic Probability
### Random Experiments
$\Omega$ : sample space
$\mathrm{F}$ : the collection of all events: event: a subset of $\Omega$
$\mathrm{P}$: thr probability of these events

### Sigma fields
1. A collection of subsets, $F$, forms a **field** if 
   1. null set $\phi$, the universal set $\Omega$ belongs to $F$
   2. closed to union and intersect
   3. If $A \in F,$ then $A^{c} \in F$ (complement set)
1. **sigma field**
   1. satisfied above
   2. closed under **countably infinite** (e.g. nature numbers)???

### Axiomatic Approach to Probability
> A probability law is defined with 3 Axioms, ==p4==


```c++
qqq
include <iostream>
```

### Probability Laws = Models

==p7==

### Conditional Probability
*conditional probability*: $P[A | B]=\frac{P[A \cap B]}{P[B]}$
$\mathrm{P}[\mathrm{A}]$ is called the ==*a priori*== probability
$\mathrm{P}[\mathrm{A} | \mathrm{B}]$ is called the ==*a posteriori*== probability

### Uses of the Conditional Probability
- Product Rule
	i.e. the definition of cond. prob 
	
- Total Probability Theorem
$$
P[A]=\sum_{i=1}^{n} P\left[A | B_{i}\right] P\left[B_{i}\right]
$$
if $\mathrm{B}_{1}, \mathrm{B}_{2}, \mathrm{B}_{3}, \ldots ., \mathrm{B}_{\mathrm{n}}$ are **disjoint** (partition of the sample space)

- Bayes Theorem: 

  $P[A | B]\cdot P[B]=P[B|A]\cdot P[A]$
$$
P[B_j|A] = \frac{P[A | B_j]\cdot P[B]}{\sum_{j=1}^{n} P\left[A | B_{j}\right]}
$$

example: ==P13, 16, 18==

### Independence of Events
$P[A B]=P[A]\cdot P[B]$
​	i.e. a posteriori = a priori
3 events' independence need 2 requirements: pairwise, joint 

## 2. Random Variables

***random variable* $X$** : is a function that assign a number to every *outcome*, the function is fixed and deterministic. 
> It maps the outcome of a random exp to a number in a fixed way
e.g.==p24==

### Formal Definition of a Random Variable

==p25, p26==???
==p29==

### Cumulative distribution function (CDF)
$F_{X}(x)=P[X \leq x] \quad$ for $-\infty<x<\infty$

### Characteristic Functions
$\Phi(\omega)=\int_{-\infty}^{\infty} f(x) e^{j \omega x} d x$ 

Fourier TF of Density Function. Usually used as a theorem proving device

### Probability Density Function (PDF)
$$
f_{X}(x)=\frac{d F(x)}{d x}=\lim _{h \rightarrow 0} \frac{F(x+h)-F(x)}{h}
$$
e.g. Gaussian Random Variable
$$
p(x)=\frac{1}{\sqrt{2 \pi} \sigma} e^{\frac{-(x-m)^{2}}{2 \sigma^{2}}}
$$

### Probability Mass Function (pmf)
$p(k)=P[X=k]$, for discrete random variables
e.g. Bernoulli Random Variable p37

### Expectation
$$
E[X]=\int_{-\infty}^{+\infty} x p(x) d x \quad \text{or} \quad E[X]=\sum_{k} k \cdot p(k)
$$

- denoted as $\eta, \mu$ or $m$
- defined only if the result is convergent

### Fundamental Theorem of the Expectation
- \* given a RV $X$ and a function $Y=g(X)$, expection can be written as:

  $E[Y]=\int_{-\infty}^{\infty} g(x) f_{X}(x) d x \quad$ or $\quad E[Y]=\sum_{k} g(k) p_{X}(k)$

  ==why?==: try from definition of Expectation

### Linearity of the Expectation

1. $E[aX+b]=aE[X]+b$
2. $E\left[\sum_{i} a_{i} g_{i}(X)\right]=\sum_{i} a_{i} E[g_i(X)]$

### Variance & properties

==p46==

### Moments

==p49==

### MMSE

==p50, p51==

## 3. Multiple Random Variables

### To be cont'd independence

| sad    | dsasd | ddsa |
| ------ | ----- | ---- |
| dsasdd | sadsa | dsas |
|        |       |      |
|        |       |      |
sdsdsd
|      |      |      |
| ---- | ---- | ---- |
|      |      |      |
|      |      |      |
|      |      |      |

