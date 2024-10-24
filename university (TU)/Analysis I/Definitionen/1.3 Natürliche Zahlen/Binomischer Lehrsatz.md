---
tags:
- Binome
flashcard: false
source: 
date created: 2024-10-24
proved by: 
references: 
justifications:
---
***
#### Theorem

> [!theorem] Binomischer Lehrsatz
> Seien $x, y \in \mathbb{R}$ und $n \in \mathbb{N}$. Dann gilt
> 
> $$
> (x + y)^{n} = \sum_{k = 0}^{n} \binom{n}{k} x^{n-k} y^{k}
> $$

***
#### Beweis

`\begin{proof}`
Mit vollst. Induktion, wir nutzen den Trick der Indexverschiebung.

"$n = 0$": 

Die Aussage ist für $n = 0$ wahr, da $(x+y)^{0} = 1 = \binom{0}{0} \cdot x^{0-0} y^{0}$

"$n \implies n + 1$":

Die Aussage gelte für ein $n \in \mathbb{N}$. Dann folgt

$$
\begin{align}
(x+y)^{n+1} & = (x+y)^{n} \cdot (x+y) \overbrace{ = }^{ IV } \left( \sum_{k = 0}^{n} \binom{n}{k} x^{n-k} y^{k} \right) \cdot (x+y) \\
 & = \sum_{k = 0}^{n} \binom{n}{k} x^{n-k+1} y^{k} + \sum_{k = 0}^{n} \binom{n}{k} x^{n-k} y^{k+1} \\
 & = \binom{n}{0} x^{n+1} y^0+\sum_{k=1}^n\binom{n}{k} x^{n-k+1} y^k+\sum_{k=0}^{n-1}\binom{n}{k} x^{n-k} y^{k+1}+\binom{n}{n} x^0 y^{n+1} \\
 & = x^{n+1}+\sum_{k=1}^n\binom{n}{k} x^{n-k+1} y^k+\sum_{k=1}^n\binom{n}{k-1} x^{n-k+1} y^k+y^{n+1} \\
 & = x^{n+1}+\sum_{k=1}^n\left(\binom{n}{k}+\binom{n}{k-1}\right) x^{n-k+1} y^k+y^{n+1} \\
 & = \binom{n+1}{0} x^{n+1} y^0+\sum_{k=1}^n\binom{n+1}{k} x^{n-k+1} y^k+\binom{n+1}{n+1} x^0 y^{n+1} \\
 & = \sum_{k=0}^{n+1}\binom{n+1}{k} x^{n-k+1} y^k
\end{align}
$$

`\end{proof}`

