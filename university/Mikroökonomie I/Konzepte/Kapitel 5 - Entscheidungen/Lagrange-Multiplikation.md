---
tags:
  - entscheidungen
  - problemsolving
week: 2023-11-08
flashcard: false
publish: true
source: 
date created: Saturday, December 2nd 2023, 5:16:08 pm
date modified: Wednesday, January 3rd 2024, 2:24:34 pm
---
***

> [!info] Definition
> Methode zur Lösung von Maximierungsproblemen unter einer Nebenbedingung, welche unter Verwendung einer Hilfsfunktion $L$ stattfindet.
#### Beispiel
*In diesem Beispiel wird die Bedingung für eine optimale Entscheidung unter Verwendung der Lagrange-Methode mathematisch bewiesen.*

Wir wissen, dass optimale Entscheidungen die Bedingung

$$
\text{[[university/Mikroökonomie I/Konzepte/Kapitel 3 - Präferenzen/Grenzrate der Substitution|MRS]]}(x_{1}, x_{2}) = -\frac{p_{1}}{p_{2}}
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
\max_{x_{1}, x_{2}} c \ln x_{1} d \ln x_{2}
$$

unter der Nebenbedingung $p_{1}x_{1} + p_{2}x_{2} = m$.

Man setzt die Lagrange-Funktion

$$
L = c \ln x_{1} + d \ln x_{2} - \lambda (p_{1}x_{1} + p_{2}x_{2} - m)
$$

an und differenziert, um die drei Bedingungen erster Ordnung zu finden:

$$
\begin{align}
 & \frac{ \partial L }{ \partial x_{1} } = \frac{c}{x_{1}} - \lambda p_{1} = 0 \\
 & \frac{ \partial L }{ \partial x_{2} } = \frac{d}{x_{2}} - \lambda p_{2} = 0 \\
 & \frac{ \partial L }{ \partial \lambda } = p_{1}x_{1} + p_{2}x_{2} - m = 0
\end{align}
$$

Die beste Möglichkeit ist, zuerst nach $\lambda$ zu lösen, und dann $x_{1} \text{ und } x_{2}$ zu finden. Umformung und Kreuzmultiplikation ergibt

$$
\begin{align}
 & c = \lambda p_{1}x_{1} \\
 & d = \lambda p_{2}x_{2} \\
\end{align}
$$

Diese Gleichungen verlangen einfach nach Addition:

$$
c + d = \lambda (p_{1}x_{1} + p_{2}x_{2}) = \lambda m
$$

was zu

$$
\lambda = \frac{c + d}{m}
$$

führt. Substitution in die beiden ersten Gleichungen und Auflösung nach $x_{1} \text{ und } x_{2}$ ergibt wie oben

$$
\begin{align}
 & x_{1} = \frac{c}{c + d} \frac{m}{p_{1}} \\
 & x_{2} = \frac{d}{c + d} \frac{m}{p_{1}} \\
\end{align}
$$
