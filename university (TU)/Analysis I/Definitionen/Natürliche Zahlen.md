---
tags:
  - Natural_numbers
  - mengen
flashcard: false
source: Übung 1
date created: 2024-05-08
types: 
examples: 
constructions: 
generalizations: 
justifications:
  - "[[Induktive Mengen]]"
---
***
#### Definition

> [!definition] Menge der natürlichen Zahlen
> Sei $M$ die Menge aller [[Induktive Mengen#^e84cce|induktiven Mengen]], so gilt ... 

> [!remark] Eigenschaften der natürlichen Zahlen
> - $\mathbb{N}$ ist eine induktive Menge
> - $M \subseteq \mathbb{R}$ induktiv $\implies \mathbb{N} \subseteq M$
> - $0 \in \mathbb{N}$ ist die *kleinste* natürliche Zahl, d.h. $0 \leq n : \forall n \in \mathbb{N}$, denn $I = [0, \infty)$ ist induktiv

> [!axiom] 
> Es sein $M \subseteq \mathbb{N}$ induktiv. Dann gilt $M = \mathbb{N}$

`\begin{proof}`
$M \subseteq \mathbb{N}$ ist induktiv $\implies \mathbb{N} \subseteq M \implies N = M$
`\end{proof}`

***

> [!theorem] Prinzip der vollständigen Induktion
> Zu jedem $n \in \mathbb{N}$ sei eine von $n$ abhängige Aussage $A(n)$ gegeben.
> Es gelte:
> 
> 1. $A(0)$ ist wahr
> 2. $\forall n \in \mathbb{N} : A(n) \implies A(n+1)$
> 3. ...