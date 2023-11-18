---
tags:
  - folgen
  - reihen
week: "1"
---
***
### Übungsaufgaben

##### Aufgabe 1.1
Gegeben sind für $n \in \mathbb{N}$ die Folgen
$$
a_n=3 n+2, \quad b_n=6 \cdot 4^n, \quad c_n=0,49^{\frac{n+1}{2}}, \quad d_n=n+\ln (3), \quad e_n=\frac{4}{n+3}
$$

Welche Folgen sind
**(i)** arithmetische Folgen
**(ii)** geometrische Folgen
**(iii)** weder arithmetische noch geometrische Folgen?

**(i)**
$a_{n} = 3n + 2$ ist eine arithmetische Folge, da $a_{n + 1} - a_{n} = d = 3$

$d_{n} = \ln(3)$ ist eine arithmetische Folge, da $a_{n+1} - a_{n} = d = 1$

**(ii)**
$b_{n} = 6 \cdot 4^n$ ist eine geometrische Folge, da $\frac{a_{n+1}}{a_{n}} = q = 4$

$c_{n} = 0.49^{\frac{n + 1}{2}}$ ist eine geometrische Folge, da 
$$
\frac{c_{n+1}}{c_{n}} = \frac{0.49^{\frac{n+2}{2}}}{0.49^{\frac{n+1}{2}}} = 0.49^{\frac{n+2}{2} - \frac{n+1}{2}} = 0.49^{\frac{n+2-n-1}{2}} = \sqrt{ 0.49 } = 0.7 = q
$$

**(iii)**
weder arithmetische noch geometrische Folge ist $e_n$, denn für $n=1,2, \ldots$ ist
$$
e_{n+1}-e_n=\frac{4}{n+4}-\frac{4}{n+3}=\frac{4(n+3)-4(n+4)}{(n+4) \cdot(n+3)}=\frac{-4}{(n+4) \cdot(n+3)}
$$
nicht konstant und für $n=1,2, \ldots$ ist auch
$$
\frac{e_{n+1}}{e_n}=\frac{\frac{4}{n+4}}{\frac{4}{n+3}}=\frac{4(n+3)}{4(n+4)}=\frac{n+3}{n+4}
$$
nicht konstant.