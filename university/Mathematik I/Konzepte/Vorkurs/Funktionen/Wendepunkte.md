---
tags:
  - funktionen
week: 
flashcard: false
---
***

```ad-important
title: Definition
Es sei $f: D \rightarrow \mathbb{R}$ eine differenzierbare Funktion.
Eine lokale Extremstelle $x_0$ der ersten Ableitung $f^{\prime}$ heißt Wendestelle von $f$. Der dazugehörige Punkt $\left(x_0, f\left(x_0\right)\right)$ heißt Wendepunkt.
```

- Ein Wendepunkt von $f$ ist ein (lokales) Maximum oder Minimum der Steigung $f'$
- Bei einem Wendepunkt ändert sich die Veränderung der Steigung (Krümmung).

![[Pasted image 20231107225629.png|center|600]]

***

```ad-note
title: Notwendige Bedingung für Wendepunkte
Es sei $\left(x_0, f\left(x_0\right)\right)$ ein Wendepunkt einer zweimal differenzierbaren Funktion $f: D \rightarrow \mathbb{R}$. Dann gilt
$$
f^{\prime \prime}\left(x_0\right)=0 .
$$
```

```ad-note
title: Hinreichende Bedingung für Wendepunkte
Es sei $f: D \rightarrow \mathbb{R}$ eine dreimal differenzierbare Funktion. Wenn für $x_0 \in D$
- $f^{\prime \prime}\left(x_0\right)=0$ und
- $f^{\prime \prime \prime}\left(x_0\right) \neq 0$
gilt, dann ist $\left(x_0, f\left(x_0\right)\right)$ ein Wendepunkt von $f$.

```

***
#### Sattelpunkte

```ad-important
title: Definition
Ein stationärer Punkt $\left(x_0, f\left(x_0\right)\right)$ einer differenzierbaren Funktion $f$ (d.h. ein Punkt mit $f^{\prime}\left(x_0\right)=0$ ), der kein lokales Extremum ist, heißt Sattelpunkt.

```

- Ein Sattelpunkt ist ein Wendepunkt, in dem die Steigung gleich 0 ist

![[Pasted image 20231107230041.png|center|300]]
