---
tags:
  - funktionen
  - grenzwerte
  - stetigkeit
week: 2023-12-15
flashcard: false
publish: true
---
***

*Wir verallgemeinern in diesem Abschnitt die Begriffe von Konvergenz und Stetigkeit auf Funktionen mit zwei Variablen. Auf die gleiche Weise können diese Begriffe auch für Funktionen mit mehr Variablen verallgemeinert werden.*

#### Konvergenz

> [!abstract] Definition 
> Eine Folge $P_n=\left(x_n, y_n\right), n \geq 1$ von Punkten in $\mathbb{R}^2$ konvergiert gegen den Punkt $P_0=\left(x_0, y_0\right)$, wenn
> 
> $$
> \lim _{n \rightarrow \infty} x_n=x_0 \quad \text { und } \quad \lim _{n \rightarrow \infty} y_n=y_0
> $$
> 
> gilt.

**Bemerkung:**
$\left(x_n, y_n\right) \stackrel{n \rightarrow \infty}{\longrightarrow}\left(x_0, y_0\right)$ ist äquivalent zu:

Für jedes $\epsilon>0$ gibt es ein $n_0 \in \mathbb{N}$, sodass für alle $n \geq n_0$

$$
\underbrace{\sqrt{\left|x_n-x_0\right|^2+\left|y_n-y_0\right|^2}}_{\text {Abstand von }\left(x_n, y_n\right) \text { zu }\left(x_0, y_0\right)}<\epsilon
$$
gilt.

![[Pasted image 20231220154243.png|center|300]]

***
#### Funktionsgrenzwerte

> [!abstract] Definition 
> Konvergiert für jede beliebige gegen $P_0=\left(x_0, y_0\right)$ konvergierende Folge $P_n=\left(x_n, y_n\right), n \geq 1$ die Folge der Funktionswerte
> 
> $$
> f\left(x_n, y_n\right), n \geq 1
> $$
> 
> gegen einen festen Wert $z$, so heißt $z$ der Grenzwert der Funktion $f$ an der Stelle $\left(x_0, y_0\right)$.
> Wir schreiben
> 
> $$
> z=\lim _{(x, y) \rightarrow\left(x_0, y_0\right)} f(x, y) .
> $$

***
##### Beispiel für