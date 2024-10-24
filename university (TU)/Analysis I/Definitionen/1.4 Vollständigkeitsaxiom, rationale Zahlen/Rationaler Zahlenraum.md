---
tags:
- Rationale_Zahlen
flashcard: false
source: 
date created: 2024-10-24
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Rationale Zahlen
> Die Menge
> 
> $$
> \mathbb{Q}:=\left\{x \in \mathbb{R} \left\lvert\, x=\frac{p}{q}\right., p, q \in \mathbb{Z}, q>0\right\}
> $$
> 
> heißt Menge der rationalen Zahlen. Ihre Elemente heißen rationale Zahlen.

***
#### Bemerkungen

> [!remark] Eigenschaften der rationalen Zahlen
> Für die Menge der rationalen Zahlen gibt es auch andere Mengenschreibweisen, die von unserer Definition leicht abweichen, wie z.B.
> $$
> \mathbb{Q}=\left\{x \in \mathbb{R} \left\lvert\, x=\frac{p}{q}\right., p, q \in \mathbb{Z}, q \neq 0\right\}
> $$
> 
> So können wir z.B. ausnutzen, dass $-\frac{1}{2}=\frac{-1}{2}$ gilt, um einzusehen, dass $-\frac{1}{2}$ auch nach unserer Definintion von $\mathbb{Q}$ eine rationale Zahl ist.
> 
> Für $x, y \in \mathbb{Q}$ gilt $x+y, x-y, x \cdot y \in \mathbb{Q}$ und im Fall $y \neq 0$ auch $\frac{x}{y} \in \mathbb{Q}$. Insbesondere erfüllt auch $\mathbb{Q}$ die Körper- und Anordnungsaxiome.

***

> [!theorem] Rationale vs. reelle Zahlen, Vollständigkeitsaxiom
> Es gibt keine rationale Zahl $x \in \mathbb{Q}$ mit $x^{2} = 2$.

`\begin{proof}`
Angenommen, es gibt ein $x \in \mathbb{Q}$ mit $x^2=2$. Dann existieren $p, q \in \mathbb{Z}$ mit $q>0$, so dass

$$ 
x=\displaystyle \frac{R}{q}
$$

O.B.d.A. können wir annehmen, dass $p$ und $q$ nicht beide gerade sind, denn andernfalls können wir solange kürzen, bis $p$ ungerade oder $q$ ungerade ist. Aus 

$$ 
x^2=\frac{p^2}{q^2}=2
$$

folgt $p^2=2 q^2$. Demnach ist $p^2$ und damit auch $p$ eine gerade Zahl. Dann gibt es aber ein $m \in \mathbb{Z}$ mit $p = 2m$. Daraus erhalten wir wiederum

$$
2 q^2=p^2=4 m^2 \quad \text { bzw. } \quad q^2=2 m^2 .
$$


Das bedeutet aber, dass $q^2$ und damit auch $q$ gerade ist und dies steht im Widerspruch dazu, dass $p$ und $q$ nicht beide gerade sind. Folglich war unsere Annahme falsch und es gibt keine rationale Zahl $x$ mit $x^2=2$.

`\end{proof}`

