---
tags:
week:
flashcard: false
publish: true
---
***
#### Inhalte
Diese Liste enthält alle Eigenschaften, die man bei einer Funktion überprüfen kann:
- Definitionsbereich (mit Definitionslücken)

***
#### Definitionsbereich

> [!note] Vorgehensweise 
> Betrachtung aller Summanden des Funktionsterms: Gibt es Brüche, Logarithmen oder Wurzeln, die in $\mathbb{R}$ für bestimmte Werte nicht definiert sind?
> 
> Der Definitionsbereich der Funktion $f(x)$ wird bspw. mit
> 
> $$
> D_{f} = \mathbb{R}^{+}\backslash\{ 1 \}
> $$
> 
> beschrieben.
##### Beispiel
Bestimmung des Definitionsbereichs der Funktion

$$
f(x) = \frac{1}{x-1} \cdot \ln(x)
$$

Der Funktionsterm besteht aus zwei Summanden: einem **Bruch** und einem **Logarithmus**. Der Bruch ist nicht definiert für $x=1$ (denn dann ist $x-1=0$ im Nenner). Also muss man 1 aus der Definitionsmenge nehmen. Der Logarithmus ist nur definiert, wenn $x$ positiv ist. Man muss also auch noch alle negativen Zahlen und die Null aus Definitionsmenge nehmen.

Übrig bleiben alle positiven Zahlen ohne die 1.
In verschiedenen Mengenschreibweisen:

$$
\begin{aligned}
& D_f=\mathbb{R}^{+} \backslash\{1\} \\
& \left.D_f=\right] 0 ; 1[\cup] 1 ; \infty[
\end{aligned}
$$

***
#### Definitionslücken

> [!abstract] Erklärung 
> (Stetig) hebbare oder behebbare Definitionslücken können bei **gebrochen-rationalen Funktionen** vorkommen.
> 
> Es gibt eine hebbare Definitionslücke bei $x_0$, falls $x_0$ Nullstelle des Zählers und des Nenners ist und die Vielfachheit im Zähler größer ist als die im Nenner oder die Vielfachheiten gleich groß sind (die Nullstelle sich also aus dem Nenner kürzen lässt).
> 
> An dieser Stelle ist die Funktion nicht definiert, kann aber (stetig) fortgesetzt werden, deswegen bezeichnet man die Definitionslücke als **hebbar**.

> [!note] Schließen der Lücke 
> Man kann eine Funktion $\hat{f}$ aus $f$ konstruieren, mit der man die **Definitionslücke** $x_0$ **schließt**:
> Man kürzt die Nullstelle aus dem Bruch, sodass sie im Nenner nicht mehr vorkommt. Dann definiert man $\hat{f}\left(x_0\right)$ als den Wert, den man erhält, wenn man $x_0$ in den gekürzten Bruch einsetzt.
> 
> Man erhält $\hat{f}(x)=\left\{\begin{array}{l}\hat{f}\left(x_0\right)&, \text { wenn } x=x_0 \\ f(x)&, \text { wenn } x \neq x_{0} \end{array}\right.$ , die Fortsetzung von $\mathrm{f}$
> 
> $\hat{f}$ ist **stetig**.
##### Beispiel
Die Funktion

$$
f(x)=\frac{3-x}{2 x^2-6 x}
$$

hat den Definitionsbereich $D_f=\mathbb{R} \backslash\{0 ; 3\}$. Setzt man 3 in die Funktion ein, ergibt sich

$$
f(3)=\frac{3-3}{2 \cdot 9-6 \cdot 3}=\frac{3-3}{18-18}=\frac{0}{0}
$$
.
Wenn man faktorisiert, sieht man, dass die Nullstelle $x_0=3$ aus dem Nenner gekürzt werden kann:

$$
\frac{3-x}{2 x^2-6 x}=\frac{3-x}{-2 x(3-x)}
$$

Es handelt sich bei 3 also um eine **hebbare Definitionslücke**.

$3-x$ wird aus dem Nenner gekürzt:

$$
\frac{3-\mathbf{x}}{-2 x \cdot(3-\mathbf{x})}=\frac{1}{-2 x}
$$

Man setzt 3 in den gekürzten Bruch ein:

$$
\begin{aligned}
& \frac{1}{-2 \cdot 3}=-\frac{1}{6} \\
& \Rightarrow \hat{f}(x)=\left\{\begin{array}{cc}
-\frac{1}{6} & \text { für } x=3 \\
f(x) & \text { für } x \neq 3
\end{array}\right.
\end{aligned}
$$

***
#### [[Grenzwerte]]

***
#### Nullstellen

> [!note] Herangehensweise 
> Selbsterklärend, für Polynome höheren Grades Polynomdivision und dann lösen mit p-q-Formel.

***
#### Monotonie

> [!abstract] Definition 
> Beschreibt das Steigungsverhalten in einem Intervall der Funktion.

> [!note] Herangehensweise
> 1. Intervallgrenzen durch Extremwerte der Funktion bestimmen $\implies f'(x) = 0$
> 2. Nullstellen der Ableitung in die zweite Ableitung einsetzen $\implies f''(x) = 0$
> 	- Für $f''(x) > 0$ ist ein Hochpunkt an der Stelle $x$ gegeben, für $f''(x) < 0$ ein Tiefpunkt
> 	- Wenn $f''(x) = 0$, muss die 3. Ableitung gebildet werden. Ist diese auch Null, liegt ein **Terassenpunkt** vor.
> 
> Wenn man weiß, ob ein Hoch-, Tief- oder Terrassenpunkt vorliegt, kennt man auch die Monotonie des Graphen vor bzw. nach diesen Stellen:
> - Tiefpunkt: links davon fallend, rechts davon steigend
> - Hochpunkt: links davon steigend, rechts davon fallend
> - Terrassenpunkt: links und rechts davon gleiche Monotonie

***
#### Extremwerte
*siehe [[Kurvendiskussion - Übersicht#Monotonie|Monotonie]]*

***
#### Krümmungsverhalten & Wendepunkte

> [!abstract] Definition 
> Das Krümmungsverhalten eines Funktionsgraphen an einer Stelle $x$ ist die Richtungsänderung in diesem Punkt. Man unterscheidet **rechtsgekrümmte** und **linksgekrümmte** Abschnitte sowie **Wendepunkte**.

> [!note] Herangehensweise 
> Dazu betrachtet man für $x$ aus einem bestimmten Abschnitt die zweite Ableitung:
> - $f^{\prime \prime}(x)>0 \Rightarrow f$ linksgekrümmt
> - $f^{\prime \prime}(x)<0 \Rightarrow f$ rechtsgekrümmt
> 
> Als Abschnittsgrenzen bieten sich die **Wendepunkte** an, diese berechnet man mit:
> - $f''(x) = 0$
> - $f'''(x) \neq 0$

- Ein Wendepunkt mit einer Steigung $0$ wird als **Terassen-** oder **Sattelpunkt** bezeichnet

***
#### Bild- und Zielmenge
In der Wertemenge befinden sich nur die Werte, die wirklich von der Funktion angenommen werden.

Die Zielmenge ist eine Menge, in der die Wertemenge enthalten ist, in der es aber auch noch weitere Elemente gibt. So ist z. B. eine Zielmenge der Funktion $f(x)=x^2$ die Menge der reellen Zahlen $\mathbb{R}$. Die eigentliche Wertemenge ist aber $\mathbb{R}_0^{+}$(alle positiven reellen Zahlen und die Null), da keine negativen Zahlen von der Funktion angenommen werden. Ein anderes Wort für Zielmenge ist Wertevorrat.