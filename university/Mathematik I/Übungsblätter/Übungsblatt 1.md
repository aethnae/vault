---
tags:
  - folgen
  - reihen
  - übung
week: 2023-11-14
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

***
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

***
#### Aufgabe 1.3
Ein Unternehmen erhöht jede Woche seinen Output um $d=50$ Einheiten. Der Anfangsoutput in der ersten Woche betrage $a=100$ Einheiten. Nach wie vielen Wochen hat das Unternehmen einen (kumulativen) Gesamtoutput von $N=800$ erstmals erreicht oder überschritten?

$$
\sum_{i = 1}^{4} 100 + 50(i - 1) = 700
$$
$$
\sum_{i = 1}^{5} 100 + 50(i - 1) = 1000
$$

Daher hat das Unternehmen nach fünf Wochen erstmals einen kumulativen Gesamtoutput von 800 überschritten.

***
#### Aufgabe 1.4
Untersuchen Sie die Folge
$$
a_n=4 n^2-\frac{1}{2 n}, n=1,2, \ldots
$$
auf Monotonie.

$$
4n^2-\frac{1}{2 n} < 4(n+1)^{2} - \frac{1}{2(n+1)}
$$
$$
0 < 4(n+1)^{2} - \frac{1}{2(n+1)} - (4n^2-\frac{1}{2n})
$$
$$
4(n+1)^{2} - 4n^{2} - \frac{1}{2(n+1)} + \frac{1}{2n}
$$
$$
4((n+1)^{2} - n^{2}) - \frac{1}{2}\left( \frac{1}{n+1} - \frac{1}{n} \right)
$$
$$
4(n+1-n)(n+1+n)-\frac{1}{2}\left(\frac{n}{n(n+1)}-\frac{n+1}{n(n+1)}\right)
$$
$$
4(2 n+1)-\frac{1}{2} \cdot \frac{n-n-1}{n(n+1)}=\underbrace{4(2 n+1)}_{>0}+\underbrace{\frac{1}{2 n(n+1)}}_{>0}
$$
Da beide Summanden $4(2 n+1)$ und $\frac{1}{2 n(n+1)}$ für alle $n \geq 1$ positiv sind, gilt
$$
a_{n+1}-a_n>0 \Longleftrightarrow a_{n+1}>a_n \text { für alle } n \geq 1 \text {. }
$$
D.h. die Folge $\left(a_n\right)$ ist streng monoton wachsend.

***
#### Aufgabe 1.5
Gegeben sind die beiden Folgen
$$
a_n=\frac{n}{(n+2) 2^n} \quad \text { und } \quad b_n=2^n+5, \quad n=1,2, \ldots
$$

**a)**
Untersuchen Sie, ob die Folgen $a_n$ und $c_n:=a_n \cdot b_n, n=1,2, \ldots$, einen Grenzwert besitzen, und geben Sie diesen an, falls er existiert.

$$
a = \lim_{ n \to \infty } a_{n} = \lim _{n \rightarrow \infty} \frac{n}{(n+2) 2^n}=\lim _{n \rightarrow \infty} \frac{n}{n} \frac{1}{\left(1+\frac{2}{n}\right)} \cdot \frac{1}{2^n}=\lim _{n \rightarrow \infty} \frac{1}{\left(1+\frac{2}{n}\right)} \cdot \lim _{n \rightarrow \infty} \frac{1}{2^n}=1 \cdot 0=0
$$

$$
c = \lim_{ n \to \infty } c_{n} = \lim_{ n \to \infty } (a_{n} \cdot b_{n}) = \frac{n}{(n+2)2^{n}}(2^{n}+5) = \lim _{n \rightarrow \infty} \frac{n}{n} \frac{1}{\left(1+\frac{2}{n}\right)} \cdot \frac{2^n}{2^n}\left(1+\frac{5}{2^n}\right)
$$
$$
=\lim _{n \rightarrow \infty} \frac{1}{1+\frac{2}{n}} \cdot \lim _{n \rightarrow \infty}\left(1+\frac{5}{2^n}\right)=1(1+0)=\underline{\underline{1}}
$$

**b)**
Hat die Folge $d_n:=a_n+\frac{1}{b_n}, \quad n=1,2, \ldots$ einen Grenzwert? Falls ja, so bestimme man diesen.

$$
d = \lim_{ n \to \infty } d_{n} = \lim_{ n \to \infty } \frac{n}{(n+2)2^{n}} + \frac{1}{2^{n}+5} = 0 + 0 = 0
$$

***
#### Aufgabe 1.6
Die untenstehenden Folgen sind auf Häufungspunkte zu untersuchen.

**a)**
$a_{n} = \frac{2n(-1)^{n}}{n+1}$

$$
a_n=\frac{2 \cdot n \cdot(-1)^n}{n+1}=\overbrace{\frac{1}{\frac{1}{n}}}^{=n} \frac{2 \cdot(-1)^n}{(n+1)}=\frac{2 \cdot(-1)^n}{1+\frac{1}{n}}=\left\{\begin{array}{cl}
\frac{2}{1+\frac{1}{n}} & \text { für } n \text { gerade } \\
-\frac{2}{1+\frac{1}{n}} & \text { für } n \text { ungerade }
\end{array}\right.
$$

Die Teilfolge $a_{2 j}, j=1,2, \ldots$ der geraden Indizes konvergiert für $j \rightarrow \infty$ gegen 2.
Die Teilfolge $a_{2 j-1}, j=1,2, \ldots$ der ungeraden Indizes konvergiert für $j \rightarrow \infty$ gegen -2.
Daher sind 2 und -2 die Häufungspunkte der Folge $\left(a_n\right)$.

**b)**
$b_n=\left(1+(-1)^n\right) \frac{n}{n+1}$

$$
b_n=\left(1+(-1)^n\right) \frac{n}{n+1} = \left\{\begin{array}{cl}
\frac{2 n}{n+1} & \text { für } n \text { gerade } \\
0 & \text { für } n \text { ungerade }
\end{array}\right.
$$

Die Teilfolge $b_{2 j}=\frac{4 j}{2 j+1}, j=1,2, \ldots$ der geraden Indizes konvergiert für $j \rightarrow \infty$ gegen 2.
Die Teilfolge $b_{2 j-1}=0$ der ungeraden Indizes konvergiert für $j \rightarrow \infty$ gegen 0. 
Daher sind 0 und 2 die Häufungspunkte der Folge $b_n, n=1,2, \ldots$

***
### Tutoriumsaufgaben

#### Aufgabe 1.7
Für eine geometrische Folge $a_n$ mit $n \geq 1$ gelte:
$$
q=0,4 \quad \text { und } \quad s_4=\sum_{i=1}^4 a_i=812
$$

**(a)**
Geben Sie das explizite Bildungsgesetz dieser Folge an.

Gesucht ist die Größe $a_1$.
Aus der Formel für die geometrische Summe $s_n=a_1 \cdot \frac{1-q^n}{1-q}$ erhalten wir für $n=4$ mit $q=0,4$ die Gleichung
$$
s_4=a_1 \cdot \frac{1-0,4^4}{1-0,4}=812 .
$$

Wir lösen die Gleichung nach $a_1$ auf
$$
s_4=a_1 \cdot \frac{1-0,4^4}{1-0,4}=812 \Longrightarrow \underline{\underline{\underline{a_1}}}=812 \cdot \frac{1-0,4}{1-0,4^4}=\underline{\underline{500}} .
$$

Das explizite Bildungsgesetz ist somit
$$
a_n=500 \cdot 0,4^{n-1}, \quad n=1,2,3 \ldots
$$

**b)**
Bestimmen sie $a_{3}$ und $a_{5}$

Mit dem expliziten Bildungsgesetz aus (a) berechnen wir
$$
\begin{aligned}
& \underline{\underline{a_3}}=500 \cdot 0,4^2=500 \cdot 0,16=\underline{\underline{80}} \\
& \underline{\underline{a_5}}=500 \cdot 0,4^4=\overbrace{500 \cdot 0,16}^{a_3} \cdot \overbrace{0,16}^{q^2}=80 \cdot 0,16=\underline{\underline{12,8}} .
\end{aligned}
$$

***
#### Aufgabe 1.8
Es sei $\left(a_n\right), n \geq 1$ eine arithmetische Folge. Zeigen Sie, dass für jedes Glied $a_n$ mit $n \geq 2$ das arithmetische Mittel seiner Nachbarglieder $a_{n-1}$ und $a_{n+1}$ ist.

Aus dem rekursiven Bildungsgesetz der arithmetischen Folge $a_{n+1}=a_n+d$ bzw. $a_n=a_{n+1}-d, n \geq 1$ folgt

$$
\underline{\underline{\frac{1}{2}\left(a_{n-1}+a_{n+1}\right)}}=\frac{1}{2}\left(a_n-d+a_n+d\right)=\underline{\underline{a_n}} .
$$

***
#### Aufgabe 1.9
In $n-1$ Jahren wächst das Produktionsvolumen eines Unternehmens von $a_1>0$ auf den Wert $a_n$ an, wobei jedes Jahr eine (konstante) Steigerung um $p \%$ zu verzeichnen ist. Wie hoch muss $p$ sein, um die Steigerung von $a_1$ auf $a_n$ zu realisieren?

Die Produktionsmengen $a_n$ bilden eine geometrische Folge mit dem expliziten Bildungsgesetz
$$
a_n=a_1 \cdot q^{n-1}, \quad n \geq 1
$$
wobei $q$ der Wachstumsfaktor $q=1+\frac{p}{100}$ ist.

Gesucht ist die Größe $p$. Setzen wir $q$ in das explizite Bildungsgesetz ein, erhalten wir
$$
a_n=a_1\left(1+\frac{p}{100}\right)^{n-1} \quad \mid: a_1 \Longleftrightarrow \frac{a_n}{a_1}=\left(1+\frac{p}{100}\right)^{n-1}
$$

Ziehen wir auf beiden Seiten der Gleichung die $n$-1-te Wurzel folgt
$$
1+\frac{p}{100}=\sqrt[n-1]{\frac{a_n}{a_1}} \Longleftrightarrow \frac{p}{100}=\sqrt[n-1]{\frac{a_n}{a_1}}-1 \quad \text { und somit } \quad =100 \cdot\left(\sqrt[n-1]{\frac{a_n}{a_1}}-1\right)
$$

***
#### Aufgabe 1.10
Angenommen, ein Postunternehmen plant, Briefmarken von einem Automaten drucken zu lassen, und zwar von $0,05 €$ an aufwärts bis zu $99,95 €$ in Abständen von jeweils $0,05 €$. Wie viel müsste ein Sammler für deren Erwerb aufwenden?

$$
\frac{99,95}{0,05} = 1.999
$$
$$
\sum_{i = 1}^{1999} i \cdot 0,05 = 99.950
$$
Ein Sammler müsste für den Erwerb aller 1.999 Briefmarken 99.950€ aufwenden.

***
#### Aufgabe 1.11
Untersuchen Sie die Folge
$$
a_n=\frac{n+1}{n-1}, n=2,3, \ldots
$$
auf Monotonie.

$$
a_{n+1} \geq a_{n}
$$
$$
\frac{n+2}{n} \geq \frac{n+1}{n-1}
$$
$$
\frac{n+2}{n} - \frac{n+1}{n-1} \geq 0
$$
$$
\frac{n}{n} \cdot \frac{3}{1} - \frac{n + 1}{n - 1} \geq 0
$$
$$
3 \geq \frac{n+1}{n - 1} \quad \text{ für } n \geq 2
$$

***
### Selbstrechenaufgaben

#### Aufgabe 1.12
Für eine arithmetische Folge $a_n$ mit $n \geq 1$ gelte: $\quad a_{18}-a_8=60, \quad a_5=38$.

**a)**
Geben Sie das explizite Bildungsgesetz dieser Folge an.

Gesucht sind die Größen $a_1$ und $d$.
Wir setzen zunächst $n=18$ und $n=8$ in die Formel ein und betrachten die Gleichung $a_1 8-a_8=60$.

$$
a_{18}-a_8=60 \Rightarrow a_1+17 \cdot d-\left(a_1+7 \cdot d\right)=a_1+17 d-a_1-7 d=10 d=60 \Rightarrow \underline{\underline{d=6}}
$$

Setzen wir $d=6$ in die Voraussetzung $a_5=38$ ein, folgt

$$
a_5=a_1+4 \cdot 6=38 \Rightarrow \underline{\underline{a_1}=14}
$$

Die explizite Bildungsvorschrift ist somit

$$
\underline{\underline{a_n=14+(n-1) \cdot 6}}, \quad n \geq 1
$$

**b)**
Bestimmen Sie $a_8, a_{18}$ und die Partialsumme $s_8=\displaystyle \sum_{i=1}^8 a_i$

Setzen wir $n=8$ und $n=18$ in das explizite Bildungsgesetz ein, folgt

$$
\begin{gathered}
a_8=14+7 \cdot 6=\underline{\underline{56}} \\
a_{18}=14+17 \cdot 6=\underline{\underline{116}}
\end{gathered}
$$

Für die Partialsumme $s_n=a_1+\ldots+a_n, n \geq 1$, kann die Formel $s_n=\frac{n}{2}\left(2 a_1+(n-1) \cdot d\right)$ verwendet werden. Für $n=8$ folgt somit

$$
\underline{\underline{s_8}}=a_1+\ldots+a_8=\frac{8}{2}(2 \cdot 14+7 \cdot 6)=\underline{\underline{280}} .
$$

**c)**
Bestimmen Sie $n$, so dass $a_n=68$ gilt.

Gesucht ist $n \geq 1$ so dass $a_n=14+(n-1) \cdot 6=68$ gilt.

$$
a_n=14+(n-1) \cdot 6=68 \Rightarrow(n-1) \cdot 6=54 \Rightarrow n-1=9 \Rightarrow \underline{n=10}
$$

***
#### Aufgabe 1.13
Für eine geometrische Folge $a_n$ mit $n \geq 1$ gelte:
$$
a_3=64 \text { und } a_5=40,96 \text {. }
$$

Bestimmen Sie die Größen $a_1, q, a_4$ und $\displaystyle \sum_{i=1}^4 a_i$.

***
#### Aufgabe 1.14
In einer Firma soll innerhalb eines Jahres eine monatliche Produktionserhöhung von $3 \%$ erreicht werden. Im Monat Januar betrug die Produktion 1000 Stück.

**a)**
Bestimmen sie die Produktion für den Monat Juli.

$$
a_{n} = 1000 \cdot 1,03^{n}
$$
$$
a_{6} = 1000 \cdot 1,03^{6} \approx 1.194,05
$$

**b)**
In welchem Monat werden ungefähr 1126 Stück produziert?

$$
1126 = 1000 \cdot 1,03^{n} \Leftrightarrow \frac{1126}{1000} = 1,03^{n} \Leftrightarrow \log_{1,03}(1,03^{n}) = {\log_{1,03}} \frac{1126}{1000} \Leftrightarrow n \approx 5,015 
$$

d.h. im Monat Mai werden fast 1126 Stück produziert. Im Juni werden bereits mehr als 1126 Stück produziert.

**c)**
Wie hoch ist die Jahresproduktion?

Gesucht ist hier
$$
s_n=a_1+a_2+\ldots+a_{12}=\sum_{j=1}^{12} a_j=\sum_{j=1}^{12}(1,03)^{j-1} \cdot a_1
$$

Mit der Formel für die geometrische Summe $s_n=\displaystyle \sum_{j=1}^n a_1 q^{j-1}=a_1 \cdot \frac{1-q^n}{1-q}$ erhalten wir
$$
\underline{\underline{s_{12}}}=a_1 \cdot \frac{1-1,03^{12}}{1-1,03} \approx \underline{\underline{14192}} \text { [Stück] }
$$

***
#### Aufgabe 1.15
Im Gründungsjahr 2002 produzierte eine Unterhaltungselektronikfirma 100.000 DVD-Player.

**a)**
Wie viele DVD-Player wurden insgesamt bis Ende 2013 hergestellt, wenn das Unternehmen ihre produzierte Stückzahl gegenüber dem Vorjahr jeweils um 10.000 Stück steigerte?

$$
a_{n} = 100.000 + n \cdot 10.000
$$
$$
s_{a} = \sum_{i = 1}^{11} 100.000 + (n - 1) \cdot 10.000 = 
$$