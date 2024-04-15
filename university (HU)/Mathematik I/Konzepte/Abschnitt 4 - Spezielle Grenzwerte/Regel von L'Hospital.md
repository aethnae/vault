---
tags:
  - grenzwerte
week: 2023-12-05
flashcard: false
publish: true
---
***

> [!def] Regel von L'Hospital 
> Es seien $g, h$ jeweils $n$-mal differenzierbare Funktionen und es gelte
> - ${} \displaystyle \lim _{x \rightarrow a} g^{(i)}=\lim _{x \rightarrow a} g^{(i)}=0 {}$ für $i=0,1, \ldots, n-1$,
> - der Grenzwert $\displaystyle\lim _{x \rightarrow a} \frac{g^{(n)}(x)}{h^{(n)}(x)}$ existiert.
>  
> Dann gilt
> $$
> \lim _{x \rightarrow a} \frac{g(x)}{h(x)}=\lim _{x \rightarrow a} \frac{g^{(n)}(x)}{h^{(n)}(x)}
> $$

- Achtung: Zähler und Nenner werden getrennt abgeleitet! (Keine Quotientenregel)
- Oft reicht der Fall $n = 1$ aus

***
#### Anwendung

##### Fall "$\frac{\infty}{\infty}$":
In diesem Fall darf die Regel von L'Hospital direkt angewendet werden. Das heißt, wenn

$$
\lim _{x \rightarrow a} g(x)=\lim _{x \rightarrow a} h(x)=\infty
$$

gilt ebenfalls

$$
\lim _{x \rightarrow a} \frac{g(x)}{h(x)}=\lim _{x \rightarrow a} \frac{g^{(n)}(x)}{h^{(n)}(x)},
$$

sofern $f$ und $g$ differenzierbar sind und der Ausdruck auf der rechten Seite existiert.

###### Fall "$\infty \cdot 0$":
Wenn $\displaystyle \lim _{x \rightarrow a} g(x)=\infty$ und $\displaystyle \lim _{x \rightarrow \infty} h(x)=0$ ist, so gilt

$$
\lim _{x \rightarrow a} \underbrace{g(x) \cdot h(x)}_{=\infty \cdot 0}=\lim _{x \rightarrow a} \frac{h(x)}{\frac{1}{g(x)}}= \frac{0}{0}
$$

**Fall "$\infty - \infty$":**

Wenn $\lim _{x \rightarrow a} g(x)=\infty$ und $\lim _{x \rightarrow \infty} h(x)=\infty$ ist, so gilt
$$
\lim _{x \rightarrow a} \underbrace{g(x)-h(x)}_{=\infty-\infty}=\lim _{x \rightarrow a} \frac{1}{\frac{1}{g(x)}}-\frac{1}{\frac{1}{h(x)}}=\frac{\frac{1}{h(x)}-\frac{1}{g(x)}}{\frac{1}{g(x)} \cdot \frac{1}{h(x)}}= \frac{0}{0}
$$

##### Fall "$1^{\infty}, 0^{0}, \infty^{0}$":
Kann durch Logarithmieren des Ausdrucks auf "$\frac{0}{0}$" oder "$\frac{\infty}{\infty}$" zurückgeführt werden.
Als Beispiel nennen wir hier den Grenzwert

$$
\lim _{x \downarrow 0} x^x=\lim _{x \downarrow 0} e^{\ln (x) \cdot x} .
$$

Hierbei muss nun der Grenzwert $\lim _{x \downarrow 0} \ln (x) \cdot x=-\infty \cdot 0$ berechnet werden. (Dabei ist $\ln (x) \cdot x=$ $\ln \left(x^x\right)$ gerade der Logarithmus des Ausgangsterms.) Dieser kann mit der Regel von L'Hospital gelöst werden.

Schließlich bemerken wir noch, dass auch wenn $x \rightarrow \pm \infty$ untersucht wird (statt wie bisher $x \rightarrow$ $a \in \mathbb{R}$ ), die Regel von L'Hospital angewendet werden kann. Dazu nutzen wir die folgende Idee: Ersetze $x=\frac{1}{t}$ und untersuche $t \rightarrow 0$ :
$$
\lim _{x \rightarrow \infty} \frac{g(x)}{h(x)}=\lim _{t \rightarrow 0} \frac{g\left(\frac{1}{t}\right)}{h\left(\frac{1}{t}\right)} .
$$

Daraus lässt sich leicht folgern, dass die Regel von L'Hospital ganz normal auch für Grenzwerte $x \rightarrow \pm \infty$ benutzt werden darf.
##### Fall $x \rightarrow \pm \infty$:
Auch wenn $x \rightarrow \pm \infty$ untersucht wird (statt wie bisher $x \rightarrow a \in \mathbb{R}$ ), kann die Regel angewendet werden.

Idee: Ersetze $x=\frac{1}{t}$ und untersuche $t \rightarrow 0$ :

$$
\lim _{x \rightarrow \infty} \frac{g(x)}{h(x)}=\lim _{t \rightarrow 0} \frac{g\left(\frac{1}{t}\right)}{h\left(\frac{1}{t}\right)}
$$
