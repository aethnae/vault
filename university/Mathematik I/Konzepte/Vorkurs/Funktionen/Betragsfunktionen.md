---
tags:
  - funktionen
week: 2023-10-31
flashcard: true
---
***

```ad-important
title: Definition
Die reellwertige Funktion $f: \mathbb{R} \rightarrow \mathbb{R}$ definiert durch
$$
x \mapsto|x|=\left\{\begin{aligned}
-x & \text { falls } x<0 \\
x & \text { falls } x \geq 0
\end{aligned}\right.
$$
heißt Betragsfunktion.
```

- Die Betragsfunktion ist eine zusammengesetze Funktion
- Sie besteht aus zwei Teilen: Der Funktion $f_1(x)=-x$ für negative Eingabewerte und der Funktion $f_2(x)=x$ für nicht-negative Eingabewerte.
- Die Betragsfunktion gibt den Eingabewert ohne Vorzeichen zurück.
- Die Betragsfunktion besteht aus zwei Geraden:
$$
|x|=\left\{\begin{aligned}
-x & \text { falls } x<0 \\
x & \text { falls } x \geq 0
\end{aligned}\right.
$$
- Die Betragsfunktion hat ein Minimum im Ursprung $(0,0)$

$$
\text{Verallgemeinerte Betragsfunktion:} f(x)=a|x+b|+c
$$

- Besteht aus zwei Geraden mit Steigung - $a$ bzw. $a$, die bei $x=-b$ aneinander stoßen
- Hat ein Minimum im Punkt $(-b, c)$

![[Pasted image 20231105181708.png|center|300]]

#### Betragsgleichungen

- Die Betragsfunktion funktioniert unterschiedlich für $x<0$ und $x \geq 0$
- Fallunterscheidung zum Lösen nötig

**Folgende Umformung ist eine Äquivalenzumformung:**
- Fallunterscheidung bezüglich Vorzeichen:

$$
|g(x)|=c \Leftrightarrow \underbrace{(-g(x)=c \text { und } g(x)<0)}_{\text {Fall } 1} \text { oder } \underbrace{(g(x)=c \text { und } g(x) \geq 0)}_{\text {Fall } 2}
$$

wobei $c \in \mathbb{R}$.

- Fallunterscheidung bezüglich Nullstellen der Funktion im Betrag, z.B.:

$$
|x-a|=c \Leftrightarrow(-(x-a)=c \text { und } x<a) \text { oder }((x-a)=c \text { und } x \geq a)
$$