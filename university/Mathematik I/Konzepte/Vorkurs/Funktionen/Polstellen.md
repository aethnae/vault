---
tags:
  - funktionen
week: 2023-11-03
flashcard: true
---
***

> [!important] Definition
> Ein Wert $x_0 \in \mathbb{R}$ heißt Polstelle einer Funktion $f: D \rightarrow \mathbb{R}$, falls
> $$
> \lim _{x \uparrow x_0} f(x)= \pm \infty \text { oder } \lim _{x \downarrow x_0} f(x)= \pm \infty
> $$

- An einer Polstelle wird die Funktion unendlich groß / klein
- Polstellen treten bei rationalen Funktionen $f(x) = \frac{g(x)}{h(x)}$ an den Nullstellen der Nennerfunktion $h(x)$ auf

![[Pasted image 20231105194314.png|center|500]]

#### Bestimmung von Polstellen

**Gegeben**: Rationale Funktion $f(x)=\frac{g(x)}{h(x)}$
**Gesucht**: Polstellen

- Bestimme Nullstellen $x_i$ vom Zähler und Nullstellen $y_i$ des Nenners. Die Funktion kann geschrieben werden als

$$
f(x)=\frac{\left(x-x_1\right) \cdot \ldots \cdot\left(x-x_n\right) \cdot \tilde{g}(x)}{\left(x-y_1\right) \cdot \ldots \cdot\left(x-y_m\right) \cdot \tilde{h}(x)}
$$

1. Kürze Linearfaktoren wenn möglich 
2. Zähle Vielfachheit der Nullstellen $y_i$ des Nenners
	- Ungerade Vielfachheit von $y_i \rightarrow$ Polstelle mit Vorzeichenwechsel bei $y_i$
	- Gerade Vielfachheit von $y_i \rightarrow$ Polstelle ohne Vorzeichenwechsel bei $y_i$
3. Grenzverhalten an der Polstelle kann z.B. durch Einsetzen von Werten nah an der Polstelle bestimmt werden

