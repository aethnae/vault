---
tags:
  - polynome
  - ableitungen
week: 2023-12-01
flashcard: true
publish: true
---
***

Wir wissen: Für Werte $x$ nahe bei $x_0$ gilt
$$
f(x) \approx \underbrace{f\left(x_0\right)+f^{\prime}\left(x_0\right)\left(x-x_0\right)}_{\begin{array}{c}
=T_{1, x_0}(x) \\
\text { Tangente im Punkt } x_0
\end{array}}
$$

- Nahe bei $x_0$ lässt sich $f$ gut durch die Tangente $T_{1, x_0}$ in $x_0$ **approximieren**
- Die Tangente $T_{1, x_0}$ ist ein [[Polynomfunktionen|Polynom]] vom Grad 1 und es gilt
	- $f\left(x_0\right)=T_{1, x_0}\left(x_0\right)$
	- $f^{\prime}\left(x_0\right)=T_{1, x_0}^{\prime}\left(x_0\right)$
$\rightarrow f$ und $T_{1, x_0}$ **stimmen** in $x_0$ in Funktions- und Ableitungswert **überein**
- Notation $T_{1, x_0}$, da Polynom **1. Grades** angelegt an $f$ an der **Stelle $x_0$**

***
#### Approximation 2. Ordnung

> [!abstract] Idee
> Approximation wird besser mit höherem Grad des Polynoms

**Ansatz**: Polynom vom Grad 2

$$
T_{2, x_0}(x)=A+B\left(x-x_0\right)+C\left(x-x_0\right)^2
$$

sodass an der Stelle $x_0$ gilt

(i) $T_{2, x_0}\left(x_0\right)=f\left(x_0\right)$
(ii) $T_{2, x_0}^{\prime}\left(x_0\right)=f^{\prime}\left(x_0\right)$
(iii) $T_{2, x_0}^{\prime \prime}\left(x_0\right)=f^{\prime \prime}\left(x_0\right)$

***
#### Approximation höherer Ordnung

> [!abstract] Ansatz
> Ansatz: Polynom vom Grad $n$
> $$
> T_{n, x_0}(x)=A_0+A_1\left(x-x_0\right)+A_2\left(x-x_0\right)^2+\cdots+A_n\left(x-x_0\right)^n
> $$
> 
> sodass an der Stelle $x_0$ gilt
> $$
> T_{n, x_0}\left(x_0\right)=f\left(x_0\right) \quad T_{n, x_0}^{\prime}\left(x_0\right)=f^{\prime}\left(x_0\right) \quad T_{n, x_0}^{\prime \prime}\left(x_0\right)=f^{\prime \prime}\left(x_0\right) \quad \ldots \quad T_{n, x_0}^{(n)}\left(x_0\right)=f^{(n)}\left(x_0\right)
> $$

Es ergibt sich

$$
A_k=\frac{f^{(k)}\left(x_0\right)}{k !} \quad \text { für } k=0,1,2, \ldots, n
$$

und damit

$$
\begin{align}
 & T_{n, x_0}(x) \\
 & =f\left(x_0\right)+f^{\prime}\left(x_0\right)\left(x-x_0\right)+\frac{f^{\prime \prime}\left(x_0\right)}{2}\left(x-x_0\right)^2+\cdots+\frac{f^{(n)}\left(x_0\right)}{n !}\left(x-x_0\right)^n \\
 & =\sum_{k=0}^n \frac{f^{(n)}\left(x_0\right)}{k !}\left(x-x_0\right)^n
\end{align}
$$

was auch als [[Satz von Taylor]] bezeichnet wird.