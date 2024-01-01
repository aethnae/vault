---
tags:
  - vektoren
week: 2023-12-22
flashcard: false
publish: true
---
***

> [!definition] Vektoren und Skalare
> Es seien
> 
> $$
> x=\left(x_1, \ldots, x_n\right), \quad y=\left(y_1, \ldots, y_n\right) \in \mathbb{R}^n \quad \text { sowie } \quad \lambda \in \mathbb{R}
> $$
> 
> gegeben. Wir nennen $x$ und $y$ auch **Vektoren** und $\lambda$ **Skalar**.

Wir definieren folgende Rechenoperationen:

1. Addition von $x$ und $y$:

$$
x + y = (x_{1}+y_{1},\dots,x_{n}+y_{n})
$$

2. Multiplikation von $x$ mit einem Skalar $\lambda$:

$$
\lambda \cdot x = (\lambda \cdot x_{1},\dots,\lambda \cdot x_{n})
$$

3. **Skalarprodukt** von $x$ und $y$:

$$
\langle x,y \rangle = \sum_{i = 1}^{n} x_{i}y_{i}
$$

$$
\text { (Alternative Schreibweisen: } x^{\top} y \text { oder } x \cdot y \text { ) }
$$

Außerdem gilt die Halbordnung $x \leq y \text { falls } x_i \leq y_i \text { für alle } i=1, \ldots, n \text {. }$

***
##### Beispiel
Für $n=2$ betrachte
$x=(2,4) \in \mathbb{R}^2 \quad$ und $\quad y=(4,5) \in \mathbb{R}^2 \quad$ sowie $\quad \lambda=3 \in \mathbb{R}$.

**Rechenoperationen:**

$$
x+y =(2,4)+(4,5)=(2+4,4+5)=(6,9)
$$

$$
\lambda x = 3 \cdot(2,4) = (3 \cdot 2,3 \cdot 4) = (6,12)
$$

$$
\langle(2,3),(4,5)\rangle = 2 \cdot 4 + 4 \cdot 5 = 28
$$

Es gilt $(2,3) \leq (4,5)$.

**Grafische Darstellung:**

![[Pasted image 20231228194230.png|center|300]]
