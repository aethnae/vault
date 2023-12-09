---
tags:
  - funktionen
week: 2023-12-05
flashcard: false
publish: true
---
***

> [!abstract] Definition 
> Eine Funktion der Art
> 
> $$
> f(x)=\frac{p(x)}{q(x)},
> $$
> 
> wobei
> 
> $$
> \begin{aligned}
> & p(x)=a_n x^n+a_{n-1} x^{n-1}+\ldots+a_2 x^2+a_1 x+a_0 \\
> \text { und } & q(x)=b_m x^m+b_{m-1} x^{m-1}+\ldots+b_2 x^2+b_1 x+b_0
> \end{aligned}
> $$
> 
> zwei Polynome vom Grad $n$ bzw. $m$ sind, nennen wir **rationale Funktion**.

***
#### Polstellen

> [!abstract] Definition 
> Eine Zahl $x_0$ heißt **$k$-fache Nullstelle** eines Polynoms $q(x)$, falls
> 
> $$
> q(x)=\left(x-x_0\right)^k \tilde{q}(x)
> $$
> 
> ist und $\tilde{q}\left(x_0\right) \neq 0$ gilt. Wir sagen auch: Die Nullstelle $x_0$ tritt $k$-mal auf.

- Angenommen, $p(x)$ und $q(x)$ haben keine gemeinsamen Nullstellen. Dann heißt eine Nullstelle, die in $q(x)$ genau $k$-mal auftritt, Pol der Ordnung $k$ der rationalen Funktion

$$
f(x) = \frac{p(x)}{q(x)}
$$

***
#### Verhalten im Unendlichen

**Gegeben:**
Rationale Funktion $f(x)=\frac{p(x)}{q(x)}$ mit $n=\operatorname{Grad}$ von $p(x), m=$ Grad von $q(x)$

**Fall 1**:
$n<m$. Dann gilt

$$
\lim _{x \rightarrow \pm \infty}|f(x)|=0
$$

**Fall 2**:
$n \geq m$. Dann ergibt Polynomdivison

$$
f(x)=p_1(x)+\frac{r(x)}{q(x)},
$$

wobei $r(x)$ ein Polynom vom Grad $k<m$ ist.

In diesem Fall gilt:

- $f(x)$ nähert sich für $x \rightarrow \pm \infty$ der Funktion $p_1(x)$ an
- Die Funktion $p_1(x)$ heißt **Grenzkurve** oder **Asymptote**

***
##### Beispiel 1 ($n < m$)

Rationale Funktion

$$
f(x)=\frac{p(x)}{q(x)}=\frac{3(x-2)}{(x-1)^2(x+2)}=\frac{3 x-6}{x^3-3 x+2}
$$

Es gilt
- Grad von $p(x)$ ist $n=1$
- Grad von $q(x)$ ist $m=3$
- Also $\displaystyle n<m \Rightarrow \lim _{x \rightarrow \pm \infty}|f(x)|=0$

![[Pasted image 20231209221359.png|350]]
***
##### Beispiel 2 ($n \geq m$)

Rationale Funktion

$$
f(x)=\frac{p(x)}{q(x)}=\frac{x^2-1}{x^2+1}
$$

Es gilt
- Grad von $p(x)$ ist $n=2$
- Grad von $q(x)$ ist $m=2$

Polynomdivison liefert

$$
f(x)=\frac{x^2-1}{x^2+1}=\frac{x^2+1-2}{x^2+1}=1-\frac{2}{x^2+1}
$$

mit

$$
\begin{aligned}
p_1(x) & =1 \\
r(x) & =-\frac{2}{x^2+1}
\end{aligned}
$$


![[Pasted image 20231209221524.png|350]]
***
##### Beispiel 3 ($n > m$)

Rationale Funktion

$$
f(x)=\frac{p(x)}{q(x)}=\frac{x^3}{x^2-1}
$$

Es gilt
- Grad von $p(x)$ ist $n=3$
- Grad von $q(x)$ ist $m=2$

Polynomdivison liefert

$$
f(x)= \frac{x^3}{x^2-1}=x+\frac{x}{x^2-1}
$$

mit

$$
\begin{align}
 & p_{1}(x) = x \\
 & r(x) = \frac{x}{x^{2} - 1}
\end{align}
$$

![[Pasted image 20231209222440.png|350]]
