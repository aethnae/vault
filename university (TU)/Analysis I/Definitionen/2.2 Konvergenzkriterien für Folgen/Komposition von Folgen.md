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

> [!theorem] Komposition mehrerer Folgen
> Seien $\left(a_n\right),\left(b_n\right)$ konvergente reelle Zahlenfolgen mit den Grenzwerten a bzw. $b$ und sei $c \in \mathbb{R}$. Dann sind auch $\left(a_n+b_n\right),\left(c a_n\right)$ und $\left(a_n b_n\right)$ konvergente Folgen und es gilt:
> 1) $\lim _{n \rightarrow \infty}\left(a_n+b_n\right)=a+b$,
> 2) $\lim _{n \rightarrow \infty}\left(c a_n\right)=c \cdot a$,
> 3) $\lim _{n \rightarrow \infty}\left(a_n b_n\right)=a \cdot b$.
> 4) Gilt zusätzlich $b \neq 0$ und $b_n \neq 0$ für alle $n \in \mathbb{N}$, so ist auch die Folge ${} \displaystyle \left(\frac{a_n}{b_n}\right) {}$ konvergent und es gilt
>    
>    $$
>    \lim _{n \rightarrow \infty} \frac{a_n}{b_n}=\frac{a}{b} .
>    $$


***
#### Beweis

`\begin{proof}`
1. Sei $\varepsilon>0$ beliebig. Dann gibt es zu $\widetilde{\varepsilon}:=\frac{\varepsilon}{2}$ natürliche Zahlen $\widehat{N}, \widetilde{N}$, so dass
   
   $$
   \begin{array}{ll}
   \left|a_n-a\right|<\frac{\varepsilon}{2} & \text { für alle } n \geq \widehat{N}, \\
   \left|b_n-b\right|<\frac{\varepsilon}{2} & \text { für alle } n \geq \widetilde{N} .
   \end{array}
   $$
   
   Setze $N=\max \{\hat{N}, \tilde{N}\}$. Dann gilt für alle $n \geq N$, dass
   
   $$
   \left|\left(a_n+b_n\right)-(a+b)\right|=\left|a_n-a+b_n-b\right| \leq\left|a_n-a\right|+\left|b_n-b\right|<\frac{\varepsilon}{2}+\frac{\varepsilon}{2}=\varepsilon .
   $$
   
   Da $\varepsilon$ beliebig war, folgt, dass $a+b$ der Grenzwert der Folge $\left(a_n+b_n\right)$ ist.
2. Übung
3. 

`\end{proof}`

<br> 

***
