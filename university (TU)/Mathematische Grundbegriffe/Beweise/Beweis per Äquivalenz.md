---
tags:
- Beweise
- Logik
flashcard: false
source: "Skript p. 25" 
date created: 2024-04-14
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Äquivalenzbeweis
> Beweise einer Äquivalenz "$A \Leftrightarrow B$" werden oft in Beweise der Implikationen "$A \implies B$" und "$B \implies A$" aufgeteilt. Der Beweis dieser Methode kann über eine Wahrheitstafel geführt werden.

***
#### Eigenschaften

- 

***
#### Beispiele

> [!exm|*] Beweis der geraden Quadratzahlen mit Hilfe einer Äquivalenz 
> Sei $n \in \mathbb{N}$. Dann gilt: $n$ gerade $\Leftrightarrow$ $n^{2}$ gerade.
> 
> `\begin{proof}`
> Wir teilen den Beweis in *Hinrichtung* ($\implies$) und *Rückrichtung* ($\impliedby$) auf.
> 
> ($\implies$) Zuerst beweisen wir: "$n$ gerade $\implies$ $n^{2}$ gerade." Sei also $n$ gerade, d.h. es existiert ein $k \in \mathbb{N}$ mit $n = 2k$. Somit gilt
> 
> $$
> n^{2} = (2k)^{2} = 4k^{2} = 2 \cdot 2k^{2}
> $$
> 
> Wegen $2k^{2} \in \mathbb{N}$ ist dann auch $n^{2}$ gerade.
> 
> ($\impliedby$) Es bleibt noch zu zeigen: "$n^{2}$ gerade $\implies$ $n$ gerade." Diese Aussage haben wir schon [[Beweis per Kontraposition#^707a66|hier]] bewiesen, und können sie somit als wahr annehmen.
> `\end{proof}`

***
$$

$$