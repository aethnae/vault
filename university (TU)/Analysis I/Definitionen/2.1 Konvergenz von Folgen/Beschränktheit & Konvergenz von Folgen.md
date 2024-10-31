---
tags:
- Folgen
flashcard: false
source: 
date created: 2024-10-31
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Beschränktheit von Folgen
> Eine Folge $(a_{n})_{n \in \mathbb{N}}$ heißt *beschränkt*, falls die Menge $\{ a_{n} \mid n \in \mathbb{N} \}$ [[Beschränktheit & Supremum#^922d3d|beschränkt]]  ist.

> [!remark] Äquivalenz der Beschränktheit
> Offenbar sind für eine Folge $\left(a_n\right)_{n \in \mathbb{N}}$ die folgenden Aussagen äquivalent:
> 1. $\left(a_n\right)$ ist beschrănkt.
> 2. Es gibt $k, K \in \mathbb{R}$, so dass $k \leq a_n \leq K$ für alle $n \in \mathbb{N}$ gilt.
> 3. Es gibt $M>0$, so dass $\left|a_n\right| \leq M$ für alle $n \in \mathbb{N}$ gilt.

***
#### Eigenschaften

> [!theorem] Konvergenz $\implies$ Beschränktheit
> Jede konvergente Folge reeller Zahlen ist beschränkt.

`\begin{proof}`
Sei $\left(a_n\right)_{n \in N}$ eine konvergente Folge mit Grenzwert $a$. Dann gibt es zu $\varepsilon:=1>0$ ein $N_1 \in \mathbb{N}$, so dass $\left|a_n-a\right|<1$ für alle $n \geq N_1$ gilt. Damit erhalten wir

$$
\left|a_n\right|=\left|a+a_n-a\right| \leq|a|+\left|a_n-a\right|<|a|+1
$$

für alle $n \geq N_1$. Setzen wir daher

$$
M:=\max \left\{\left|a_0\right|,\left|a_1\right|, \ldots,\left|a_{N_1-1}\right|,|a|+1\right\},
$$

so gilt $\left|a_n\right| \leq M$ für alle $n \in \mathbb{N}$ und daher ist $\left(a_n\right)$ beschränkt.

`\end{proof}`

<br> 

***
