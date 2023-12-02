---
tags:
  - entscheidungen
  - problemsolving
week: 2023-11-08
flashcard: false
publish: true
---
***

> [!info] Definition
> Methode zur Lösung von Maximierungsproblemen unter einer Nebenbedingung, welche unter Verwendung einer Hilfsfunktion $L$ stattfindet.
#### Beispiel
*In diesem Beispiel wird die Bedingung für eine optimale Entscheidung unter Verwendung der Lagrange-Methode mathematisch bewiesen.*

Wir wissen, dass optimale Entscheidungen die Bedingung

$$
\text{MRS}(x_{1}, x_{2}) = -\frac{p_{1}}{p_{2}}
$$

erfüllen müssen, was das selbe wie

$$
\frac{\partial u \frac{x_{1}, x_{2}}{\partial x_{1}}}{\partial \frac{x_{1}, x_{2}}{\partial x_{2}}} = \frac{p_{1}}{p_{2}}
$$

ist.

Auch muss solch eine Entscheidung die [[Budgetbeschränkung]] erfüllen. Also

$$
p_{1}x_{1} + p_{2}x_{2} = m
$$

Das sind unsere beiden Gleichungen, sprich unser Maximierungsproblem und die Nebenbedingung.

$$
\max_{x_{1}, x_{2}} u(x_{1}, x_{2})
$$

unter der NB: $p_{1}x_{1} + p_{2}x_{2} = m$.

Formulieren wir nun unsere **Hilfsfunktion**,

$$
L = u(x_{1}, x_{2}) - \lambda (p_{1}x_{1} + p_{2}x_{2} - m)
$$

die sogenannte **Lamba-Funktion**.
Nach dem Theorem von Lagrange muss ein Optimum $(x_{1}^{*}, x_{2}^{*})$ folgende drei Bedingungen erster Ordnung erfüllen:

$$
\begin{aligned}
& \frac{\partial L}{\partial x_{1}} = \frac{\partial u(x_{1}^{*}, x_{2}^{*})}{\partial x_{1}} - \lambda p_{1} = 0 \\
& \frac{ \partial L }{ \partial x_{2} } = \frac{ \partial u(x_{1}^{*}, x_{2}^{*}) }{ \partial x_{2} } - \lambda p_{2} = 0 \\
& \frac{ \partial L }{ \partial \lambda } = p_{1}x_{1}^{*} + p_{2}x_{2}^{*} - m = 0
\end{aligned}
$$

Anhand dieser drei Gleichungen ist es möglich, nach $x_{1}$, respektive $x_{2}$ aufzulösen.

Hier beispielsweise für eine monotone Transformation der [[Cobb-Douglas-Präferenzen]]:

$$
\ln u(x_{1}, x_{2}) = c \ln x_{1} + d \ln {x_{2}}
$$

Wir wollen die Nachfragefunktion für $x_{1} \text{ und } x_{2}$ finden; unser Problem ist daher

$$
f(x + h) = f(x) + f'(x)h + f''(x) \frac{h^{2}}{2!} + \dots
$$