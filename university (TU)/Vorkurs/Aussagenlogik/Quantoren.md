---
tags:
  - aussagen
  - logik
flashcard: false
source: Skript p. 9
date created: 2024-04-09
types: 
examples: 
constructions: 
generalizations: 
justifications:
  - "[[Junktoren]]"
---
***
#### Definition

> [!definition] Quantoren
> Sei $M$ eine *nichtleere* Menge und für jedes $x \in M$ sei $A(x)$ eine Aussage.
> 
> 1. Die Aussage "Für alle $x \in M$ gilt $A(x)$" schreiben wir kurz als $\forall x \in M : A(x)$. Dabei bezeichnet $\forall$ den **Allquantor**.
> 2. Die Aussage "Es existiert ein $x \in M$ für das $A(x)$ gilt." schreiben wir kurz als $\exists x \in M : A(x)$. Dabei bezeichnet $\exists$ den **Existenzquantor**.

***
#### Eigenschaften

> [!theorem] 
> Seien $A$ und $B$ zwei Aussagen. Dann gilt
> 
> 1. $\neg (A \wedge B) \Leftrightarrow \neg A \vee \neg B$
> 2. $\neg (A \vee B) \Leftrightarrow \neg A \wedge \neg B$

`\begin{proof}`

Die Vorherigen Aussagen können durch eine Wahrheitstafel bewiesen werden.

$$
\begin{array}{c|c|c|c|c|c|c|c|c|c}
A & B & \neg A & \neg B & A \wedge B & \neg(A \wedge B) & \neg A \vee \neg B & A \vee B & \neg(A \vee B) & \neg A \wedge \neg B \\
\hline \mathrm{w} & \mathrm{w} & \mathrm{f} & \mathrm{f} & \mathrm{w} & \mathbf{f} & \mathbf{f} & \mathrm{w} & \mathbf{f} & \mathbf{f} \\
\mathrm{w} & \mathrm{f} & \mathrm{f} & \mathrm{w} & \mathrm{f} & \mathbf{w} & \mathbf{w} & \mathrm{w} & \mathbf{f} & \mathbf{f} \\
\mathrm{f} & \mathrm{w} & \mathrm{w} & \mathrm{f} & \mathrm{f} & \mathbf{w} & \mathbf{w} & \mathrm{w} & \mathbf{f} & \mathbf{f} \\
\mathrm{f} & \mathrm{f} & \mathrm{w} & \mathrm{w} & \mathrm{f} & \mathbf{w} & \mathbf{w} & \mathrm{f} & \mathbf{w} & \mathbf{w}
\end{array}
$$

Somit haben $\neg (A \wedge B)$ und $\neg A \vee \neg B$, sowie $\neg (A \vee B)$ und $\neg A \wedge \neg B$ die gleiche Wahrheitswertbelegung. Die Aussagen sind also jeweils äquivalent.
`\end{proof}`

***
#### Beispiele

> [!exm|*] <% tp.file.cursor(4) %> 
> <% tp.file.cursor(5) %>

***
