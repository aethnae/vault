---
tags:
  - Abbildungen
flashcard: false
source: 
date created: 2024-10-21
types: 
examples: 
constructions: 
generalizations: 
justifications:
  - "[[Bild und Urbild von Abbildungen]]"
---
***
#### Definition

> [!definition] Komposition von Abbildungen
> Seien $f: X \to Y, x \mapsto f(x)$, und $g: Y \to Z, y \mapsto g(y)$ zwei Abbildungen. Die *Komposition* von $f$ und $g$ ist die Abbildung $g \circ f: X \to Z, x \mapsto g(f(x))$. Gelesen wird dies als "$g$ nach $f$" 

***
#### Eigenschaften der Komposition

> [!theorem] Eigenschaften der Komposition
> Seien $f: W \to X$, $g: X \to Y$, $h: Y \to Z$ Abbildungen. Dann gelten
> 1. $h \circ (g \circ f) = (h \circ g) \circ f$, d.h. die Komposition ist assoziativ.
> 2. Sind $f,g$ beide (injektiv, surjektiv, bijektiv) dann ist $g \circ f$ (injektiv, surjektiv, bijektiv).
> 3. Ist $g \circ f$ injektiv, dann ist $f$ injektiv.
> 4. Ist $g \circ f$ surjektiv, dann ist $g$ surjektiv. 

^ec86a8

`\begin{proof}`
*Beweis nur von (2) für Injektivität, Rest ist HA (ergänzen!)*

Seien $f,g$ beide injektiv und seien $x_{1},x_{2} \in W$, mit $(g \circ f)(x_{1}) = (g \circ f)(x_{2})$. Es ist zu zeigen, dass $x_{1} = x_{2}$ gilt.
Es gilt $g(f(x_{1})) = g(f(x_{2}))$ und somit folgt $f(x_{1}) = f(x_{2})$, denn $g$ ist injektiv. Also gilt auch $x_{1} = x_{2}$, denn $f$ ist injektiv.

`\end{proof}`