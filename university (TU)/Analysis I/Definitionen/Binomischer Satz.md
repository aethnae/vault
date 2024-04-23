---
tags:
- Mengen
flashcard: false
source: "Skript Satz 1.6"
date created: 2024-04-23
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!theorem] Binomischer Satz
> Für $n \in \mathbb{N}, n \geq 1$ gilt
> 
> $$
> \begin{align}
> (x+y)^{n} & = 1 \cdot x^{n} + {n \choose 1} x^{n-1}y + \ldots + {n \choose n-1} x y^{n-1} + y^{n} \\
>  & = \sum_{k = 0}^{n} {n \choose k} x^{n-k}y^{k}
\end{align}
> $$

***
#### Beweis

`\begin{proof}`
Beweis über Induktion.

**IA**:
$n = 1 : (x+y)^{1} = {1 \choose 0} x^{1} + {1 \choose 1} y^{1}$ ist richtig

**IVor**:
$(x+y)^{n} = \sum_{k = 0}^{n} {n \choose k} x^{n - k} y^{k}$

**IBeh**:
$(x+y)^{n+1} = \sum_{k = 0}^{n+1}{n+1 \choose k}x^{n+1-k}y^{k}$

**ISchritt**:
Laut **IVor** gilt:

$$
\begin{align}
(x+y)^{n} & = \sum_{k = 0}^{n} {n \choose k} x^{n-k}y^{k} \\
(x+y)^{n+1} & = (x+y) \left( \sum_{k = 0}^{n} {n \choose k} x^{n-k}y^{k} \right) \\
 & = \sum_{k = 0}^{n} {n \choose k} x^{n + 1 - k}y^{k} + \sum_{k = 0}^{n} {n \choose k} x^{n-k}y^{k+1} \\
 & = \sum_{k = 0}^{n} {n \choose k} x^{n+1-k}y^{k} + \sum_{l = 1}^{n+1} {n \choose l - 1} x^{n-(l-1)}y^{l}
\end{align}
$$
`\end{proof}`

***
#### Beispiele

> [!exm|*] <% tp.file.cursor(5) %> 
> <% tp.file.cursor(6) %>

***
