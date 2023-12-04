---
tags:
  - ableitungen
week: 2023-12-01
flashcard: false
publish: true
---
***

> [!abstract] Definition
> Es sei $f$ eine Funktion, die im Intervall $\left[x_0, x\right](n+1)$-mal stetig differenzierbar ist. Dann gibt es ein $t \in] x_0, x\left[\right.$ (abhängig von $x, x_0$ und $n$ ), sodass gilt
> $$
> f(x)=\sum_{k=0}^n \frac{f^{(k)}\left(x_0\right)}{k !}\left(x-x_0\right)^k+R_{n, x_0}(x)=T_{n, x_0}(x)+R_{n, x_0}(x),
> $$
> wobei
> $$
> T_{n, x_0}(x)=\sum_{k=0}^n \frac{f^{(k)}\left(x_0\right)}{k !}\left(x-x_0\right)^k
> $$
> das n-te Taylorpolynom von $f$ bezüglich der Stelle $x_0$ ist und
> $$
> R_{n, x_0}(x)=\frac{f^{(n+1)}(t)}{(n+1) !}\left(x-x_0\right)^{n+1}
> $$
> das Lagrangesche Restglied ist.

$$
f(x)=\underbrace{T_{n, x_0}(x)}_{\text {Taylorpolynom }}+\underbrace{R_{n, x_0}(x)}_{\begin{array}{c}
\text { Lagrangesches Restglied } \\
\hat{=} \text { Approximationsfehler }
\end{array}}
$$
- Das Restglied $R_{n, x_0}(x)$ hat die gleiche Struktur wie die anderen Glieder des Taylorpolynoms, aber die Ableitung wird bei einem Zwischenwert $t$ und nicht bei $x_0$ berechnet
- Das Restglied lässt sich i.A. nicht explizit berechnen
- Die Existenzaussage $t \in ]x_{0}, x[$ ermöglicht für gegebene $x_{0}, x$ eine Abschätzung des Fehlers $\mid R_{n, x_{0}}(x)\mid$
