---
tags:
  - funktionen
week: 2023-11-07
flashcard: true
---
***

> [!important] Definition
> Hat ein **Polynom** $f(x)$ vom Grad $n$ die Nullstellen $x_1, \ldots, x_n$, so kann $f(x)$ als
> $$
> f(x)=a_n \cdot\left(x-x_1\right) \cdot\left(x-x_2\right) \cdot \ldots \cdot\left(x-x_n\right)
> $$
> dargestellt werden. Dabei ist $a_n$ der Vorfaktor des Terms $x^n$ mit höchstem Exponenten.
> Diese Darstellung heißt **Linearfaktorzerlegung**.

**Beispiel:**
Das Polynom

$$
f(x)=2 x^3-8 x^2+2 x+12
$$

hat die Nullstellen $x_1=-1, x_2=2$ und $x_3=3$ und kann geschrieben werden als

$$
f(x)=2 \cdot \underbrace{(x+1)}_{=(x-(-1))} \cdot(x-2) \cdot(x-3)
$$
***

Die Anzahl, wie oft ein gleicher *Linearfaktor* vorkommt, heißt **Vielfachheit der Nullstelle**.

**Beispiel:**
Das Polynom

$$
f(x)=(x+1)^2(x-3)^3(x+2)
$$

hat die Nullstellen

- $x_1=-1$ mit Vielfachheit $2 \quad x_2=3$ mit Vielfachheit $3 \quad x_3=-2$ mit Vielfachheit 1
***

Hat ein Polynom $f(x)$ nur $k<n$ Nullstellen $x_1, \ldots, x_k$, so kann $f(x)$ als

$$
f(x)=\left(x-x_1\right) \cdot\left(x-x_2\right) \cdot \ldots \cdot\left(x-x_k\right) \cdot \tilde{f}(x)
$$

dargestellt werden, wobei $\tilde{f}$ ein Polynom vom Grad $n-k$ ist, das keine Nullstellen besitzt.

**Beispiel:**
Das Polynom

$$
f(x)=2 x^4-6 x^3+5 x^2-3 x+2
$$

hat nur zwei Nullstellen $x_1=1$ und $x_2=2$.
Es gilt

$$
f(x)=(x-1)(x-2) \underbrace{\left(2 x^2+1\right)}_{=\tilde{f}(x)} .
$$
