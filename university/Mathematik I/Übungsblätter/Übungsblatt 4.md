---
tags:
  - übung
week: 2023-12-05
flashcard: false
publish: true
---
***
### Übungsaufgaben

#### Aufgabe 4.1
Bestimmen sie die Ableitungen der nachstehenden Funktionen.

**(a)** $f(x)=x^{\frac{2}{3}}+3 x-x^{\frac{3}{2}}+12$
**(b)** ${} f(x)=\ln \left(\frac{x-3}{x}\right) = \ln\left( 1 - \frac{3}{x} \right) {}$
**(c)** $f(x)=2^x+\frac{\ln (x)}{2}-\frac{1}{x}$
**(d)** $f(x)=\frac{x}{1+x^2}$
**(e)** $f(x)=\sin ^2 x \cdot \cos ^2 x = \sin(x)^{2} \cdot \cos(x)^{2}$

**(a)**
$$
\begin{align}
f'(x) &  = \frac{2}{3}x^{-1/3} + 3 - \frac{3}{2}x^{1/2} \\
\Leftrightarrow \quad & = \frac{2}{3}x^{-1/3} - \frac{3}{2}x^{1/2} + 3
\end{align}
$$

**(b)**
$$
\begin{align}
f'(x) & = \frac{3}{x^{2}} \cdot \frac{1}{1 - \frac{3}{x}} \\
\Leftrightarrow \quad  & = \frac{3}{x^{2} - \frac{3x^{2}}{x}} \\
\Leftrightarrow \quad  & = \frac{3}{\frac{x^{3} - 3x^{2}}{x}} \\ \\
\Leftrightarrow \quad  & = \frac{3}{x^{2} - 3x} \\
\Leftrightarrow \quad  & = \frac{3}{x(x - 3)}
\end{align}
$$

**(c)**
$$
\begin{align}
f'(x) & = \ln(2) \cdot 2^{x} + \frac{1}{2x} + x^{-2}
\end{align}
$$

**(d)**
$$
\begin{align}
f'(x) & = \frac{(1 + x^{2}) - 2x^{2}}{(1+x^{2})^{2}} \\
\Leftrightarrow \quad  & = \frac{1 - x^{2}}{(1 + x^{2})^{2}}
\end{align}
$$

**(f)**
$$
\begin{align}
f'(x) & = 2\sin(x) \cdot \cos(x) \cdot \cos(x)^{2} + \sin(x)^{2} \cdot 2\cos(x) \cdot (-\sin(x)) \\
\Leftrightarrow \quad & = 2 \sin(x) \cos(x) \cdot (\cos(x)^{2} - \sin(x)^{2})
\end{align}
$$

***
#### Aufgabe 4.2

**(a)**
*Zeigen Sie, dass die Funktion*

$$
f(x)=x^5+2 x+1
$$

*im Intervall $[-1,1]$ eine Nullstelle besitzt.*

**(b)**
*Die Funktion*

$$
f(x)=\frac{1}{1+e^{x^2-x}}-\frac{1}{3}
$$

*hat im Intervall $[-2,2]$ zwei Nullstellen $x_1$ und $x_2$.
Finden Sie ein $c \in[-2,2]$, sodass die Nullstelle $x_1$ im Intervall $[-2, c]$ und die Nullstelle $x_2$ im Intervall $[c, 2]$ liegt.*

***

**(a)**
Unter Anwendung des [[Zwischenwertsatz|Zwischenwertsatzes]] existiert eine Nullstelle, falls $f$ auf $[a, b]$ stetig ist mit $f(a) > 0 \text{ und } f(b) < 0$ oder andersherum.

Da Polynomfunktionen wie $f(x)$ allgemein als stetig gelten, ist der Nachweis dafür bereits erbracht.

$$
f(-1) = -1^{5} + (-2) + 1 = - 1 - 2 + 1 = -2
$$

und

$$
f(1) = 1^{5} + 2 + 1 = 4
$$

daher existiert eine Nullstelle von $f(x) \text{ im Intervall } [-1, 1]$.

***

**(b)**
Da $f(x)$ als Grundfunktion für alle $x \in [-1, 1]$ stetig ist, gilt

$$
\begin{align}
f(-2) & = \frac{1}{1 + e^{ 6 }} - \frac{1}{3} < 0 \\
f(2) & = \frac{1}{1 + e^{ 2 }} - \frac{1}{3} < 0 \\
\end{align}
$$

da $e^{ 6 } > e^{ 2 } > 2$ und damit der erste Bruch in beiden Termenkleiner ist als ${} \frac{1}{3}$.
Halbiert man das Intervall nun bei $c = 0$

$$
f(c) = f(0) = \frac{1}{1 + e^{ 0 }} - \frac{1}{3} = \frac{1}{2} - \frac{1}{3} = \frac{1}{6} > 0
$$

Da $f(-2) < 0$ und $f(0) > 0$, gibt es nach dem [[Zwischenwertsatz]] ein $x_{1} \in \mathbb{R} \text{ mit } -2 < x_{1} < 0$, für das $f(x_{1}) = 0$ gilt.

Da $f(2) < 0 \text{ und } f(0) > 0$, gibt es nach dem [[Zwischenwertsatz]] ein $x_{2} \in \mathbb{R}$ mit $0 < x_{2} < 2$, für das $f(x_{2}) = 0$ gilt.

***
#### Aufgabe 4.3
*Untersuchen Sie die folgenden Funktionen auf Stetigkeit und Differenzierbarkeit und skizzieren Sie den Verlauf der Funktionen. Geben Sie dort, wo die Funktionen nicht differenzierbar sind, die rechts- und linksseitigen Ableitungen an, sofern diese existieren.*

**(a)**
$$
f(x)=\left\{\begin{array}{llr}
6 x+4 & \text { falls }  & x \leq -1 \\
2 x^3 & \text { falls } & -1 < x \leq 1 \\
-x^2+2 x+1 & \text { falls }  & x > 1
\end{array}\right.
$$

**(b)**
$$
g(x)= \begin{cases}x^2-2 x+1 & \text { falls } x<3 \\ 4 x-10 & \text { falls } x \geq 3\end{cases}
$$

***

**(a)**
$$
\begin{align}
 & \lim_{ x \uparrow -1 } (6x + 4) = -6 + 4 = -2 \\
 & \lim_{ x \downarrow -1 } (2x^{3}) = -1 \cdot 2 = -2 \\
 & f(-1) = 6 \cdot (-1) + 4 = -6 + 4 = -2
\end{align}
$$

und

$$
\begin{align}
 & \lim_{ x \uparrow 1 } (2x^{3}) = 2 \\
 & \lim_{ x \downarrow 1 } (-x^{2} + 2x + 1) = -1 + 2 + 1 = 2 \\
 & f(1) = 2 \cdot 1^{3} = 2
\end{align}
$$

daher ist die Funktion stetig, und $\displaystyle \lim_{ x \to -1 } \text{und } \lim_{ x \to 1 }$ existieren.

Um auf Differenzierbarkeit zu prüfen, berechnen wir zunächst die Ableitungen als

$$
f'(x)=\left\{\begin{array}{llr}
6 & \text { falls }  & x < -1 \\
6x^{2} & \text { falls } & -1 < x < 1 \\
-2x +2 & \text { falls }  & x > 1
\end{array}\right.
$$

$$
\begin{align}
f'_{-}(-1) & = 6 = 6 \cdot (-1)^{2} = f'_{+}(-1) \\
f'_{-}(1)  & = 6 \neq 0 = -2 \cdot 1 + 2 = f'_{+}(1)
\end{align}
$$

Daher ist $f(x)$ an der Stelle $x = -1$ differenzierbar mit $f'(-1) = 6$, aber bei $x = 1$ nicht differenzierbar, da die oben berechneten einseitigen Ableitungen nicht identisch sind.
Die gesamte Ableitung lautet also (für $x \neq 1$)

$$
f'(x)=\left\{\begin{array}{llr}
6 & \text { falls }  & x \leq -1 \\
6x^{2} & \text { falls } & -1 < x < 1 \\
-2x +2 & \text { falls }  & x > 1
\end{array}\right.
$$

**(b)**
$$
\begin{align}
 & \lim_{ x \uparrow 3 } (x^{2}-2x+1) = 3^{2}-6+1=4 \\
 & \lim_{ x \downarrow 3 } (4x-10) = 12-10 = 2 \\
 & g(3) = 4 \cdot 3 - 10 = 2
\end{align}
$$

Die Funktion $g(x)$ ist also nicht linksseitig stetig.

Um auf Differenzierbarkeit zu prüfen, berechnen wir zunächst die Ableitungen

$$
g'(x)= \begin{cases}2x-2 & \text { falls } x<3 \\
4 & \text { falls } x > 3\end{cases}
$$

Da $g(x)$ nicht linksseitig stetig ist, existiert keine linksseitige Ableitung $g'_{-}(3)$. Daher ist $g$ auch nicht differenzierbar bei $x = 3$.

***
#### Aufgabe 4.4
*Wir betrachten die Funktion $f(x)=(1+x)^m$ für ein $m>0$.*

**(a)**
*Berechnen Sie das Differential $\mathrm{d} f$ der Funktion $f$ an der Stelle $x_0=0$.*

**(b)**
*Nutzen Sie das Differential aus (a), um die Näherung*

$$
(1+x)^m \approx 1+m x \quad \text { für } x \text { nahe bei } 0
$$

*zu zeigen.*

**(c)**
*Angenommen, ein Anfangskapital von $K_0=1000 €$ wird für $20 \mathrm{Jahre}$ zu $2 \%$ verzinst. Nutzen Sie die Formel aus (b), um das Endkapital $K_{20}$ zu approximieren.*

***

**(a)**
$$
\mathrm{d}f = f'(x_{0})\mathrm{d}x
$$

also

$$
\mathrm{d}f = m\mathrm{d}x
$$

**(b)**
