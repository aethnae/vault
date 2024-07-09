---
tags:
  - summen
flashcard: false
source: Skript Satz 1.1
date created: 2024-06-01
types: 
examples: 
constructions: 
generalizations: 
justifications:
  - "[[Beweis per Vollständiger Induktion]]"
---
***

> [!definition] Kleiner Satz von Gauß
> Für jede natürliche Zahl $n \in \mathbb{N}, n \geq 1$ gilt
> 
> $$
> \sum_{k = 1}^{n} k = 1 + 2 + \ldots + n = \frac{n(n+1)}{2}
> $$

`\begin{proof}`
Siehe [[Beweis per Vollständiger Induktion#^7fcf58]].

`\end{proof}`

***

> [!theorem] Satz 1.2
> Für $n \in \mathbb{N}, n \geq 1$ gilt
> 
> $$
> \sum_{k = 1}^{n} \frac{1}{k(k+1)} = 1 - \frac{1}{n+1}
> $$

`\begin{proof}`
Beweis über vollständige Induktion. Für $n = 1$ gilt somit

$$
\frac{1}{1(1+1)} = \frac{1}{2} = 1 - \frac{1}{1+1}
$$

Angenommen $\sum_{k = 1}^{n} \frac{1}{k(k+1)} = 1 - \frac{1}{n+1}$ gelte für ein beliebiges, aber festes $n \in \mathbb{N}$. Im Induktionsschritt gilt also

$$
\sum_{k = 1}^{n+1} \frac{1}{k(k+1)} = \sum_{k = 1}^{n} \frac{1}{k(k+1)} + \frac{1}{(n+1)(n+2)} = 1 - \frac{1}{n+1} + \frac{1}{(n+1)(n+2)}
$$

Also gilt abschließend

$$
1 - \frac{1}{n+1} + \frac{1}{(n+1)(n+2)} = 1 - \frac{n+2-1}{(n+1)(n+2)} = 1 - \frac{1}{n+2}
$$

`\end{proof}`