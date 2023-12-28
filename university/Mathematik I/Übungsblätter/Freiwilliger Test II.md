---
tags:
  - übung
  - differenzierbarkeit
  - stetigkeit
week: 2023-12-27
publish: true
---
***
##### 1. Aufgabe
*Untersuchen Sie die Funktion*

$$
f(x)= \begin{cases}x^2-3 x+5 & \text { falls } x<1 \\ -2 x+5 & \text { falls } x \geq 1\end{cases}
$$

*auf Stetigkeit und Differenzierbarkeit.*

**Stetigkeit:**

$$
\begin{align}
 & \lim_{ x \uparrow 1 } f(x) = \lim_{ x \uparrow 1 } (x^{2}-3x+5) \stackrel{x \uparrow 1}{\longrightarrow} 3 \\
 & \lim_{ x \downarrow 1 } f(x) = \lim_{ x \downarrow 1 } (-2x+5) \stackrel{x \downarrow 1}{\longrightarrow} 3 \\
 & f(1) = -2 \cdot 1 + 5 = 3 \\
\end{align}
$$

Somit ist die Funktion $f(x)$ auf ihrem gesamten Definitionsbereich stetig.

**Differenzierbarkeit:**

Für die 1. Ableitung von $f(x)$ gilt:

$$
f'(x)= \begin{cases} 2x-3 & \text { falls } x<1 \\ -2 & \text { falls } x > 1\end{cases}
$$

Also

$$
\begin{align}
 & f_{-}'(1) = 2 \cdot 1 - 3 = -1 \\
 & f_{+}'(x) = -2 \\
\end{align}
$$

Somit ist $f(x)$ an der Stelle $x = 1$ nicht differenzierbar, da die links- und rechtsseitigen Ableitungen nicht identisch sind, und $f'(x)$ somit nicht existiert.

***
##### 2. Aufgabe
*Gegeben eine differenzierbare Funktion $f$, sei $y=f(x)$. Welche mathematischen Bedingungen können den folgenden Texten entnommen werden?*

**(a)** $x=-2$ ist eine Nullstelle der Funktion.
**(b)** Der Graph der Funktion schneidet die $y$-Achse bei $y=-3$.
**(c)** Die Funktion hat im Punkt $(7,-1)$ ein Minimum.
**(d)** An der Stelle $x=0$ hat $f(x)$ den Funktionswert 3 und die Steigung 1.
**(e)** Die Funktion besitzt im Punkt $(1,-1)$ eine waagrechte Tangente.

**(a)**
Da $x=-2$ eine Nullstelle von $f(x)$ ist, muss

$$
f(-2) = 0
$$

gelten.

**(b)**
Da der Graph von $f(x)$ die $y$-Achse bei $y=-3$ schneidet, gilt

$$
f(0) = -3
$$


**(c)**
Da die Funktion im Punkt $(7, -1)$ ein Minimum hat, gilt offensichtlich

$$
f(7) = -1
$$

Desweiteren gilt für Extremstellen, dass deren Steigung 0 beträgt, somit gilt auch

$$
f'(7) = 0
$$


**(d)**
Da $f(x)$ an der der Stelle $x=0$ den Funktionswert 3 und die Steigung 1 hat, gilt

$$
\begin{align}
 & f(0) = 3 \\
 & f'(0) = 1 \\
\end{align}
$$

**(e)**
Da die Funktion im Punkt $(1,-1)$ eine waagerechte Tangente besitzt, gilt

$$
\begin{align}
 & f(1) = -1 \\
 & f'(1) = 0 \\
\end{align}
$$

***
##### 3. Aufgabe
*Bestimmen Sie die Funktionsgleichung einer kubischen Funktion $y=f(x)$, die in $(0,0)$ ein lokales Maximum und in $(1,-1)$ einen Wendepunkt hat.*

*Fertigen Sie anschließend eine Skizze der kubischen Funktion $f(x)$ an.*

Da $(0,0)$ ein Punkt auf dem Graphen der Funktion ist, muss

$$
f(0) = a \cdot 0^{3} + b \cdot 0^{2} + c \cdot 0 + d = d
$$

gelten. Somit ist $d = 0$, da $f(0) = 0$.

Da die Steigung einer Extremstelle 0 betragen muss, gilt an der Stelle $x = 0$ auch $f'(x) = 0$. Somit

$$
f'(0) = 3 \cdot a \cdot 0^{2} + 2 \cdot b \cdot 0 + c = c
$$

Somit ist auch $c = 0$. Setzt man $c \text{ und } d$ in $f(x)$ ein, gilt $f(x) = ax^{3}+bx^{2}$.

Da desweiteren gegeben ist, dass ein Wendepunkt in $(1,-1)$ vorliegt, muss eine Extremstelle von $f'(x)$ bei $x = 1$ vorliegen, die zweite Ableitung ($f''(x) = 6ax + 2b$) muss also 0 sein. Außerdem muss $f(1)=-1$ gelten.

Also

$$
\begin{align}
 f(1) & = a + b = -1 \\
 f''(1) & = 6a + 2b = 0
\end{align}
$$

Durch Umstellen der zweiten Gleichung nach $b$ ($b = -3a$) und Einsetzen in die erste Gleichung ergibt sich

$$
f(1) = a -3a = -2a = -1 \quad \Leftrightarrow \quad a = \frac{1}{2}
$$

Erneutes Einsetzen ergibt für $b$

$$
f(1) = \frac{1}{2} + b = -1 \quad \Leftrightarrow \quad b = -\frac{3}{2}
$$

Somit gilt abschließend als Funktionsgleichung $f(x) = \frac{1}{2}x^{3} -\frac{3}{2}x^{2}$.

Anbei eine Skizze des Graphen von $f(x)$:

![[Pasted image 20231227233221.png|center|450]]