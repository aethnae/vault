---
tags:
- Abbildungen
flashcard: false
source: "Skript p. 20"
date created: 2024-05-29
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Komposition mehrerer Abbildungen

> [!definition] Komposition
> Seien $f: X \rightarrow Y, x \mapsto f(x)$, und $g: Y \rightarrow Z, y \mapsto g(y)$, Abbildungen. Dann ist die *Komposition* oder *Hintereinanderausfuïhrung* von $f$ und $g$ die Abbildung
> 
> $$
> g \circ f: X \rightarrow Z, \quad x \mapsto g(f(x)) .
> $$
> 
> Der Ausdruck $g \circ f$ wird oft ,,g nach $f$ “ gelesen, woraus die Reihenfolge der Komposition deutlich wird: Erst wird $f$ auf $x$ und dann $g$ auf $f(x)$ angewandt. Man sieht leicht, dass $f \circ \operatorname{Id}_X=f=\operatorname{Id}_Y \circ f$ für jede Abbildung $f: X \rightarrow Y$ gilt.

***

> [!theorem] Eigenschaften der Komposition
> Seien $f: W \rightarrow X, g: X \rightarrow Y, h: Y \rightarrow Z$ Abbildungen, dann gilt:
> 1. $h \circ(g \circ f)=(h \circ g) \circ f, d$. h. die Komposition von Abbildungen ist assoziativ.
> 2. Sind $f$ und $g$ beide injektiv/surjektiv/bijektiv, dann ist $g \circ f$ injektiv/surjektiv/bijektiv.
> 3. Ist $g \circ f$ injektiv, dann ist $f$ injektiv.
> 4. Ist $g \circ f$ surjektiv, dann ist $g$ surjektiv.

^e6cedb

