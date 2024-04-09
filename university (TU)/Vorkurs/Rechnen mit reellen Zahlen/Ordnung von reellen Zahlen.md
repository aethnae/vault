---
tags:
  - ordnung
  - reell
flashcard: false
source: Skript p. 12
date created: 2024-04-09
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Anordnungsaxiome für $<$ und $\leq$
> Für alle $w,x,y,z \in \mathbb{R}$ gelten folgende Aussagen.
> 
> 1. Es gilt genau einer der drei Fälle: $x < y$, $x = y$ oder $x > y$
> 2. Sind $x < y$ und $y < z$, so folgt $x < z$
> 3. Sind $x < y$ und $w \leq z$, so folgt $x + w < y + z$
> 4. Sind $x < y$ und $z > 0$, so folgt $zx < zy$
> 
> Die Axiome 2. - 4. gelten auch, wenn überall $<$ durch $\leq$ ersetzt wird.

^5cf0fa

***
#### Eigenschaften

Aus den Anordnungsaxiomen können weitere Eigenschaften von $<$ und $\leq$ hergeleitet werden, etwa folgender Satz:

> [!theorem] Abgeleitete Eigenschaften für $<$ und $\leq$
> Seien $w,x,y,z \in \mathbb{R}$. Dann gelten folgende Aussagen.
> 
> 1. Für $x < 0$ ist $-x > 0$ und für $x > 0$ ist $-x < 0$.
> 2. Sind $x < y$ und $z < 0$, so folgt $zx > zy$.
> 
> Beide Aussagen gelten auch wieder äquivalent für $\leq$.

`\begin{proof}`

Zu (1): Sei $x < 0$, es gilt $-x \leq -x$. Durch die Anwendung von [[Ordnung von reellen Zahlen#^5cf0fa|(03)]] erhalten wir $0 = x + (-x) < 0 + (-x) = -x$, d.h. es gilt $-x > 0$. Sein nun umgekehrt $x > 0$. Wir nutzen wieder $-x \leq -x$. Durch die Anwendung von [[#^5cf0fa|(03)]] erhalten wir in diesem Fall $0 = x + (-x) > 0 + (-x) = -x$, d.h. es gilt $-x < 0$.

Zu (2): Seien $x < y$ und $z < 0$. Dann folgt aus (1) zunächst $-z > 0$ und zusammen mit [[#^5cf0fa|(04)]] folgt $-zx < -zy$. Die Anwendung von [[#^5cf0fa|(03)]] für $zx + zy \leq zx + zy$ ergibt nun $-zx + (zx + zy) < -zy + (zx + zy)$ und unter Ausnutzung der Assoziativität und Kommutativität der Addition erhalten wir $zy + (-zx + zx) + zy < zx + (-zy + zy)$ und somit $zy < zx$.
`\end{proof}` 

***

