---
tags:
  - differential
week: 2023-12-19
flashcard: false
publish: true
---
***

*Wie sehen die Zuwächse von $z=f(x, y)$ aus, wenn $x, y$ gleichzeitig geändert werden?*

> [!def] Totales Differential 
> Für eine Funktion $z=f\left(x_1, \ldots, x_n\right)$ heißt
> $$
> \mathrm{d} f=\frac{\partial f}{\partial x_1} \mathrm{~d} x_1+\frac{\partial f}{\partial x_2} \mathrm{~d} x_2+\cdots+\frac{\partial f}{\partial x_n} \mathrm{~d} x_n=\sum_{i=1}^n \frac{\partial f}{\partial x_i} \mathrm{~d} x_i=\sum_{i=1}^n \mathrm{~d} f_{x_i}
> $$
> 
> das **totale Differential** von $f$ an der Stelle $x=\left(x_1, \ldots, x_n\right)$.

Das totale Differential erfüllt die folgende Näherungseigenschaft

$$
\Delta f=f\left(x_1+\Delta x_1, \ldots, x_n+\Delta x_n\right)-f\left(x_1, \ldots, x_n\right) \approx \mathrm{d} f=\sum_{i=1}^n \frac{\partial f}{\partial x_i} \mathrm{~d} x_i
$$

Dabei ist dies eine gute Näherung, wenn alle $\Delta x_i$ klein sind.