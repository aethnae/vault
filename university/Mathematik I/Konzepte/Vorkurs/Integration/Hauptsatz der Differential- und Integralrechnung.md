---
tags:
week:
flashcard: false
---
***

```ad-important
title: Definition
Sei $f:[a, b] \rightarrow \mathbb{R}$ eine stetige* Funktion. Dann gilt - Die Funktion
$$
F(x)=\int_0^x f(t) \mathrm{d} t
$$
ist eine Stammfunktion von $f$.
- Jede Stammfunktion $F$ von $f$ erfüllt
$$
\int_a^b f(x) \mathrm{d} x=F(b)-F(a)=[F(x)]_a^b
$$

Eine Funktion $F$ mit $F^{\prime}(x)=f(x)$ heißt Stammfunktion von $f$.
```

- Die Stammfunktion heißt auch unbestimmtes Integral
- Wenn $F(x)$ eine Stammfunktion von $f(x)$ ist, dann ist $F(x)+c$ auch eine Stammfunktion
- Wir schreiben deshalb
$$
\int f(x) \mathrm{d} x=F(x)+c \quad \text { mit } c \in \mathbb{R}
$$
- Die Berechnung eines Integrals reduziert sich auf das Bestimmen einer Stammfunktion
- Integration ist der umgekehrte Vorgang zum Ableiten

$$
\begin{array}{c|cccccccc}
f(x) & 0 & 1 & x & \begin{array}{c}
x^p \\
p \neq-1
\end{array} & \frac{1}{x} & e^x & \sin x & \cos x \\
\hline F(x) & 1 & x & \frac{1}{2} x^2 & \frac{1}{p+1} x^{p+1} & \ln |x| & e^x & -\cos x & \sin x
\end{array}
$$

***
#### Linearität des Integrals

```ad-important
Für zwei stetige Funktionen $f, g:[a, b] \rightarrow \mathbb{R}$ und $c \in \mathbb{R}$ gilt
$$
\begin{aligned}
\int_a^b c \cdot f(x) \mathrm{d} x & =c \cdot \int_a^b f(x) \mathrm{d} x \\
\int_a^b f(x)+g(x) \mathrm{d} x & =\int_a^b f(x) \mathrm{d} x+\int_a^b g(x) \mathrm{d} x
\end{aligned}
$$

```
