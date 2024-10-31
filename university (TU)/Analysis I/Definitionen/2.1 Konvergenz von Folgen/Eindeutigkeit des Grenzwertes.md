---
tags:
- Folgen
flashcard: false
source: 
date created: 2024-10-31
proved by: 
references: 
justifications:
---
***
#### Theorem

> [!theorem] Eindeutigkeit des Folgengrenzwertes
> Eine konvergente Folge $(a_{n})_{n \in \mathbb{N}}$ reeller Zahlen hat genau einen Grenzwert.

***
#### Beweis

`\begin{proof}`
Beweis: Seien $a, b$ Grenwerte der Folge $\left(a_n\right)$. Angenommen, es gilt $a \neq b$. Dann gibt es zu $\varepsilon:=\frac{|a-b|}{2}>0$ natürliche Zahlen $\widehat{N}_{\varepsilon}, \widetilde{N}_{\varepsilon} \in \mathbb{N}$, so dass

$$
\begin{array}{ll}
\left|a_n-a\right|<\varepsilon & \text { für alle } n \geq \widehat{N}_{\varepsilon}, \\
\left|a_n-b\right|<\varepsilon & \text { für alle } n \geq \widetilde{N}_{\varepsilon} .
\end{array}
$$


Setze $N_{\varepsilon}:=\max \left\{\widehat{N}_\epsilon, \widetilde{N}_{\varepsilon}\right\}$. Dann gilt für alle $n \geq N_{\varepsilon}$, dass

$$
|a-b|=\left|a-a_n+a_n-b\right| \leq\left|a-a_n\right|+\left|a_n-b\right|<\varepsilon+\varepsilon=2 \varepsilon=|a-b| .
$$


Dies ist ein Widerspruch und folglich gilt $a=b$.

`\end{proof}`

<br> 

***
