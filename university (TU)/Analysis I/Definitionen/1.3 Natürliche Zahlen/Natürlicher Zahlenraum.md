---
tags:
- Mengen
flashcard: false
source: 
date created: 2024-10-23
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Natürlicher Zahlenraum
> Sei $\mathcal{M}$ die Menge aller induktiven Teilmengen von $\mathbb{R}$. Dann heißt
> 
> $$
> \mathbb{N} \coloneqq \bigcap_{M \in \mathcal{M}} M = \{ x \in \mathbb{R} \mid x \in M \; \forall \; M \in \mathcal{M} \}
> $$
> 
> die *Menge der natürlichen Zahlen*.

> [!remark|*]
> 1. $\mathbb{N}$ ist induktiv
> 2. $M \subseteq \mathbb{R}$ induktiv $\implies \mathbb{N} \in M$
> 3. $0 \in \mathbb{N}$ ist die kleinste natürliche Zahl
> 4. Es gibt keine größte natürliche Zahl, denn aus $n \in \mathbb{N}$ folgt $n + 1 \in \mathbb{N}$ und es gilt $n + 1 > n$.

***
#### Eigenschaften

> [!theorem] Induktionssatz
> Sei $M \subseteq \mathbb{N}$ induktiv. Dann gilt $M = \mathbb{N}$.

^a0fadf

`\begin{proof}`
Da $M$ induktiv ist, gilt $N \subseteq M$. Mit $M \subseteq \mathbb{N}$ folgt $M = \mathbb{N}$.

`\end{proof}`
