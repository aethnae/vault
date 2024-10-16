---
tags:
  - mengen
flashcard: false
source: 
date created: 2024-10-16
types: 
examples: 
constructions: 
generalizations:
  - "[[Mengen|Mengen]]"
justifications:
---
***
#### Definition

> [!definition] Leere Menge
> Die Menge $\varnothing \coloneqq \{ x \mid x \neq x \}$ bezeichen wir als *leere Menge*. Eine Menge, die mindestens ein Objekt enthält, bezeichnen wir als *nichtleer*.

> [!theorem] Sätze bzgl. der Leeren Menge
> Für jede [[Mengen|Menge]] $M$ gilt
> 1. $\varnothing \subseteq M$
> 2. $M \subseteq \varnothing \implies M = \varnothing$

`\begin{proof}`
1. Zu Zeigen ist die Aussage $\forall x : x \in \varnothing \implies x \in M$. Da die leere eben keine Elemente enthält, ist der erste Teil der Aussage, $x \in \varnothing$ falsch, und die Implikation $x \in M$ somit für alle $x$ wahr. Damit ist $\varnothing \subseteq M$ für alle Mengen $M$.
2. Sei $M \subseteq \varnothing$. Aus (1) folgt, dass $\varnothing \subseteq M$ gilt, somit ist nach [[Teilmengen#^e7c837]] (3) also $M = \varnothing$ falls, $M \subseteq \varnothing$. 
`\end{proof}`
