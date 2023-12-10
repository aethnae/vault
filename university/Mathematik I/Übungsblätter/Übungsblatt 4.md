---
tags:
  - übung
  - ableitungen
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
*Angenommen, ein Anfangskapital von $K_{0} = \texteuro 1000$ wird für 20 Jahre zu $2 \%$ verzinst. Nutzen Sie die Formel aus (b), um das Endkapital $K_{20}$ zu approximieren.*

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
Wir wissen, dass $\Delta f \approx \mathrm{d} f$, wenn $\Delta x=\mathrm{d} x$ klein ist. Konkrekt gilt hier für $x_0=0$ und kleines $\mathrm{d} x=\Delta x-$ $\left(x-x_0\right)=(x-0)=x$, dass

$$
\Delta f=f(0+x)-f(0) \approx \mathrm{d} f=m \cdot \mathrm{d} x=m \cdot x .
$$

Mit $f(0)=(1+0)^m=1$ erhalten wir also

$$
f(x)-1 \approx m \cdot x \quad \Leftrightarrow \quad f(x) \approx 1+m \cdot x .
$$

**(c)**
Das Endkapital berechnet sich als

$$
K_{20}=K_0 \cdot\left(1+\frac{p}{100}\right)^{20}=1000 \cdot(1+0,02)^{20} .
$$

Auf den Term $(1+0,02)^{20}$ können wir nun die Approximationsformel aus **(b)** mit $x=0,02$ (nahe bei 0 ) und $m=20$ anwenden. Wir erhalten

$$
K_{20}=1000 \cdot(1+0,02)^{20} \approx 1000(1+0,02 \cdot 20)=1000 \cdot 1,4=\underline{\underline{1400}} .
$$

Zum Vergleich: Der exakte Wert lautet $1000 \cdot(1+0,02)^{20} \approx 1485,95$.

***
#### Aufgabe $4.5^{F}$
*Untersuchen Sie die nachstehende Funktion auf Definitionsbereich, Wertebereich, Stetigkeit, Differenzierbarkeit, Nullstellen, Schnittpunkt mit der $y$-Achse, Verhalten im Unendlichen, Extremwerte, Monotonie und skizzieren Sie den Verlauf der Funktion.*

$$
f(x)=|x+1|+|2 x-4|
$$

**Definitions- und Wertemenge:**

$$
\begin{align}
 & D_{f} = \mathbb{R} \\
 & W_{f} = \mathbb{R}_{3}^{+}
\end{align}
$$

**Stetigkeit:**

$$
f(x)=|x+1|+|2 x-4|=\left\{\begin{array}{rlr}
-(x+1)-(2 x-4) & \text { falls } & x \leq -1 \\
(x+1)-(2 x-4) & \text { falls } & -1 < x \leq 2 \\
(x+1)+(2 x-4) & \text { falls } & x > 2
\end{array}\right.
$$

was

$$
\left\{\begin{array}{llr}
-3 x+3 & \text { falls } & x \leq -1 \\
-x+5 & \text { falls } & -1 < x \leq 2 \\
3 x-3 & \text { falls } & x > 2
\end{array}\right.
$$

entspricht. Um auf Stetigkeit zu überprüfen, müssen die links- und rechtsseitigen Grenzswerte in den Definitionsübergängen übereinstimmen:

$$
\begin{align}
 & \lim_{ x \uparrow -1 } (-3x+3) = 3 + 3 = 6 \\
 & \lim_{ x \downarrow -1 } (-x+5) = 1 + 5 = 6 \\
 & f(-1) = -3 \cdot (-1) + 3 = 3 + 3 = 6
\end{align}
$$

die Funktion ist also am ersten Definitionsübergang bei $x = -1$ stetig. Das selbe Verfahren für $x = 2$ liefert:

$$
\begin{align}
 & \lim_{ x \uparrow 2 } (-x+5) = -2 + 5 = 3 \\
 & \lim_{ x \downarrow 2 } (3x - 3) = 3 \cdot 2 - 3 = 3 \\
 & f(2) = -2 + 5 = 3
\end{align}
$$

somit ist die Funktion auch am zweiten Definitonsübergang, und damit in ihrer Gesamtheit stetig.
Dieses Verfahren kann auch übersprungen werden, und die Folgerung, wonach zusammengesetzte Funktionen, die aus elementaren Funktionen, wie hier die Betragsfunktionen, bestehen, immer stetig sind.

**Differenzierbarkeit:**
Für $f(x)$ existieren die Ableitungen

$$
f'(x) = \left\{\begin{array}{lrr}
 -3  & \text{ falls }  & x < -1 \\
 -1  & \text{ falls }  & -1 < x < 2 \\
 3  & \text{ falls }  & x > 2
\end{array}\right.
$$

Am Definitionsübergang $x = -1$ ist $f'_{-}(-1) = -3$ und $f'_{+}(-1) = -1$, somit ist die Funktion an der Stelle $x = -1$ nicht differenzierbar. Auch ist ohne weitere Rechnung ersichtlich, dass die Funktion an der Stelle $x = 2$ nicht differenzierbar ist.

**Nullstellen:**
Aus der Analyse des Wertebereichs wissen wir bereits, dass $W_{f} = \mathbb{R}_{3}^{+}$, somit gibt es keine Nullstelle der Funktion $f$.

**Schnittpunkt mit der $y$-Achse:**
Berechnung für $x = 0$ liefert

$$
f(0) = \mid 0 + 1 \mid + \mid 2 \cdot 0 - 4 \mid = 1 + 4 = 5
$$

Der Schnittpunkt mit der $y$-Achse liegt somit im Punkt $P = (0, 5)$.

**Verhalten im Unendlichen:**
Berechnung des Limes liefert

$$
\begin{align}
\lim_{ x \to \infty } f(x)  & = \lim_{ x \to \infty } (\mid x+1\mid + \mid 2x - 4\mid) \stackrel{x \rightarrow \infty}{\longrightarrow} \infty \\
\lim_{ x \to -\infty } f(x)  & = \lim_{ x \to -\infty } (\mid x + 1 \mid + \mid 2x - 4\mid) \stackrel{x \rightarrow -\infty}{\longrightarrow} \infty
\end{align}
$$

**Monotonie:**
Die Funktion besteht aus zwei fallenden Geraden und einer steigenden Gerade. Auf dem Intervall $(-\infty, 2]$ ist $f$ streng mononton fallend, auf $[2, \infty)$ streng monoton steigend.

**Extremwerte:**
Aus der Monotonie folgt sofort, dass $f$ genau ein lokales und globales Minimum bei $x=2$ (mit dem Funktionswert $f(2)=-2+5=3$ ) hat. Die Funktion hat kein (lokales oder globales) Maximum.

**Stetigkeit:**
Die Funktion ist als Summe von Betragsfunktionen selber auch stetig.

***
#### Aufgabe $4.6^{F}$
*Untersuchen Sie die Funktion*

$$
f(x)= \begin{cases}x \cdot \sin \left(\frac{1}{x}\right) & \text { falls } x<0, \\ 4 x & \text { falls } x \geq 0\end{cases}
$$

*auf Stetigkeit und Differenzierbarkeit an der Stelle $x_0=0$.*

$$
\begin{align}
 & \lim_{ x \uparrow 0 } \left( x \cdot \sin\left( \frac{1}{x} \right) \right) \stackrel{x \rightarrow 0}{\longrightarrow} 0 \\
 & \lim_{ x \downarrow 0 } (4x) \stackrel{x \rightarrow 0}{\longrightarrow} 0 \\
 & f(0) = 4 \cdot 0 = 0
\end{align}
$$

Somit ist $f(x)$ an der Stelle $x = 0$ stetig, und $\displaystyle\lim_{ x \to 0 } f(x) = 0$.
Um $f(x)$ auf Differenzierbarkeit zu überprüfen, müssen die Ableitungen gebildet werden:

$$
f'(x) = \begin{cases} \sin \left(\frac{1}{x}\right) - \frac{1}{x} \cdot \cos\left( \frac{1}{x} \right) & \text { falls } x<0, \\ 4 & \text { falls } x \geq 0\end{cases}
$$

Die rechtsseitige Ableitung ist offensichtlich $f'_{+}(x) = 4$, die linksseitige Ableitung kann jedoch nicht bestimmt werden, da die Sinus- und Kosinusterme unbestimmt divergieren und $\frac{1}{x}$ bestimmt divergiert. Somit ist $f$ nicht differenzierbar bei $x = 0$.

***
### Tutoriumsaufgaben

#### Aufgabe 4.7
*Berechnen Sie die Ableitungen der nachstehenden Funktionen.*

**(a)** $f(x)=x^{\frac{3}{4}}+x^2-7 x+4$
**(b)** $f(x)=\frac{1}{x}-x^3+2 \ln (x)+e$
**(c)** $f(x)=\sqrt{\frac{1}{3} x^3}$
**(d)** ${} f(x)=\sqrt{e^x+x} = (e^{ x } + x)^{1/2} {}$
**(e)** $f(x)=\frac{\ln (x)}{x^4}$
**(f)** $f(x)=e^{(x+2)^2-x}$

**(a)**
$$
f'(x) = \frac{3}{4}x^{-1/4} + 2x - 7
$$

**(b)**
$$
f'(x) = -x^{-2} -3x^{2} + \frac{2}{x}
$$

**(c)**
$$
f'(x) = x^{2} \cdot \frac{1}{2\sqrt{ \frac{1}{3}x^{3} }}
$$

**(d)**
$$
f'(x) = (e^{ x } + 1) \cdot \frac{1}{2}(e^{ x } + x)^{-1/2} = \frac{e^{ x } + 1}{2\sqrt{ e^{ x } + x }}
$$

**(e)**
$$
\frac{1}{x} \cdot x^{-4} + \ln(x) \cdot -4x^{-5} = \frac{1}{x^{5}} + \frac{\ln(x) \cdot -4x^{-5} \cdot x^{5}}{x^{5}} = \frac{1 - 4\ln(x)}{x^{5}}
$$

**(f)**
$$
f'(x) = (2 x+3) e^{(x+2)^2-x}
$$

***
#### Aufgabe 4.8
*Zeigen Sie, dass die Gleichungen*

**(a)**
$\cos (x)=\frac{1}{2} x-1 \quad$ für $x \in[0, \pi]$

**(b)**
$\frac{4 x}{\sqrt{1+x^2}}=x-\cos (\pi x) \quad$ für $x \in[-1,1]$

*jeweils eine Lösung besitzen.*

**(a)**
Das Problem kann umformuliert werden, sodass zu zeigen ist, dass die Funktion

$$
f(x)=\cos (x)-\frac{1}{2} x+1
$$

auf dem Intervall $x \in[0, \pi]$ eine Nullstelle besitzt.
Die Funktion $f(x)=\cos (x)-\frac{1}{2} x+1$ ist als Grundfunktion für alle $x \in[0, \pi]$ stetig. Es gilt:

$$
f(0)=2>0 \text { und } f(\pi)=-\frac{1}{2} \pi<0
$$

Nach dem Zwischenwertsatz gibt es eine Stelle $x_0$, die $f\left(x_0\right)=0$ erfüllt.

**(b)**
Das Problem kann umformuliert werden, sodass zu zeigen ist, dass die Funktion

$$
g(x) = \frac{4x}{\sqrt{ 1 + x^{2} }} - x + \cos(\pi x)
$$

auf dem Intervall $x \in [-1, 1]$ eine Nullstelle besitzt.
Die Funktion $g(x)$ ist als Grundfunktion für alle $x \in [-1, 1]$ stetig. Es gilt

$$
\begin{align}
 & g(-1) = \frac{-4}{\sqrt{ 2 }} + 1 + \cos(-\pi) = \frac{-4}{\sqrt{ 2 }} + 1 - 1 < 0 \\
 & g(1) = \frac{4}{\sqrt{ 2 }} - 1 - 1 \frac{4}{\sqrt{ 2 }} - 2 > 0, \text{ da } \frac{4}{\sqrt{ 2 }} > 2
\end{align}
$$

Somit besitzt die Funktion $g(x)$ auf dem Intervall eine Nullstelle, das Problem ist also gelöst.

***
#### Aufgabe 4.9
*Untersuchen Sie die folgenden Funktionen auf Stetigkeit und Differenzierbarkeit und skizzieren Sie den Verlauf der Funktionen. Geben Sie dort, wo die Funktionen nicht differenzierbar sind, die rechts- und linksseitigen Ableitungen an, sofern diese existieren.*

**(a)**
$$
f(x)=\left\{\begin{array}{llr}
e^{-x}  &  \text { falls } & x<-2 \\
5 x & \text { falls } & -2  \leq x \leq 0 \\
e^x+4 x & \text { falls } & x>0
\end{array}\right.
$$

**(b)**
$$
g(x)=\left\{\begin{array}{llr}
-(x-2)^2+2 & \text { falls } & x<2 \\
 x & \text { falls }  & 2 \leq x \leq 4 \\
\ln (x-3)+4 & \text { falls } & x>4
\end{array}\right.
$$

**(a)**

**Stetigkeit:**

$$
\begin{align}
 & \lim_{ x \uparrow -2 } f(x) = \lim_{ x \uparrow -2 } (e^{ -x }) \stackrel{x \rightarrow -2}{\longrightarrow} e^{ 2 } \\
 & \lim_{ x \downarrow -2 } f(x) = \lim_{ x \downarrow -2 } (5x) \stackrel{x \rightarrow -2}{\longrightarrow} -10 \\
 & \lim_{ x \uparrow 0 } f(x) = \lim_{ x \uparrow 0 } (5x) \stackrel{x \rightarrow 0}{\longrightarrow} 0 \\
 & \lim_{ x \downarrow 0 } f(x) = \lim_{ x \downarrow 0 } (e^{ x } + 4x) \stackrel{x \rightarrow 0}{\longrightarrow} 1 + 4 \cdot 0
\end{align}
$$

Da $f(-2)=-10$ ist, ist $f$ bei $x=-2$ zwar noch rechtsseitig, aber nicht linksseitig stetig. Bei $x=0$ gilt, dass $f(0)=0$ ist. Damit ist $f$ noch linksseitig, aber nicht rechtsseitig stetig.

**Differenzierbarkeit:**

$$
f^{\prime}(x)=\left\{\begin{array}{llr}
-e^{-x} & \text { falls } & x<-2 \\
5 & \text { falls } & -2<x<0 \\
e^x+4 & \text { falls } & x>0
\end{array}\right.
$$

Die rechtsseitige Ableitung ist $f_{+}^{\prime}(-2)=5$. Die linksseitige Ableitung $f_{-}^{\prime}(-2)$ existiert nicht, da $f$ bei -2 nicht (links-)stetig ist. Damit existiert $f^{\prime}(-2)$ auch nicht nicht. Die linksseitige Ableitung bei $x=0$ ist $f_{-}^{\prime}(0)=5$. Die rechtsseitige Ableitung $f_{+}^{\prime}(0)$ existiert nicht (wegen der fehlenden Rechtsstetigkeit bei 0 ) und damit existiert auch $f^{\prime}(0)$ nicht.

**(b)**

**Stetigkeit:**
Für $x \neq 2,4$ ist $f$ als Polynom/Logarithmusfunktion stetig. Für $x=2$ berechnen wir

$$
g(2)=2, \quad \lim _{x \uparrow 2} g(x)=\lim _{x \uparrow 2}-(x-2)^2+2=-0^2+2=2, \quad \lim _{x \downarrow 2} g(x)=\lim _{x \downarrow 2} x=2 .
$$

Da alle drei Werte übereinstimmen, ist $g$ auch bei $x=2$ stetig. Für $x=4$ berechnen wir

$$
g(4)=2, \quad \lim _{x \uparrow 4} g(x)=\lim _{x \uparrow 4} x=4, \quad \lim _{x \downarrow 4} g(x)=\lim _{x \downarrow 4} \ln (x-3)+4=\ln (1)+4=4 .
$$

Da alle drei Werte übereinstimmen, ist $g$ auch bei $x=4$ stetig.

**Differenzierbarkeit:**
Die Funktion $g(x)$ hat für $x \neq 2 \text{ und } x \neq 4$ die Ableitung:

$$
g^{\prime}(x)=\left\{\begin{array}{llr}
-2(x-2) & \text { falls } & x<2 \\
1 & \text { falls }  & 2<x<4 \\
\frac{1}{x-3} & \text { falls } & x>4
\end{array}\right.
$$

Überprüfung der Ableitungen an den Definitionsübergängen:

$$
\begin{align}
 & g'_{-}(2) = 0 \\
 & g'_{+}(2) = 1 \\
 & g'_{-}(4) = 1 \\
 & g'_{+}(4) = 1
\end{align}
$$

Somit ist $g(x)$ an der Stelle $x = 2$ nicht differenzierbar, und an der Stelle $x = 4$ differenzierbar mit $g'(4) = 1$.

***
#### Aufgabe 4.10
*Eine Kostenfunktion in Abhängigkeit von der Produktionsmenge $x$ (in Mengeneinheiten, ME) habe die Gestalt $K(x)=100+\sqrt{x}$ (in €). Von $x_0=10.000$ soll die Produktion um zwei ME erhöht werden.*

**(a)**
*Bestimmen Sie mit Hilfe des Differentials die ungefähre Kostensteigerung für diese zusätzliche Produktion.*

**(b)**
*Vergleichen Sie den angenäherten Wert mit dem exakten Kostenzuwachs.*

**(a)**
$$
K(10.000) = 100 + \sqrt{ 10.000 } = 200 \texteuro
$$

Die Produktionssteigerung von $x_{0} = 10.000$ auf $x_{1} = 10.002$ kann durch $\Delta x$ beschrieben werden. Um die Kostensteigerung zu berechnen, ist $\mathrm{d}K$ gesucht. Einsetzen in die Formel für das Differential ergibt

$$
\mathrm{d}K = K'(x_{1}) \cdot \Delta x = \frac{1}{2\sqrt{ 10.002 }} \cdot 2 = \frac{2}{2\sqrt{ 10.002 }} = \frac{1}{\sqrt{ 10.002 }} \approx 0,01 \texteuro
$$

die Kostensteigerung bei einer Produktionssteigerung um 2 Mengeneinheiten beträgt somit ca. 1 Cent.

**(b)**
Der exakte Kostenzuwachs berechnet sich durch

$$
\Delta K=K(10002)-K(10000)=100+\sqrt{10002}-(100+\sqrt{10000})=0,0099995 \texteuro
$$

***
### Selbstrechenaufgaben

#### Aufgabe 4.11
*Berechnen Sie die Ableitungen der nachstehenden Funktionen.*

**(a)** $f(x)=e^{\sqrt{x}}$
**(b)** $f(x)=\frac{x^2}{\sin (x)+x}$
**(c)** $f(x)=e^{-\frac{x^2}{2}}$
**(d)** $f(x)=e^{-\frac{x^2}{2}} \cdot \sin (x)$
**(e)** $f(x)=\frac{\sin (x)}{\cos (x)}$
**(f)** $f(x)=\ln \left(\frac{3 x-4}{2}\right)$
**(g)** $f(x)=x^2 \cdot 7^x$

**(a)**
$$
f'(x) = e^{ \sqrt{ x } } \cdot \frac{1}{2\sqrt{ x }}
$$

**(b)**
$$
f'(x) = 2x \cdot \frac{1}{\sin(x) + x} + x^{2} \cdot -(\sin(x) + x)^{-2} \cdot (\cos(x) + 1)
$$

oder mit Quotientenregel

$$
f'(x) = \frac{2x \cdot (\sin(x) + x) - x^{2} \cdot (\cos(x) + 1)}{(\sin(x) + x)^{2}} = \frac{2 x \sin (x)+x^2-x^2 \cos (x)}{(\sin (x)+x)^2}
$$

**(c)**
$$
f^{\prime}(x)=e^{-\frac{x^2}{2}} \cdot(-x)=-x e^{-\frac{x^2}{2}}
$$

**(d)**
$$
f^{\prime}(x)=-x e^{\frac{-x^2}{2}} \sin (x)+e^{\frac{-x^2}{2}} \cos (x)
$$

**(e)**
$$
f^{\prime}(x)=\overbrace{\frac{\cos (x)^2+\sin (x)^2}{\cos (x)^2}}^{=1}=\frac{1}{\cos (x)^2}
$$

**(f)**
$$
f'(x) = \frac{3}{3x - 4}
$$

***
#### Aufgabe 4.12
*Untersuchen Sie die folgende Funktion auf Stetigkeit und Differenzierbarkeit und skizzieren Sie den Verlauf der Funktion. Geben Sie dort, wo die Funktion nicht differenzierbar ist, die rechts- und linksseitigen Ableitungen an, sofern diese existieren.*

$$
f(x)=\left\{\begin{array}{llc}
-2 x-1 & \text { falls } & x \leq-2 \\
x^2+2 x & \text { falls } -2 < &  x < 0 \\
\sqrt{x} & \text { falls } & x \geq 0
\end{array}\right.
$$

**Stetigkeit:**
Für $x=-2$ berechnen wir

$$
\lim _{x \uparrow-2} f(x)=\lim _{x \uparrow-2}-2 x-1=3 \neq 0=(-2)^2+2 \cdot(-2)=\lim _{x \downarrow-2} x^2+2 x=\lim _{x \downarrow-2} f(x) .
$$

Damit ist $f$ bei $x=-2$ nicht stetig.
Für $x=0$ berechnen wir

$$
\lim _{x \uparrow 0} f(x)=\lim _{x \uparrow 0} x^2+2 x=0^2+2 \cdot 0=0=\lim _{x \downarrow 0} \sqrt{x}=\lim _{x \downarrow 0} f(x)
$$

sowie $f(0)=\sqrt{0}=0$. Damit ist $f$ stetig bei $x=0$.

**Differenzierbarkeit:**
Für $x \neq-2$ und $x \neq 0$ berechnen wir die Ableitung mit den bekannten Regeln als

$$
f^{\prime}(x)=\left\{\begin{array}{llr}
-2 & \text { falls } & x < -2, \\
2 x+2 & \text { falls } & -2 < x < 0, \\
\frac{1}{2 \sqrt{x}} & \text { falls } & x > 0 .
\end{array}\right.
$$

Da die Funktion bei $x=-2$ nicht (rechtsseitig) stetig ist, existiert die rechtsseitige Ableitung $f_{+}^{\prime}(-2)$ nicht. Die linksseitige Ableitung ist $f_{-}^{\prime}(-2)=-2$.
Bei $x=0$ ist $f$ stetig und es gilt

$$
f_{-}^{\prime}(x)=2 \cdot 0+2=2 \text { sowie } f_{+}^{\prime}(x)=\lim _{x \downarrow 0} f^{\prime}(x)=\lim _{x \downarrow 0} \frac{1}{2 \sqrt{x}}=\infty .
$$

Da die rechtsseitige Ableitung hier ebenfalls nicht existiert, ist die Funktion auch nicht differenzierbar bei $x=0$.

***
#### Aufgabe 4.13
*Es sei $y=f(x)=\sqrt{19+x^4}$*

**(a)**
*Berechnen Sie das Differential von $f$.*

**(b)**
*Bestimmen Sie approximativ mit Hilfe das Differentials die Änderung der Funktion, wenn ausgehend von $x=3$ das Argument $x$ um 0,05 verändert wird. Vergleichen Sie diesen Wert mit der exakten Veränderung.*

**(a)**
$$
\mathrm{d}f = \frac{2 x^3}{\sqrt{19+x^4}} \cdot \mathrm{d} x, \text{ da }f^{\prime}(x)=\frac{1}{2}\left(19+x^4\right)^{-\frac{1}{2}} \cdot 4 x^3=\frac{2 x^3}{\sqrt{19+x^4}} \text{ und } \mathrm{d}f = f'(x_{0}) \cdot \mathrm{d}x
$$

**(b)**
$$
\mathrm{d}x = 0,05
$$

somit ist ${} \mathrm{d}f$ 

$$
\mathrm{d}f = f^{\prime}(3) \cdot 0,05=\frac{2 \cdot 3^3}{\sqrt{19+3^4}} \cdot \frac{1}{20}=\frac{27}{100}=0,27
$$

für die exakte Veränderung berechnen wir

$$
\Delta y=f(3,05)-f(3)=\sqrt{19+(3,05)^4}-\sqrt{19+3^4} \approx 0,2731
$$
