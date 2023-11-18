---
tags:
  - folgen
  - reihen
week: "1"
---
***
### Übungsaufgaben

#### Aufgabe 1.1
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

#### Aufgabe 1.2
Für eine arithmetische Folge $a_n$ mit $n \geq 1$ gelte: $\quad a_{15}=37, \quad a_{20}=117$.

**a)**
Geben sie das explizite Bildungsgesetz dieser Folge an.

$$
a_{20} - a_{15} = 117 - 37 = 80
$$
$$
\frac{80}{5} = 16 = d
$$
$$
a_{0} = 37 - 15 \cdot 16 = -203
$$
$$
a_{n} = -203 + 16n \text{ mit n} \in \mathbb{N}
$$

**b)**
Bestimmen Sie $a_{10}$ und die Partialsumme $s_{10}=\displaystyle\sum_{i=1}^{10} a_i$.

siehe Notizbuch

#### Aufgabe 1.3
Ein Unternehmen erhöht jede Woche seinen Output um $d=50$ Einheiten. Der Anfangsoutput in der ersten Woche betrage $a=100$ Einheiten. Nach wie vielen Wochen hat das Unternehmen einen (kumulativen) Gesamtoutput von $N=800$ erstmals erreicht oder überschritten?

$$
\sum_{i = 1}^{4} 100 + 50(i - 1) = 700
$$
$$
\sum_{i = 1}^{5} 100 + 50(i - 1) = 1000
$$

Daher hat das Unternehmen nach fünf Wochen erstmals einen kumulativen Gesamtoutput von 800 überschritten.

#### Aufgabe 1.4
Untersuchen Sie die Folge
$$
a_n=4 n^2-\frac{1}{2 n}, n=1,2, \ldots
$$
auf Monotonie.

