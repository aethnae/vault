---
tags:
  - Binominalkoeffizienten
  - Induktion
flashcard: false
source: Skript p. 6
date created: 2024-07-09
types: 
examples: 
constructions:
  - "[[Binomischer Lehrsatz]]"
generalizations: 
justifications:
---
***
#### Binominalkoeffizient

> [!definition] Binominalkoeffizient
> Für $n,k \in \mathbb{N}, n \geq 1, n \geq k$ heißt
> 
> $$
> \binom{n}{k}:=\frac{n!}{k!(n-k)!}
> $$
> 
> *Binominalkoeffizient* $n$ über $k$. Falls $n < k$ oder $k < 0$ sei
> 
> $$
> \binom{n}{k} \coloneqq 0
> $$
> 
> definiert.

***

> [!lemma] Zerlegung des Binominalkoeffizienten
> Für $n \in \mathbb{N}, n \geq 1$ und $k \in \mathbb{N}, k \leq n$ gilt
> 
> $$
> \binom{n}{k} = \binom{n-1}{k} + \binom{n-1}{k-1}
> $$

`\begin{proof}`
Es gilt

$$
\begin{align}
\binom{n-1}{k-1} + \binom{n-1}{k} & = \frac{(n-1)!}{(k-1)!(n-k)!} + \frac{(n-1)!}{k!(n-k-1)!} \\
 & = \frac{k(n-1)! + (n-k)(n-1)!}{k!(n-k)!} = \frac{n(n-1)!}{k!(n-k)!} \\
 & = \binom{n}{k}
\end{align}
$$

`\end{proof}`
<br> 
***

> [!theorem] Teilmengen einer $n$-elementigen Menge
> Es sei $k,n \in \mathbb{N}$ so, dass $0 \leq k \leq n$ und $n \geq 1$. Die Anzahl der $k$-elementigen Teilmengen einer $n$-elementigen Menge $\{ a_{1},a_{2},\ldots,a_{n} \}$ ist gegeben durch
> 
> $$
> \binom{n}{k}
> $$

