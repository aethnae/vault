---
tags:
  - Axiom
  - Natural_numbers
flashcard: false
source: Übung 1
date created: 2024-05-08
types: 
examples:
  - "[[Intervallschachtelungsprinzip]]"
constructions: 
generalizations: 
justifications:
---
***

> [!theorem] Äquivalenz der Vollständigkeitsaxiome
> Das Vollständigkeitsaxiom impliziert das Intervallschachtelungsprinzip.

`\begin{proof}`
Es seien $I_{n} = [a_{n}, b_{n}]$.

1. Z.z.: $(a_{n})_{n \in \mathbb{N}}$ bildet eine Cauchy-Folge. 

Wir wissen zum einen $\operatorname{diam}(I_{n}) \rightarrow 0, n \rightarrow \infty$, d.h. es existiert zu jedem $\epsilon > 0$ ein $N_{\epsilon} \in \mathbb{N}$ mit $\operatorname{diam}(I_{n}) < \epsilon : \forall n \geq N_{\epsilon}$.

Für $n, m \geq N_{\epsilon}$ liegen $a_{n}, a_{m} \in I_{N_{\epsilon}}$.

$$
\begin{align}
 & \implies \lvert a_{n} - a_{m} \rvert \leq \operatorname{diam}(I_{N_{\epsilon}}) < \epsilon \\
 & \implies (a_{n})_{n \in \mathbb{N}} \text{ ist eine Cauchy-Folge } \\
 & \implies (a_{n})_{n \in \mathbb{N}} \text{ konvergiert in } \mathbb{R}
\end{align}
$$

`\end{proof}`