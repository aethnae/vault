---
tags:
  - vektoren
week: 2023-12-22
flashcard: false
publish: true
---
***

Da die Tangente bei $x_0$ eine Gerade ist, die bei $x_0$ mit der Funktion $f$ in Funktionswert und Ableitungswert übereinstimmt, ergibt sich als allgemeine Form für Tangenten

$$
t(x) = f(x_{0}) + f'(x_{0}) \cdot (x-x_{0})
$$

***

> [!definition] Tangentialebene
> Ebene, die bei $\left(x_0, y_0\right)$ in Funktionswert und den partiellen Ableitungen mit der Funktion $f$ übereinstimmt. Die Tangentialebene lässt sich durch die Funktion
> 
> $$
>\begin{align}
 t(x, y) & =f\left(x_0, y_0\right)+\frac{\partial f}{\partial x}\left(x_0, y_0\right)\left(x-x_0\right)+\frac{\partial f}{\partial y}\left(x_0, y_0\right)\left(y-y_0\right) \\
 & = f\left(x_0, y_0\right)+\underbrace{\left\langle\operatorname{grad} f,\left(x-x_0, y-y_0\right)\right\rangle}_{\text {Skalarprodukt }}
\end{align}
> $$
> 
> darstellen.

***

> [!definition] Tangentialhyperebene
> Ebene, die bei $\left(x_0, y_0\right)$ mit der Funktion $f$ im Funktionswert sowie in allen $n$ partiellen Ableitungen erster Ordnung übereinstimmt. Die Tangentialhyperebene lässt sich durch die Funktion
> 
> $$
> \begin{aligned}
> t\left(x_1, \ldots, x_n\right) & =f\left(x^{(0)}\right)+\sum_{i=1}^n \frac{\partial f}{\partial x_i}\left(x^{(0)}\right) \cdot\left(x_i-x_i^{(0)}\right) \\
> & =f\left(x^{(0)}\right)+\underbrace{\left\langle\operatorname{grad} f,\left(x_1-x_1^{(0)}, \ldots, x_n-x_n^{(0)}\right)\right\rangle}_{\text {Skalarprodukt }}
> \end{aligned} 
> $$

