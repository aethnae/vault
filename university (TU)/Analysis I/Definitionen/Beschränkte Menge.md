---
tags:
- Menge
flashcard: false
source: 
date created: 
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***

> [!definition] Nach oben beschränkte Menge
> Es sein $M \in \mathbb{R}$.
> - $M$ heißt nach oben *beschränkt*, falls es ein $s \in \mathbb{R}$ gibt, sodass $x \leq s \; \forall x \in M$
> - Die Zahl $s$ heißt "obere Schranke" von $M$

> [!definition] Supremum
> Es sei $M \in \mathbb{R}$ und $s_{0} \in \mathbb{R}$ eine obere Schranke.
> - $s_{0}$ heißt **Supremum** von $M$, falls für jede obere Schranke $s \in \mathbb{R}$ von $M$ gilt, dass $s_{0} \leq s$
> - Ist $s_{0}$ ein Supremum von $M$ und gilt zusätzlich, dass $s_{0} \in M$, dann heißt $s_{0}$ **Maximum**
> 	- Wir schreiben $s_{0}$ in diesem Fall auch als $\max_{}(M)$

`\begin{proof}`
Es sei $A \subseteq \mathbb{R}$ nach oben beschränkt und nicht leer. Es sei $a_{0} \in \mathbb{R}$ eine obere Schranke von $A$. Da $A \neq \varnothing$ finden wir ein $b_{0} \in A$, insbesondere gilt damit

$$
b_{0} \leq a_{0}
$$

Wir definieren rekursiv nun zwei Folgen $(a_{n})_{n \in \mathbb{N}}, (b_{n})_{n \in \mathbb{N}}$ und definieren

$$
x_{n} = \frac{b_{n} + a_{n}}{2}
$$

und

$$
a_{n+1} = \begin{cases}
x_{n}  & \text{ falls } x_{n} \text{ eine obere Schranke von } A \\
a_{n}  & \text{ anderenfalls }
\end{cases}
$$

und

$$
b_{n+1} = \begin{cases}
b_{n}  & \text{ falls } x_{n} \text{ eine obere Schranke von } A \text{ ist } \\
b  & \text{ sonst, so dass } x_{n} < b < a_{n}
\end{cases}
$$

Damit gilt $b_{n} \in A \; \forall n \in \mathbb{N}$ und $(a_{n})_{n \in \mathbb{N}}$ ist eine Folge von oberen Schranken.

Zu zeigen ist nun, dass $a_{n}$ eine Cauchy-Folge ist. Dazu sei $n \leq m$.

Es gilt

$$
\lvert a_{n} - a_{n-1} \rvert = \begin{cases}
0  & \text{ falls } x \text{ eine obere Schranke von } A \\
\frac{1}{2}\lvert b_{n} - a_{n} \rvert  & \text{ sonst } 
\end{cases}
$$

außerdem gilt auch

$$
\lvert b_{n+1} - a_{n+1} \rvert \leq \frac{1}{2} \lvert b_{n} - a_{n} \rvert \leq \ldots \leq \frac{1}{2} \lvert b_{0} - a_{0} \rvert 
$$



`\end{proof}`



> [!definition] Beschränkte Menge
> Eine Menge $M \subseteq \mathbb{R}$ heißt *beschränkt*, genau dann wenn $M$ nach oben und unten beschränkt ist, d.h.
> 
> $$
> \exists s_{0}, s_{1} \in \mathbb{R} : s_{0} \leq x \leq s_{1} \; \forall x \in M
> $$

