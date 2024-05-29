---
tags:
- Logik
- Beweise
flashcard: false
source: "Übung 1"
date created: 2024-04-19
types: 
examples: 
constructions: 
generalizations: 
- "[[Junktoren]]"
- "[[Aussagen]]"
justifications:
---
***
#### Definition

> [!definition] Reihenfolge der logischen Verknüpfungen
> Die stärkste Bindung findet durch **Negationen** ($\neg$) statt, darauf folgen "und"-, sowie "oder"-[[Junktoren]] ($\vee \text{ und } \wedge$). Am schwächsten binden **Implikationen** ($\implies$) sowie **Äquivalenzen** 
> ($\Leftrightarrow$). 

***
#### Eigenschaften

- $\neg A \wedge B$ bedeutet $(\neg A) \wedge B$
- $A \wedge B \implies C$ bedeutet $(A \wedge B) \implies C$ 

***
#### Beispiele

> [!exm|*] Satz vom ausgeschlossenen Dritten 
> Für eine Aussage $A$ ist $A$ oder $\neg A$ wahr.
> 
> `\begin{proof}`
> Der Beweis wird mittels einer Wahrheitstafel geführt.
> 
> $$
> \begin{array}{c|c|c}
A & \neg A & A \vee \neg A \\
\hline w & f & w \\
f & w & w
\end{array}
> $$
> 
> Somit ist $A \vee \neg A$ immer wahr.
> `\end{proof}`

***
