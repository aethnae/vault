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

> [!theorem] Bijektivität im Hinblick auf Kompositionen
> Eine Abbildung $f: X \rightarrow Y$ ist genau dann bijektiv, wenn es eine Abbildung $g: Y \rightarrow X$ gibt mit
> 
> $$
> g \circ f=\operatorname{Id}_X \quad \text { und } \quad f \circ g=\operatorname{Id}_Y .
> $$

`\begin{proof}`
$\Rightarrow$ : Ist $f$ bijektiv, so gibt es nach Satz 2.17 zu jedem $y \in Y$ genau ein $x=x_y \in X$ mit $f\left(x_y\right)=y$. Wir definieren die Abbildung $g$ durch
$$
g: Y \rightarrow X, \quad g(y)=x_y .
$$

Sei nun ein $\tilde{y} \in Y$ gegeben, dann gilt
$$
(f \circ g)(\widetilde{y})=f(g(\widetilde{y}))=f\left(x_{\widetilde{y}}\right)=\widetilde{y}, \quad \text { also } \quad f \circ g=\operatorname{Id}_Y .
$$

Ist andererseits ein $\tilde{x} \in X$ gegeben, dann ist $\tilde{y}=f(\widetilde{x}) \in Y$. Nach Satz 2.17 gibt es genau ein $x_{\tilde{y}} \in X$ mit $f\left(x_{\tilde{y}}\right)=\tilde{y}$, so dass $\tilde{x}=x_{\tilde{y}}$ folgt. Somit gilt
$$
(g \circ f)(\widetilde{x})=g(f(\widetilde{x}))=g(\widetilde{y})=x \tilde{y}=\widetilde{x}, \quad \text { also } \quad g \circ f=\operatorname{Id}_X .
$$
$\Leftarrow$ : Nach Annahme ist $g \circ f=\operatorname{Id}_X$, also ist $g \circ f$ injektiv und daher ist $f$ injektiv (vgl. (3) in Satz 2.20). Außerdem ist $f \circ g=\operatorname{Id}_Y$, also ist $f \circ g$ surjektiv und daher ist $f$ surjektiv (vgl. (4) in Satz 2.20). Somit ist $f$ bijektiv.

Die in Satz 2.21 charakterisierte Abbildung $g: Y \rightarrow X$ ist eindeutig bestimmt. Gibt es eine weitere Abbildung $h: Y \rightarrow X$ mit $h \circ f=\operatorname{Id}_X$ und $f \circ h=\operatorname{Id}_Y$, dann folgt
$$
h=\operatorname{Id}_X \circ h=(g \circ f) \circ h=g \circ(f \circ h)=g \circ \operatorname{Id}_Y=g .
$$
`\end{proof}`