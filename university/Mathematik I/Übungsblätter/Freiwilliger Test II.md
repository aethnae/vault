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

Da aus **(c)** ersichtlich wird, dass es sich bei dieser Extremstelle um ein Minimum handelt, werden weitere Informationen über die Funktionswerte links, bzw. rechts von $x = 7$ gegeben:

$$

$$