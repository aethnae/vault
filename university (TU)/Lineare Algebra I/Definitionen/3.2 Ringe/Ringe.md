---
tags:
- Ringe
flashcard: false
source: 
date created: 2024-10-29
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Ring
> Ein Ring ist eine Menge $R$ mit zwei Abbildungen, genannt Operationen oder Verknüpfungen,
> $$
> \begin{aligned}
> & +: R \times R \rightarrow R, \quad(a, b) \mapsto a+b, \quad \text { (Addition) } \\
> & \text { * : } R \times R \rightarrow R, \quad(a, b) \mapsto a * b, \quad \text { (Multiplikation) }
> \end{aligned}
> $$
> 
> für die folgende Regeln erfüllt sind:
> 1. $(R,+)$ ist eine kommutative Gruppe.
>    (Wir nennen das neutrale Element bzgl. der Addition Null, bezeichnen es mit 0, und bezeichnen das zu $a \in R$ inverse Element mit $-a$. Wir schreiben $a-b$ anstatt $a+$ $(-b)$.)
> 2. Die Multiplikation * ist assoziativ, d. h. $(a * b) * c=a *(b * c)$ gilt für alle $a, b, c \in R$.
> 3. Es gelten die Distributivgesetze, d. h. für alle $a, b, c \in R$ gelten
> 
> $$
> \begin{aligned}
> & a *(b+c)=a * b+a * c \\
> & (a+b) * c=a * c+b * c
> \end{aligned}
> $$

- Ein Ring heißt *kommutativ*, falls $a \cdot b = b \cdot a$ für alle $a,b \in \mathbb{R}$ gilt.
- Ein Element $1 \in \mathbb{R}$ heißt *Einselement* (kurz: Eins), falls $1 \cdot a = a \cdot 1 = a$ für alle $a \in \mathbb{R}$ gilt. In diesem Fall nennen wir den Ring einen *Ring mit Eins*.

***

> [!theorem] Ringeigenschaften
> Ist $R$ ein Ring mit Eins, dann gelten folgende Aussagen:
> 1. Das Einselement in $R$ ist eindeutig bestimmt.
> 2. Es gilt $1 = 0$ genau dann, wenn $R$ der [[Nullring]] ist.

`\begin{proof}`
1. Sind $1, e \in R$ mit $1 * a=a * 1=a$ und $e * a=a * e=a$ für alle $a \in R$, dann gilt $1=e * 1=e$.
2. Übungsaufgabe.

`\end{proof}`
