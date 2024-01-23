---
tags:
  - vektoren
week: 2023-12-22
flashcard: false
publish: true
---
***

> [!definition] Gradient
> Der Vektor der partiellen Ableitungen einer Funktion $z=f\left(x_1, \ldots, x_n\right)$
> $$
> \operatorname{grad} f=\left(\frac{\partial f}{\partial x_1}, \ldots, \frac{\partial f}{\partial x_n}\right)
> $$
> 
> heißt Gradient der Funktion $f$.

**Schreibweisen:** $\operatorname{grad} f$ oder $\nabla f$

- Der Gradientenvektor an einer Stelle $x^{(0)}$ zeigt in die Richtung des steilsten Anstiegs von $f$
- Das [[Totales Differential|totale Differential]] lässt sich schreiben als

$$
\mathrm{d}f = \sum_{i = 1}^{n} \frac{ \partial f }{ \partial x_{i} } = \underbrace{ \langle \operatorname{grad}f, (\mathrm{d}x_{1},\dots,\mathrm{d}x_{n}) \rangle }_{ \text{ Skalarprodukt } }
$$

$$
\frac{ \mathrm{d} y }{ \mathrm{d} x } 
$$