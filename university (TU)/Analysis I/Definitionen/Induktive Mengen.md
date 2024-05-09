---
tags:
  - Axiom
  - Natural_numbers
flashcard: false
source: Übung 1
date created: 2024-05-08
types: 
examples: []
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Induktive (Teil-)Menge
> Eine Teilmenge $M \subseteq \mathbb{R}$ heißt *induktiv*, falls folgende Eigenschaften erfüllt sind:
> 
> 1. $0 \in M$
> 2. $\forall a \in \mathbb{R} : a \in M \implies a + 1 \in M$

^e84cce

- Ein Beispiel wäre durch $I = [0, \infty)$ gegeben

***

> [!theorem] Schnitt der induktiven Mengen
> Es sei $I \in \mathbb{R}$ eine [[Indexmenge]] und $M_{i} \subseteq \mathbb{R}, i \in I$ eine induktive Menge. So gilt
> 
> $$
> \bigcap_{i \in I} M_{i} = \{ x \mid x \in M : \forall i \in I \}
> $$

`\begin{proof}`
1. Da $M$ induktiv ist für alle $i \in I$, gilt

$$
\forall i \in I : 0 \in M \implies 0 \in \bigcap_{i \in I} M
$$

2. Es sei $a \in \mathbb{R}$ mit $a \in \bigcap_{i \in I} M$, so gilt

$$
\forall i \in I : a \in M
\implies \forall i \in I : a + 1 \in M
\implies a + 1 \in \bigcap_{i \in I} M
$$
`\end{proof}`