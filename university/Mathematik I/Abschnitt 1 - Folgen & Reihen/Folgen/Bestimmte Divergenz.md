---
tags:
  - folgen
---
***

```ad-important
title: Definition
Eine Folge $\left(a_n\right)$ heißt bestimmt divergent mit dem Wert $\infty$ (bzw. $\left.-\infty\right)$, wenn für jedes $M \in \mathbb{R}$ ein $n_0 \in N$ existiert, sodass
$$
a_n \underset{(<)}{>} M \text { für alle } n \geq n_0
$$
```

- Wir schreiben
$$
\lim _{n \rightarrow \infty} a_n=\infty \quad \text { bzw. } \quad \lim _{n \rightarrow \infty} a_n=-\infty
$$
***
### Konvergenz und Divergenz von [[Arithmetische Folgen|arithmetischen]] & [[Geometrische Folgen| geometrischen Folgen]]

- Die arithmetische Folge
$$
a_n=a_0+n \cdot d, \quad n \geq 0
$$
mit $d \neq 0$ ist bestimmt divergent. Es gilt
$$
\lim _{n \rightarrow \infty} a_n=\lim _{n \rightarrow \infty} a_0+n \cdot d= \begin{cases}+\infty & \text { falls } d>0, \\ -\infty & \text { falls } d<0\end{cases}
$$

- Die geometrische Folge
$$
a_n=a_0 \cdot q^n, \quad n \geq 0
$$
- mit $a_0 \neq 0$ ist
	- für $|q|<1 \quad$ konvergent und es gilt $\lim _{n \rightarrow \infty} a_n=0$,
	- für $q>1$ bestimmt divergent,
	- für $q \leq-1$ divergent


(Für $q=1$ ist $a_n$ die konstante Folge $a_n=1 \stackrel{n \rightarrow \infty}{\longrightarrow} 1$ )

