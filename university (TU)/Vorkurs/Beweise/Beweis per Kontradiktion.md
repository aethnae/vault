---
tags:
- Beweise
- Logik
flashcard: false
source: "Skript p. 22" 
date created: 2024-04-11
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Beweis per Kontradiktion (Widerspruchsbeweis)
> Ein weiteres indirektes Beweisverfahren ist der Beweis per **Kontradiktion**. Bei diesem nehmen wir zunächst an, dass die Voraussetzung $A$ wahr und die Behauptung $B$ falsch ist. Unter dieser Annahme konstruieren wir danach einen Widerspruch, d.h. wir zeigen, dass
> "$A \wedge \neg B$" falsch ist (bzw. dass "$\neg(A \wedge \neg B)$" wahr ist).

***
#### Eigenschaften



***
#### Beispiele

> [!exm|*] Beispiel für einen Beweis per Kontradiktion 
> Für alle $m,n \in \mathbb{Z}$ gilt $m^{2} \neq 4n + 2$.
> 
> `\begin{proof}`
> Die Voraussetzung des Satzes ist $m,n \in \mathbb{Z}$, und die Behauptung ist $m^{2} \neq 4n +2$. Wir nehmen an, dass $m,n \in \mathbb{Z}$ mit $m^{2} = 4n +2$ existieren (Aussage $A \wedge \neg B$). Insbesondere würde dann
> 
> $$
> m^{2} = 4n + 2 = 2(2n +1)
> $$
> 
> gelten, d.h. $m^{2}$ ist eine gerade Zahl. Wegen [[Beweis per Kontraposition#^707a66|diesem]] Satz ist dann auch $m$ gerade, d.h. es existiert ein $k \in \mathbb{Z}$ mit $m = 2k$. Hieraus folgt
> 
> $$
> \begin{align}
 & m^{2} = (2k)^{2} = 4k^{2} = 4n + 2 = 2(2n +1) \\
\Leftrightarrow \quad & 2k^{2} = 2n + 1
\end{align}
> $$
> 
> Weil die linke Seite der letzten Gleichung gerade und die rechte Seite ungerade ist, liegt ein Widerspruch vor. Eine ganze Zahl ist nämlich entweder gerade oder ungerade. Somit war unsere Annahme falsch. Es existieren also keine $m,n \in \mathbb{Z}$ mit $m^{2} = 4n + 2$.
> 
> `\end{proof}`

***
