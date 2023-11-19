---
tags:
  - Präferenzen
week: 2023-10-25
flashcard: true
---
***

```ad-important
title: Definition
Die **Präferenzrelation** $\succeq$ ist auf dem gesamten Güterraum $X=\mathbb{R}_{+}^n$ definiert.
$\succeq$ vergleicht paarweise und drückt **schwaches Bevorzugen** aus: Konnis Präferenz $x \succeq y$ : "Konni mag $x$ mindestens so sehr wie $y$."

Äquivalente Interpretation: "Wenn Konni aus dem Paar $(x, y)$ auswählen soll, ist sie willens, $x$ zu wählen."

```

```ad-important
title: Definition
$\succ: x \succ y$ genau dann wenn gilt, dass $x \succeq y$ und $y \nsucceq x$. Konni mag $x$ mehr als $y$.

```

```ad-important
title: Definition
$\sim: x \sim y$ genau dann wenn gilt, dass $x \succeq y$ und $y \succeq x$. Konni mag $x$ genauso sehr wie $y$.
```

***
#### Axiome über Präferenzen

**Vollständigkeit:**
Wir nehmen an, dass alle beliebigen Bündel miteinander verglichen werden können. Das heißt, für jedes beliebige $x$-Bündel und jedes beliebige $y$-Bündel gilt entweder $\left(x_1, x_2\right) \succeq\left(y_1, y_2\right)$ oder $\left(y_1, y_2\right) \succeq\left(x_1, x_2\right)$ oder beides; im letzten Fall wäre der Konsument zwischen den zwei Bündeln indifferent.

**Reflexivität:**
Wir nehmen an, dass jedes Bündel mindestens so gut ist, wie es selbst: $\left(x_1, x_2\right) \succeq\left(x_1, x_2\right)$.

**Transitivität:**
Wenn $\left(x_1, x_2\right) \succeq\left(y_1, y_2\right)$ und $\left(y_1, y_2\right) \succeq\left(z_1, z_2\right)$, dann nehmen wir an, dass $\left(x_1, x_2\right) \succeq \left(z_1, z_2\right)$. Mit anderen Worten, wenn der Konsument glaubt, dass $X$ mindestens so gut ist wie $Y$, und $Y$ wiederum mindestens so gut wie $Z$, dann glaubt der Konsument, dass $X$ mindestens so gut ist wie $Z$.