---
tags:
- Matrizen
flashcard: false
source: "Übung 5"
date created: 2024-05-17
types: 
examples: 
- "[[Einheitsmatrix]]"
- "[[Nullmatrix]]"
constructions: 
generalizations: 
justifications:
---
***
#### Matrizen

Sei $(R, \oplus, \odot)$ ein kommutativer Ring mit $1$ und $n,m \in \mathbb{N}$.

$$
A = [a_{ij}] = \begin{bmatrix}
a_{11} & a_{12} & a_{13} & \dots & a_{1m} \\
a_{21} & a_{22} & a_{23} & \dots & a_{2m} \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
a_{n1} & a_{n2} & a_{n3} & \dots & a_{nm}
\end{bmatrix}
$$

***
#### Rechenoperationen

- $+: R^{n,m} \times R^{n,m} \longrightarrow R^{n,m}$, somit gilt $A + B = [a_{ij} + b_{ij}]$
- ${} \star : R^{n,l} \times R^{l, m} \longrightarrow R^{n,m} {}$, somit gilt $AB = \left[ \sum_{k = 1}^{l}a_{ik}b_{kj} \right]$
- $\cdot : R \times R^{n,m} \longrightarrow R^{n,m}$, so dass gilt $\lambda A = [\lambda a_{ij}]$
- $\cdot^{\top} : R^{n,m} \longrightarrow R^{m,n}$, also gilt $A^{\top} = [a_{ji}]$

***
#### Blockmatrizen

> [!definition] Blockmatrix
> Seien $A_{11}, A_{12}, A_{21}, A_{22}$ Matrizen ${} A_{ij} \in R^{ni,mj}, \quad i,j = 1,2, \quad n_{1},n_{2},m_{1},m_{2} \in \mathbb{N} {}$
> 
> $$
> A =
\begin{bmatrix}
A_{11} & A_{12} \\
A_{21} & A_{22}
\end{bmatrix}
\coloneqq
\begin{bmatrix}
a_{11} & \ldots & a_{1m_{1}} & a_{11} & \ldots & a_{1m_{2}} \\
\vdots & \ddots & \vdots & \vdots & \ddots & \vdots \\
a_{n_{1}1} & \ldots & a_{n_{1}m_{1}} & a_{n_{1}1} & \ldots & a_{n_{1}m_{2}} \\
a_{11} & \ldots & a_{1m_{1}} & a_{11} & \ldots & a_{1m_{2}} \\
\vdots & \ddots & \vdots & \vdots & \ddots & \vdots \\
a_{n_{2}1} & \ldots & a_{n_{2}m_{1}} & a_{n_{2}1} & \ldots & a_{n_{2}m_{2}}
\end{bmatrix}
> $$
> 
> Allgemein gilt $A_{ij} \in R^{n_{i}m_{j}}, \quad i = 1, \ldots, k, \; j = 1, \ldots, l$, also
> 
> $$
> A =
\begin{bmatrix}
A_{11} & \ldots & A_{1l} \\
\vdots & \ddots & \vdots \\
A_{k1} & \ldots & A_{kl}
\end{bmatrix}
> $$

**Spezialfälle**:

1. $k = 1, l = m \in \mathbb{N}$ und $n_{1} = n \in \mathbb{N}, mj = 1$

$$
A =
\begin{bmatrix}
A_{11} & \ldots & A_{1m}
\end{bmatrix}
=
\begin{bmatrix}
a_{1} & \ldots & a_{m}
\end{bmatrix}
$$

2. $k = n$, ...

