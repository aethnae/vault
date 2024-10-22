---
tags:
  - Abbildungen
flashcard: false
source: 
date created: 2024-10-21
proved by: 
references: 
justifications:
  - "[[Injektivität, Surjektivität & Bijektivität]]"
---
***
#### Theorem

> [!theorem] Satz über Bijektivität (Eindeutigkeit)
> Eine Abbildung $f: X \to Y$ ist genau dann bijektiv, wenn es für jedes $y \in Y$ genau ein $x \in X$ mit $f(x) = y$ gibt.

^dce4b4

***
#### Beweis

`\begin{proof}`
"$\implies$":

Sei $f: X \to Y$ bijektiv. Sei $\tilde{y} \in Y$ (beliebig aber fest). Da $f$ surjektiv ist, existiert ein $\tilde{x} \in X$ mit $f(\tilde{x}) = \tilde{y}$. Sei $\hat{x} \in X$ mit $f(\hat{x}) = \tilde{y}$. Dann gilt $\tilde{y} = f(\hat{x}) = f(\tilde{x})$. Da $f$ injektiv ist, folgt $\tilde{x} = \hat{x}$. Es existiert also genau ein $\tilde{x} \in X$ mit $f(\tilde{x}) = \tilde{y}$.

"$\impliedby$":

Da es für jedes $y \in Y$ ein $x \in X$ gibt mit $f(x) = y$, gilt $f(X) = Y$, also ist $f$ surjektiv. Seien $x_{1},x_{2} \in X$ mit $f(x_{1}) = f(x_{2}) = y \in Y$. Da es genau ein $x \in X$ mit $f(x) = y$ gibt, folgt $x_{1} = x_{2}$, also ist $f$ injektiv.

`\end{proof}`

<br> 

***

> [!theorem] Satz über Bijektivität mittels Identität
> Eine Abbildung $f: X \to Y$ ist genau dann bijektiv, wenn es eine Abbildung $g: Y \to X$ gibt mit ${} g \circ f = \mathrm{Id}_{x} {}$ und $f \circ g = \mathrm{Id}_{y}$.

^7fa63f

`\begin{proof}`
"$\implies$":

Sei $f$ bijektiv. Nach [[#^dce4b4]] existiert zu jedem $y \in Y$ genau ein $x_{y} \in X$ mit $f(x_{y}) = y$. Wir definieren die Abbildung

$$
g: Y \to X, \; g(y) = x_{y}
$$

Sei nun ein $\tilde{y} \in Y$ gegeben, dann gilt $(f \circ g)(\tilde{y}) = f(g(\tilde{y})) = f(x_{\tilde{y}}) = \tilde{y}$, also $f \circ g = \mathrm{Id}_{y}$. Ist $\tilde{x} \in X$ gegeben, dann ist $f(\tilde{x}) = \tilde{y} \in Y$. Nach [[#^dce4b4]] gibt es genau ein $x_{\tilde{y}} \in X$ mit $f(x_{\tilde{y}}) = \tilde{y}$, also ist $\tilde{x} = x_{\tilde{y}}$, denn $f$ ist injektiv. Es folgt

$$
(g \circ f)(\tilde{x}) = g(f(\tilde{x})) = g(\tilde{y}) = x_{\tilde{y}} = \tilde{x}
$$ 

also ist $g \circ f = \mathrm{Id}_{X}$.

"$\impliedby$":

Nach Annahme ist $g \circ f = \mathrm{Id}_{X}$, also ist $g \circ f$ injektiv. Aus Satz [[Komposition von Abbildungen#^ec86a8]] folgt, dass $f$ injektiv ist. Aus $f \circ g = \mathrm{Id}_{y}$ und [[Komposition von Abbildungen#^ec86a8]] (4) folgt, dass $f$ surjektiv ist.  

`\end{proof}`

<br> 

***
#### Zusammenhang zur Umkehrabbildung

Sei $f$ injektiv und $g$ eine Abbildung wie in [[#^7fa63f]] mit $g \circ f = \mathrm{Id}_{x}$ und $f \circ g = \mathrm{Id}_{y}$. Sei $h: X \to Y$ mit $h \circ f = \mathrm{Id}_{x}$ und $f \circ h = \mathrm{Id}_{y}$. Es gilt also

$$
h = \mathrm{Id}_{x} \circ h = (g \circ f) \circ h = g \circ (f \circ h) = g \circ \mathrm{Id}_{y} = g
$$

^c2b5d8

Es besteht also **Eindeutigkeit** bezüglich $g$ wie in [[#^7fa63f]] bestimmt. 

