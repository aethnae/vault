---
tags:
  - funktionen
week: 2023-10-31
flashcard: true
---
***

> [!def] Polynomfunktionen
> Eine reellwertige Funktion $f: D \rightarrow \mathbb{R}$ der Form
> $$
> x \mapsto f(x)=a_n x^n+a_{n-1} x^{n-1}+\cdots+a_2 x^2+a_1 x+a_0
> $$
> mit $a_0, a_1, \ldots, a_n \in \mathbb{R}$ und $a_{n} \neq 0$ heißt **Polynomfunktion**.
> - Die Zahlen $a_i$ heißen Koeffizienten des Polynoms
> - Die Zahl $n$ (= höchste Potenz) heißt Grad des Polynoms
> - Ein Polynom vom Grad $n=1$ ist eine lineare Funktion
> - Ein Polynom vom Grad $n=2$ ist eine quadratische Funktion

#### Graphen von Polynomfunktionen
- Polynome haben bis zu $n$ (= **Grad**) viele Schnittpunkte mit der $x$-Achse (= **Nullstellen**)
- Polynome können mehrere Maxima und Minima besitzen
- Skizze möglich per Wertetabelle
- Besondere Punkte können mittels Kurvendiskussion bestimmt werden

![[Pasted image 20231031144038.png|400]]

#### Nullstellen von Polynomen

> [!def] Nullstellen von Polynomen
> Es gilt $f(x) \cdot g(x)=0$ gilt genau dann, wenn $f(x)=0$ oder $g(x)=0$
> $\rightarrow$
> Ausklammern von Faktoren (insbesondere $x$ ) hilft bei der Berechnung von Nullstellen.

**Beispiel:**

$$
\begin{array}{rrr} 
& x^3-3 x^2+2 x=0 \\
\Leftrightarrow & x \cdot\left(x^2-3 x+2\right)=0 \\
\Leftrightarrow & x=0 \text { oder } x^2-3 x+2=0 \\
\Leftrightarrow & x=0 \text { oder } x=1 \text { oder } x=2
\end{array}
$$

#### Linearfaktoren von Polynomfunktionen

Hat ein **Polynom** $f(x)$ vom Grad $n$ die Nullstelle $x_0$, so $\operatorname{kann} f(x)$ als

$$
f(x)=\left(x-x_0\right) \cdot g(x)
$$

dargestellt werden. Dabei ist $g(x)$ ein anderes Polynom mit Grad $n-1$.
Der Faktor $\left(x-x_0\right)$ heißt **Linearfaktor**.

**Beispiel:**
Das Polynom

$$
f(x)=2 x^3-8 x^2+2 x+12
$$

hat die Nullstelle $x_0=3$ und kann geschrieben werden als

$$
f(x)=\underbrace{(x-3)}_{\text {Linearfaktor }} \cdot \underbrace{\left(2 x^2-2 x-4\right)}_{=g(x)}
$$

siehe dazu auch [[Linearfaktorzerlegung]]