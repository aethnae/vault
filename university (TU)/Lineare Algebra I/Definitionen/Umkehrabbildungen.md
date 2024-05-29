---
tags:
  - Abbildungen
flashcard: false
source: Skript p. 21
date created: 2024-05-29
types: 
examples: 
constructions: 
generalizations: 
justifications: 
aliases:
  - Inverse
---
***
> [!theorem] Bijektivität im Hinblick auf Kompositionen
> Eine Abbildung $f: X \rightarrow Y$ ist genau dann bijektiv, wenn es eine Abbildung $g: Y \rightarrow X$ gibt mit
> 
> $$
> g \circ f=\operatorname{Id}_X \quad \text { und } \quad f \circ g=\operatorname{Id}_Y .
> $$

^711eb3

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

$\Leftarrow$ : Nach Annahme ist $g \circ f=\operatorname{Id}_X$, also ist $g \circ f$ injektiv und daher ist $f$ injektiv (vgl. (3) in [[#^e6cedb]] ). Außerdem ist $f \circ g=\operatorname{Id}_Y$, also ist $f \circ g$ surjektiv und daher ist $f$ surjektiv (vgl. (4) in Satz 2.20). Somit ist $f$ bijektiv.

Die in diesem Satz charakterisierte Abbildung $g: Y \rightarrow X$ ist eindeutig bestimmt. Gibt es eine weitere Abbildung $h: Y \rightarrow X$ mit $h \circ f=\operatorname{Id}_X$ und $f \circ h=\operatorname{Id}_Y$, dann folgt

$$
h=\operatorname{Id}_X \circ h=(g \circ f) \circ h=g \circ(f \circ h)=g \circ \operatorname{Id}_Y=g .
$$

`\end{proof}`

Somit folgt die Definition

> [!definition] Umkehrabbildung
> Ist $f: X \rightarrow Y$ eine bijektive Abbildung, so heißt die in [[#^711eb3]] charakterisierte, eindeutig bestimmte Abbildung $g: Y \rightarrow X$ die Inverse oder Umkehrabbildung von $f$. Wir bezeichnen die Inverse von $f$ mit $f^{-1}$.
