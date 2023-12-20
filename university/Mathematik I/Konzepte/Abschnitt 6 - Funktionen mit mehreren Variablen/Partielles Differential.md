---
tags:
  - ableitungen
  - funktionen
week: 2023-12-19
flashcard: false
publish: true
---
***

> [!abstract] Definition 
> Für eine Funktion $z=f\left(x_1, \ldots, x_n\right)$ heißt
> $$
> \mathrm{d} f_{x_i}=\frac{\partial f}{\partial x_i} \underbrace{\mathrm{d} x_i}_{=\Delta x_i}
> $$
> 
> das partielle Differential von $f$ bezüglich $x_i$ an der Stelle $x=\left(x_1, \ldots, x_n\right)$.

Das partielle Differential erfüllt die folgende Näherungseigenschaft:

$$
\Delta_{x_i} f=f\left(x_1, \ldots, x_i+\Delta x_i, \ldots x_n\right)-f\left(x_1, \ldots, x_i, \ldots, x_n\right) \approx \frac{\partial f}{\partial x_i} \Delta x_i
$$

Dabei ist dies eine gute Näherung, wenn $\Delta x_i$ klein ist.