---
tags:
  - ableitungen
week: 2023-12-19
flashcard: false
publish: true
---
***

> [!def] Partielle Ableitungen 
> Für eine Funktion $z=f(x, y)$ ist die partielle Ableitung nach $x$ bzw. $y$ an der Stelle $\left(x_0, y_0\right)$ definiert durch
> 
> $$
> \begin{aligned}
> & \left.\frac{\partial f}{\partial x}\right|_{\substack{x=x_0 \\
> y=y_0}}=\lim _{\Delta x \rightarrow 0} \frac{f\left(x_0+\Delta x, y_0\right)-f\left(x_0, y_0\right)}{\Delta x} \\
> & \left.\frac{\partial f}{\partial y}\right|_{\substack{x=x_0 \\
> y=y_0}}=\lim _{\Delta y \rightarrow 0} \frac{f\left(x_0, y_0+\Delta y\right)-f\left(x_0, y_0\right)}{\Delta y}
> \end{aligned}
> $$

^96239c

**Schreibweisen:**

$$
\left.\frac{\partial f}{\partial x}\right|_{\substack{x=x_0 \\
y=y_0}} \quad \text{ oder } \quad \frac{ \partial f(x,y) }{ \partial x }|_{\substack{x=x_{0} \\ y=y_{0}}} \quad \text{ oder } \quad \frac{\partial f}{\partial x}\left(x_0, y_0\right) \quad \text { oder } \quad f_x\left(x_0, y_0\right)
$$

**Herangehensweise:**
$f(x,y)$ kann differenziert werden, indem man die Funktion unter Konstanthaltung der einen Variablen nach der anderen differenziert.

***
#### Partielle Ableitungen höherer Ordnung

> [!def] Partielle Ableitungen höherer Ordnung 
> Die partiellen Ableitungen der partiellen Ableitungsfunktionen $f_x$ und $f_y$ heißen **partielle Ableitungen zweiter Ordnung**. Es ergeben sich vier partielle Ableitungen zweiter Ordnung:
> 
> $$
> \begin{aligned}
> \frac{\partial^2 f}{\partial x^2} & =\frac{\partial}{\partial x}\left(\frac{\partial f}{\partial x}\right)=f_{x x} & \frac{\partial^2 f}{\partial y \partial x} & =\frac{\partial}{\partial y}\left(\frac{\partial f}{\partial x}\right)=f_{x y} \\
> \frac{\partial^2 f}{\partial x \partial y} & =\frac{\partial}{\partial x}\left(\frac{\partial f}{\partial y}\right)=f_{y x} & \frac{\partial^2 f}{\partial y^2} & =\frac{\partial}{\partial y}\left(\frac{\partial f}{\partial y}\right)=f_{y y}
> \end{aligned}
> $$
> 
> Existieren alle partiellen zweiter Ordnung, heißt die Funktion $f$ **zweimal partiell differenzierbar**.
> 

Analog zu Ableitungen zweiter Ordnung werden für $i_1, \ldots, i_n \geq 0$ die partiellen Ableitungen der Ordnung $m=i_1+\cdots+i_n$

$$
\frac{\partial^m f}{\partial x_1^{i_1} \ldots \partial x_n^{i_n}}
$$

definiert.

> [!lemma] Bemerkung 
> Dabei bedeutet $i_{j} = 0$, dass nach der Variable $x_{j}$ nicht partiell abgeleitet wird.

***
#### Verallgemeinerung

> [!def] Partielle Ableitungen 
> Für eine Funktion $z=f\left(x_1, \ldots, x_n\right)$ ist die partielle Ableitung nach $x_i$ an der Stelle $x^{(0)}=\left(x_1^{(0)}, \ldots, x_n^{(0)}\right)$ definiert durch
> 
> $$
> \left.\frac{\partial f}{\partial x_i}\right|_{x=x^{(0)}}=\lim _{\Delta x_i \rightarrow 0} \frac{f\left(x_1^{(0)}, \ldots, x_i^{(0)}+\Delta x_i, \ldots, x_n^{(0)}\right)-f\left(x_1^{(0)}, \ldots, x_i^{(0)}, \ldots, x_n^{(0)}\right)}{\Delta x_i}
> $$

> [!def] Stetigkeit mehrdimensionaler Funktionen
> Die Funktion $f: \mathbb{R}^n \rightarrow \mathbb{R}$ heißt stetig in $x^{(0)}=\left(x_1^{(0)}, \ldots, x_n^{(0)}\right)$, wenn
> 
> $$
> \lim _{\substack{x_i \rightarrow x_i^{(0)} \\ i=1, \ldots, n}} f\left(x_1, \ldots, x_n\right)=f\left(x_1^{(0)}, \ldots, x_n^{(0)}\right)
> $$
> 
> gilt.

