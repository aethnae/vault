***

Unter einer Verkettung von Funktionen $u(x)$ und $v(x)$ versteht man die Hintereinanderausführung dieser Funktionen $u(v(x))$. Dabei nennt man $v(x)$ die *innere*, $u(x)$ die *äußere Funktion*.

**Erläuterung:**
Zuerst wird der Funktionswert der inneren Funktion $v$ an der Stelle $x$ gebildet. Anschließend wird der Funktionswert der äußeren Funktion $u$ an der Stelle $v(x)$ gebildet. Es gibt auch die Schreibweise mit $u°v(x)$ ("$u$ nach $v$ von $x$").

**Ableitung:**
Gegeben seien zwei differenzierbare Funktionen $u$ und $v$ sowie deren Verkettung $f$ mit $f(x) = u(v(x))$.
Dann ist auch $f$ differenzierbar und es gilt:

$$
f'(x) = u'(v(x)) \cdot v'(x)
$$
