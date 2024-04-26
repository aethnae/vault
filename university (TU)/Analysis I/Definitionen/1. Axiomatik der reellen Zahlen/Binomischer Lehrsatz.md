---
tags:
- Binominalkoeffizienten
flashcard: false
source: "Skript p. 40 | Satz 1.40"
date created: 2024-04-26
proved by: 
references: 
justifications:
---
***
#### Theorem

> [!theorem|*] Binomischer Lehrsatz
> Seien $x, y \in \mathbb{R}$ und $n \in \mathbb{N}$. Dann gilt
> 
> $$
> (x+y)^{n}=\sum_{k = 0}^{n} \binom{n}{k}x^{n-k}y^{k}
> $$

^dfe5a3

***
#### Beweis

Der Beweis wird mit [[Beweis per Vollständiger Induktion|vollständiger Induktion]] geführt, wobei auch das Prinzip der *Indexverschiebung* genutzt wird.

`\begin{proof}`
**IA**: "$n = 0$"

Es gilt: $(x+y)^{0} = 1 = \binom{0}{0}x^{0}y^{0} = \sum_{k = 0}^{0}\binom{0}{k}x^{0-k}y^{0}$.

**IV**: "$n \implies n + 1$"

Die Formel [[#^dfe5a3]] sei wahr für ein beliebiges, aber festes $n \in \mathbb{N}$. Wir zeigen, das sie dann auch für $n+1$ wahr ist. Es gilt

$$
\begin{align}
(x+y)^{n+1} & = (x+y)^{n}(x+y) = \left( \sum_{k = 0}^{n} \binom{n}{k}x^{n-k}y^{k} \right)(x+y) \\
 & = \sum_{k = 0}^{n} \binom{n}{k}x^{n-k+1}y^{k}+\sum_{k = 0}^{n} \binom{n}{k}x^{n-k}y^{k+1} \\
 & = \binom{n}{0}x^{n+1}y^{0}+\sum_{k = 1}^{n} \binom{n}{k}x^{n-k+1}y^{k}+\sum_{k = 0}^{n-1} \binom{n}{k}x^{n-k}y^{k+1}+\binom{n}{n}x^{0}y^{n+1} \\
 & = x^{n+1}+\sum_{k = 1}^{n} \binom{n}{k}x^{n-k+1}y^{k}+\sum_{k = 1}^{n} \binom{n}{k-1}x^{n-k+1}y^{k}+y^{n+1} \\
 & = 
\end{align}
$$
`\end{proof}`
***




