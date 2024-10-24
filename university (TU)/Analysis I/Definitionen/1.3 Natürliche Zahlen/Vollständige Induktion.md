---
tags:
- Mengen
flashcard: false
source: 
date created: 2024-10-23
proved by: 
references: 
justifications:
---
***
#### Theorem

> [!theorem] Beweisprinzip der vollständigen Induktion
> Zu jedem $n \in \mathbb{N}$ sei eine Aussage $A(n)$ gegeben. Sind die Aussagen
> 1. $A(0)$
> 2. $\forall \; n \in \mathbb{N} (A(n) \implies A(n+1))$
> 
> wahr, so ist auch $\forall \; n \in \mathbb{N} \; A(n)$ wahr.

***
#### Beweis

`\begin{proof}`
Setze $W \coloneqq \{ n \in \mathbb{N} \mid A(n) \text{ ist wahr } \}$. Dann gilt $W \subseteq \mathbb{N}$. Weiter ist $W$ induktiv, denn aus 1. folgt $0 \in W$ und mit 2. folgt $\forall \; x \in \mathbb{R} \; (x \in W \implies x + 1 \in W)$
Mit dem [[Natürlicher Zahlenraum#^a0fadf]] folgt $W = \mathbb{N}$.

`\end{proof}`
<br> 

***
#### Eigenschaften

> [!theorem] Eigenschaften der vollständigen Induktion
> Seien $m,n \in \mathbb{N}$. Dann gilt
> 1. $m + n \in \mathbb{N}$ und $m \cdot n \in \mathbb{N}$.
> 2. $m - n \in \mathbb{N}$ falls $m \geq n$.
> 3. Es gibt kein $p \in \mathbb{N}$ mit $n < p < n + 1$
> 4. Jede Menge $\varnothing \neq M \subseteq \mathbb{N}$ hat ein kleinstes Element, d.h. es gibt ein $a \in M$ mit $a \leq p$ für alle $p \in M$.

`\begin{proof}`
Der Beweis erfolgt als Hausaufgabe.
`\end{proof}`