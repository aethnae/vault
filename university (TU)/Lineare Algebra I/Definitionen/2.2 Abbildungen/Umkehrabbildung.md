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
  - "[[Komposition von Abbildungen]]"
---
***
#### Definition

> [!definition] Umkehrabbildung
> Ist $f: X \to Y$ eine bijektive Abbildung, so heißt die in [[Sätze über Bijektivität#^7fa63f]] charakterisierte, eindeutig bestimmte Abbildung $g: Y \to X$ die Inverse oder Umkehrabbildung von $f$. Wir bezeichnen die Inverse von $f$ mit $f^{-1}$.

Um nachzuweisen, dass eine gegebene Abbildung $g: Y \to X$ die eindeutig bestimmte Inverse der bijektiven Abbildung $f: X \to Y$ ist, reicht der Nachweis, dass eine der beiden Eigenschaften $g \circ f= \mathrm{Id}_X$ oder $f \circ g= \mathrm{Id}_Y$ gilt. Ist nämlich $f$ bijektiv, so gibt es die eindeutig bestimmte Inverse $f^{-1}$. Gilt nun $g \circ f= \mathrm{Id}_X$, so folgt

$$
g = g \circ \mathrm{Id}_Y = g \circ \left( f \circ f^{-1} \right) = (g \circ f) \circ f^{-1} = \mathrm{Id}_X \circ f^{-1} = f^{-1} .
$$


Genauso folgt $g = f^{-1}$ aus der Annahme $f \circ g = \mathrm{Id}_Y$.

***
#### Satz über Umkehrabbildungen

> [!thm] Bijektivität der Umkehrabbildungen 
> Für zwei bijektive Abbildungen $f: X \rightarrow Y$ und $g: Y \rightarrow Z$ gilt:
> 1. $f^{-1}$ ist bijektiv mit $\left(f^{-1}\right)^{-1}=f$.
> 2. $g \circ f$ ist bijektiv mit $(g \circ f)^{-1}=f^{-1} \circ g^{-1}$.

Im Folgenden beweisen wir nur (2), (1) wird dem Leser als Übung überlassen.

`\begin{proof}`
Wir wissen bereits aus [[Komposition von Abbildungen#^ec86a8]] , dass $g \circ f: X \rightarrow Z$ bijektiv ist. Es gibt somit eine (eindeutige) Inverse von $g \circ f$. Für die Abbildung $f^{-1} \circ g^{-1}$ gilt

$$
\begin{aligned}
\left(f^{-1} \circ g^{-1}\right) \circ(g \circ f) & =f^{-1} \circ\left(g^{-1} \circ(g \circ f)\right)=f^{-1} \circ\left(\left(g^{-1} \circ g\right) \circ f\right) \\
& =f^{-1} \circ\left(\operatorname{Id}_Y \circ f\right)=f^{-1} \circ f=\operatorname{Id}_X
\end{aligned}
$$

Somit ist $f^{-1} \circ g^{-1}$ die Inverse von $g \circ f$.

`\end{proof}`


