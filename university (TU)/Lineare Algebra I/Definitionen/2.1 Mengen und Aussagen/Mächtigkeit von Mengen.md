---
tags:
  - Mengen
flashcard: false
source: 
date created: ""
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Kardinalität einer Menge

> [!definition] Mächtigkeit
> Sei $M$ eine Menge. Dann gilt
> 
> 1. Die *Mächtigkeit* oder *Kardinalität* von $M$, bezeichnet mit $\lvert M \rvert$, ist die Anzahl der Elemente von $M$.
> 2. Die *Potenzmenge* von $M$, geschrieben $\mathcal{P}(M)$, ist die Menge aller Teilmengen von $M$, d.h.
> 
> $$
> \mathcal{P}(M) \coloneqq \{ N \mid N \subseteq M \}
> $$

> [!definition] Endlichkeit einer Menge
> Eine Menge $A$ heißt *endlich*, falls sie eine endliche Menge an Elementen enthält. Mathematisch ausgedrückt ist dies der Fall, wenn es eine injektive Funktion
> 
> $$
> f: A \rightarrow \{ 1,\ldots,n \}
> $$
> 
> für ein $n \in \mathbb{N}$ gibt. Andernfalls bezeichen wir die Menge als **unendlich**.

> [!remark] Endlichkeit & Kardinalität von Mengen
>  Die Anzahl der Elemente von $M$ wird **Kardinalität** (oder *Mächtigkeit*) von $M$ genannt und mit $\vert M \vert$ notiert. 


- Die leere Menge hat die Kardinalität Null und es gilt $\mathcal{P}(\varnothing) = \{ \varnothing \}$, also $\lvert \mathcal{P}(\varnothing) \rvert = 1$.
- Man kann zeigen, dass für jede Menge $M$ mit endlich vielen Elementen $\lvert \mathcal{P}(M) \rvert = 2^{\lvert M \rvert}$ gilt.
