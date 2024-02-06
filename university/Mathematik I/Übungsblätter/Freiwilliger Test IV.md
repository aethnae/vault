---
tags:
  - übung
week: 2024-01-23
flashcard: false
publish: true
source: 
date created: Tuesday, January 23rd 2024, 7:36:52 pm
date modified: Tuesday, January 23rd 2024, 7:37:04 pm
---
***
##### 1. Aufgabe
*Gegeben ist eine Produktionsfunktion*

$$
z=f(x, y)=5 x \sqrt{y}+2(x+y)+\frac{100 x}{y} \quad \text { für } x, y>0 .
$$

**(a)**
*Bestimmen Sie die partiellen Ableitungen und das totale Differential.*

**(b)**
*Wie verändert sich näherungsweise der Wert der Funktion, wenn ausgehend vom Punkt $(x, y)=(50,100)$ der $x$-Wert um 1,5 erhöht wird und der $y$-Wert um 2 verringert wird? Hinweis: Nutzen Sie das totale Differential.*

**(c)**
*Berechnen Sie die partielle Elastizität der Funktion bezüglich $y$ für $x=50$ und $y=100$.*

***

**(a)**

**Partielle Ableitungen:**

$$
\begin{align}
\frac{ \partial f }{ \partial x }  & = 5\sqrt{ y }+2+\frac{100}{y} \\
\frac{ \partial f }{ \partial y }  & = \frac{5x}{2\sqrt{ y }}+2+100x\cdot(-y^{-2}) \\
\frac{ \partial^{2} f }{ \partial x^{2} }  & = 0 \\
\frac{ \partial^{2} f }{ \partial y^{2} }  & = \frac{5x}{2} \cdot \left( -\frac{1}{2} y^{-3/2} \right) + 100x \cdot 2y^{-3} = -\frac{5x}{4y^{3/2}} + \frac{200x}{y^{3}} \\
\frac{ \partial^{2} f }{ \partial y \partial x }  & = \frac{ \partial^{2} f }{ \partial x \partial y } = \frac{5}{2\sqrt{ y }} - \frac{100}{y^{2}} 
\end{align}
$$

**Totales Differential:**

$$
\mathrm{d}f = \frac{ \partial f }{ \partial x } \mathrm{d}x + \frac{ \partial f }{ \partial y } \mathrm{d}y = (5\sqrt{ y }+2+\frac{100}{y}) \mathrm{d}x + (\frac{5x}{2\sqrt{ y }}+2+100x\cdot(-y^{-2})) \mathrm{d}y 
$$

**(b)**

${} \mathrm{d}f$ an der Stelle $(50, 100)$:

$$
\begin{align}
\mathrm{d}f  & = \left( 5\sqrt{ 100 }+2+\frac{100}{100} \right) \mathrm{d}x + \left( \frac{5\cdot 50}{2\sqrt{ 100 }}+2+100\cdot 50 \cdot(-100^{-2}) \right) \mathrm{d}y \\
 & = 53\mathrm{d}x + \left( 14,5 - \frac{5000}{100^{2}} \right) \mathrm{d}y \\
 & = 53\mathrm{d}x + 14\mathrm{d}y
\end{align}
$$

Veränderung einsetzen liefert $53 \cdot 1,5 + 14 \cdot (-2) = 79,5 - 28 = 51,5$. Somit verändert sich der Funktionswert ausgehend von $(50, 100)$ bei entsprechenden $x$- und $y$-Veränderungen um $51,5$.

**(c)**

$$
\begin{align}
\epsilon_{f, y} (50, 100) & = \frac{ \partial f }{ \partial y } \cdot \frac{100}{f} \\
 & = \frac{100 \cdot \frac{5 \cdot 50}{2\sqrt{ 100 }} + 2 + 100 \cdot 50 \cdot (-100^{-2})}{\left( 5 \cdot 50 \cdot \sqrt{100} + 2(150) + \frac{100 \cdot 50}{100} \right)} \\
 & = \frac{14 \cdot 100}{2850} \\
 & = \frac{140}{285} \\
 & = \frac{28}{57} \approx 0,49
\end{align}
$$

***
##### 2. Aufgabe
*Betrachtet wird die Funktion*

$$
G(x, y)=5 x \cdot\left(\frac{x^2}{6}+2 x+y\right)+5 y^2 .
$$

**(a)**
*Bestimmen Sie die partiellen Ableitungen erster und zweiter Ordnung der Funktion $G(x, y)$. Geben Sie die Hessematrix sowie ihre Determinante in Abhängigkeit von $x$ und $y$ an.*

**(b)**
*Berechnen Sie alle Stellen an denen $G(x, y)$ lokale Extrema bzw. Sattelpunkte besitzt und bestimmen Sie was jeweils vorliegt.*

***

**(a)**

**Partielle Ableitungen:**

$$
\begin{align}
\frac{ \partial G }{ \partial x }  & = \frac{15}{6}x^{2} + 20x + 5y \\
\frac{ \partial G }{ \partial y }  & = 5x + 10y \\
\frac{ \partial^{2} G }{ \partial x^{2} }  & = 5x + 20 \\
\frac{ \partial^{2} G }{ \partial y^{2} }  & = 10 \\
\frac{ \partial^{2} G }{ \partial x \partial y }  & = \frac{ \partial^{2} G }{ \partial y \partial x } = 5
\end{align}
$$

**Hesse-Matrix:**

$$
\mathbf{H}_{G} = \begin{bmatrix}
5x + 20 & 5 \\
5 & 10 \\
\end{bmatrix}
$$

**Determinante:**

$$
\det G = 10(5x + 20) - 5^{2} = 50x + 200 - 25 = 50x + 175
$$

**(b)**

$$
\begin{align}
\frac{ \partial G }{ \partial y }  & = 0 \quad \Leftrightarrow \quad 5x + 10y = 0 \quad \Leftrightarrow \quad x = -2y \\
\frac{ \partial G }{ \partial x }  & = 0 \quad \Leftrightarrow \quad \frac{15}{6} \cdot 4y^{2} -40y + 5y = 0 \quad \Leftrightarrow \quad 10y^{2} - 35y = 0 
\end{align}
$$

Somit gilt:

$$
\begin{align}
y_{1,2}  & = y(10y - 35) = 0 \\
y_{1} & = 0 \\
y_{2} & = 10y - 35 = 0 \quad \Leftrightarrow \quad y_{2} = 3,5
\end{align}
$$

Durch einsetzen ergibt sich für $x_{1,2}$:

$$
\begin{align}
x_{1}  & = 5x + 10 \cdot 0 = 0 \\
x_{2}  & = 5x + 35 = 0 \quad \Leftrightarrow \quad x_{2} = -7
\end{align}
$$

Somit existieren die Stationären Punkte $S_{1} = (0; 0)$, $S_{2} = (0; 3,5)$, $S_{3} = (-7; 0)$ und $S_{4} = (-7; 3,5)$.

**Entscheidung für jeden stationären Punkt:**

$$
\begin{align}
 & \det (0;0) = 50 \cdot 0 + 175 = 175 > 0 \implies \text{ Lokales Minimum } \\
 & \det (0; 3,5) = 50 \cdot 0 + 175 = 175 > 0 \implies \text{ Lokales Minimum } \\
 & \det (-7; 0) = 50 \cdot (-7) + 175 = -350 + 175 = -175 < 0 \implies \text{ Sattelpunkt } \\
 & \det (-7; 3,5) = 50 \cdot (-7) + 175 = -350 + 175 = -175 < 0 \implies \text{ Sattelpunkt }
\end{align}
$$

***
