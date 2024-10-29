---
tags:
- Gruppen
flashcard: false
source: 
date created: 2024-10-28
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Gruppen
> Eine *Gruppe* ist eine Menge $G$ mit einer Verknüpfung
> 
> $$
> \oplus : G \times G \to G
> $$
> 
> für die folgende Regeln gelten:
> 1. $\oplus$ ist assoziativ, d.h. $(a \oplus b) \oplus c = a \oplus (b \oplus c)$
> 2. Es gibt ein Element $e \in G$, genannt *neutrales* Element, für das gilt
> 	1. $e \oplus a = a$ für alle $a \in G$
> 	2. Zu jedem $a \in G$ existiert ein $\tilde{a} \in G$, so dass $\tilde{a} \oplus a = e$.
> 
> Gilt $a \oplus b = b \oplus a$ für alle $a,b \in G$, dann heißt $G$ *kommutativ* oder *abelsch*.

^a78382

***
#### Eigenschaften

> [!theorem] Gruppeneigenschaften
> Für jede Gruppe $(G, \oplus)$ gelten
> 1. Ist $e \in G$ ein neutrales Element und sind $a, \tilde{a} \in G$ mit $\tilde{a} \oplus a = e$, so ist $a \oplus \tilde{a} = e$.
> 2. Ist $e \in G$ ein neutrales Element und ist $a \in G$, so gilt $a \oplus e = a$.
> 3. $G$ enthält genau ein neutrales Element
> 4. Jedes $a \in G$ hat genau ein inverses Element

`\begin{proof}`
1. Sei $e \in G$ ein neutrales Element und seien $a, \tilde{a} \in G$ mit $\tilde{a} \oplus a=e$. Dann gibt es nach [[#^a78382]]  ein Element $a_1 \in G$ mit $a_1 \oplus \tilde{a}=e$. Es folgt

$$
\begin{aligned}
a \oplus \tilde{a} & =e \oplus(a \oplus \widetilde{a})=\left(a_1 \oplus \widetilde{a}\right) \oplus(a \oplus \widetilde{a})=a_1 \oplus((\widetilde{a} \oplus a) \oplus \widetilde{a}) \\
& =a_1 \oplus(e \oplus \widetilde{a})=a_1 \oplus \tilde{a}=e
\end{aligned}
$$

2. Sei $e \in G$ ein neutrales Element und sei $a \in G$. Dann existiert ein $\tilde{a} \in G$ mit $\tilde{a} \oplus a=e$. Nach (1) gilt dann auch $a \oplus \tilde{a}=e$ und es folgt

$$
a \oplus e=a \oplus(\widetilde{a} \oplus a)=(a \oplus \widetilde{a}) \oplus a=e \oplus a=a .
$$

3. Seien $e, e_1 \in G$ zwei neutrale Elemente. Dann gilt $e_1 \oplus e=e$, denn $e_1$ ist ein neutrales Element. Da $e$ ebenfalls ein neutrales Element ist, gilt $e_1=e \oplus e_1=e_1 \oplus e$, wobei wir für die zweite Gleichung die Aussage (2) benutzt haben. Somit folgt $e=e_1$.
4. Seien $\tilde{a}, a_1 \in G$ zwei zu $a \in G$ inverse Elemente und sei $e \in G$ das (eindeutige) neutrale Element. Mit Hilfe von (1) und (2) folgt dann

$$
\tilde{a}=e \oplus \tilde{a}=\left(a_1 \oplus a\right) \oplus \tilde{a}=a_1 \oplus(a \oplus \tilde{a})=a_1 \oplus e=a_1 .
$$


`\end{proof}`

