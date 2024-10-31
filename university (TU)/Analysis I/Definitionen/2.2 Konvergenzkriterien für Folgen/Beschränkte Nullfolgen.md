---
tags:
- Folgen
flashcard: false
source: 
date created: 2024-10-31
proved by: 
references: 
justifications:
---
***
#### Theorem

> [!theorem] Nullfolge mal beschränkte Folge
> Sei $(a_{n})$ eine Nullfolge und $(b_{n})$ eine beschränkte Folge reeller Zahlen. Dann ist die Folge $(a_{n}b_{n})$ eine Nullfolge.

***
#### Beweis

`\begin{proof}`
Sei $\epsilon > 0$ beliebig. Dann gibt es wegen der Beschränktheit von $(b_{n})$ ein $M \in \mathbb{N}$ mit $\lvert b_{n} \rvert \leq M$ für alle $n \in \mathbb{N}$. Weiter gibt es wegen der Konvergenz von $(a_{n})$ zu $\tilde{\epsilon} \coloneqq \frac{\epsilon}{M} > 0$ ein $N \in \mathbb{N}$ mit $\lvert a_{n} \rvert < \frac{\epsilon}{M}$ für alle $n \geq N$. Dann gilt

$$
\lvert a_{n}b_{n} - 0 \rvert = \lvert a_{n} \rvert \cdot \lvert b_{n} \rvert < \frac{\epsilon}{M} \cdot M = \epsilon
$$

für alle $n \geq N$. Da $\epsilon > 0$ beliebig war, folgt $\lim_{ n \to \infty }a_{n}b_{n} = 0$.

`\end{proof}`

<br> 

***
