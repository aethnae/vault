---
tags:
- Beweise
- Logik
flashcard: false
source: "Skript p. 20"
date created: 2024-04-11
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Direkter Beweis
> Beim direkten Beweis erfolt der Schluss von $A$ auf $B$ auf direktem Weg. Im Allgemeinen geschieht dies über eine Kette von Schlussfolgerungen
> 
> $$
> A \implies A_{1}, \quad A_{1} \implies A_{2} \quad A_{2} \implies A_{3}, \ldots \quad A_{n} \implies B
> $$
> 
> Dass daraus tatsächlich $A \implies B$ folgt, liegt an der **Transitivität** der Implikation, welche per Wahrheitstafeln nachgewiesen werden kann.

***
#### Eigenschaften

> [!theorem] Verkettung von Implikationen
> Seien $A,B,C$ Aussagen. Dann gilt
> 
> $$
> ((A \implies B) \wedge (B \implies C)) \implies (A \implies C)
> $$

***
#### Beispiele

> [!exm|*]  Beispiel eines direkten Beweises
> Seien $m,n \in \mathbb{Z}$. Dann gilt: $m$ gerade und $n$ gerade $\implies$ $m + n$ gerade.
> 
> **Beweis**: Seien also $m$ und $n$ gerade (Voraussetzung). Dann existieren $k \in \mathbb{Z}$ mit $m = 2k$ und $\ell \in \mathbb{Z}$ mit $n = 2 \ell$. Weiter gilt
> 
> $$
> m + n = 2k + 2\ell = 2(k + \ell)
> $$
> 
> Da die Summe zweier ganzer Zahlen wieder eine ganze Zahl ist, gilt $k + \ell \in \mathbb{Z}$. Hieraus folgt, dass $m + n$ gerade ist. (Behauptung)

***
