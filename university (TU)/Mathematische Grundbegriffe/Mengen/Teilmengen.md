---
tags:
  - mengen
  - operationen
flashcard: false
source: Skript p. 6
date created: 2024-04-09
types: 
examples: 
constructions: 
generalizations:
  - "[[Mengen|Mengen]]"
justifications: 
---
***
#### Definition

> [!definition] Teilmengen
> 1. $M$ und $N$ heißen *disjunkt*, falls $M \cap N = \varnothing$ gilt. In diesem Fall haben $M$ und $N$ keine gemeinsamen Elemente.
> 2. $M$ heißt *Teilmenge* von $N$, falls alle Elemente von $M$ auch in $N$ enthalten sind. Kurzschreibweise: $M \subseteq N$.
> 3. $M$ und $N$ sind *gleich*, wenn sie die gleichen Elemente haben. Insbesondere ist $M = N$ genau dann, wenn $M \subseteq N$ und $N \subseteq M$ gilt.

> [!definition] Kartesisches Produkt
> Das *kartesische Produkt* zweier Mengen $M$ und $N$ ist definiert durch
> 
> $$
> M \times N \coloneqq \{ (x,y) \vert x \in M \text{ und } y \in N \}
> $$
> 
> Es enthält alle (geordneten) Paare $(x,y)$ mit $x \in M$ und $y \in N$. Analog ist das kartesische Produkt von $n$ [[Mengen|Mengen]] $M_{1},\dots,M_{n}$ definiert durch
> 
> $$
> M_{1} \times M_{2} \times \dots M_{n} \coloneqq \{ (x_{1},x_{2},\dots,x_{n}) \vert x_{i} \in M_{i}, i = 1,2,\dots,n \},
> $$
> 
> d.h. als die Menge der geordneten *n-Tupel*.



***
#### Eigenschaften

- $\mathbb{R}^2:=\mathbb{R} \times \mathbb{R}$ ist die Menge aller Punkte der Ebene und $\mathbb{R}^3:=\mathbb{R} \times \mathbb{R} \times \mathbb{R}$ ist die Menge aller Punkte im Raum.

***
#### Beispiele

> [!exm|*] Kartesisches Produkt 
> Für $M=\{1,2,3\}$ und $N=\{1,4\}$ ist
> 
> $$
> M \times N=\{(1,1),(1,4),(2,1),(2,4),(3,1),(3,4)\}
> $$
> 
> Die Reihenfolge innerhalb des Paars $(x, y) \in M \times N$ ist wichtig. Der erste Eintrag ist aus $M$, der zweite aus $N$. Daher gilt beispielsweise $(4,1) \notin M \times N$.

***