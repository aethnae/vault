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

> [!definition] Induktive Mengen
> Eine Menge $M \subseteq \mathbb{R}$ heißt *induktiv*, falls gilt:
> 1. $0 \in M$
> 2. Für alle $x \in \mathbb{R}$ gilt: $x \in M \implies x + 1 \in M$

***
#### Beispiele

> [!exm|*] Beispiel für induktive Mengen 
> $M \coloneqq [0, \infty[ = \{ x \in \mathbb{R} \mid x \geq 0 \}$ ist induktiv, denn $0 \in M$ und für alle $x \in \mathbb{R}$ gilt:
> 
> $$
> x \in M \implies x \geq 0 \implies x + 1 \geq 0 + 1 \geq 0 \implies x + 1 \in M
> $$

***

> [!theorem] Satz über induktive Mengen
> Sei $I$ eine Indexmenge und für jedes $i \in I$ sei $M_{i} \in \mathbb{R}$ induktiv. Dann ist auch $\bigcap\nolimits_{i \in I} M_{i} \coloneqq \{ x \in \mathbb{R} \mid x \in M_{i} \; \forall i \in I \}$ induktiv.

`\begin{proof}`
1. Für jedes $i \in I$ gilt $0 \in M_{I}$ damit folgt $0 \in \bigcap\nolimits_{i \in I} M_{i}$
2. Für alle $x \in \mathbb{R}$ gilt
   
   $$
x \in \bigcap_{i \in I} M_{i} \implies x \in M_{i} \; \forall i \in I \overbrace{ \implies }^{ \text{ M induktiv } } x + 1 \in M_{i} \; \forall i \in I
$$

`\end{proof}`


