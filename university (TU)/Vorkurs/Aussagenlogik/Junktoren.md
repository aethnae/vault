---
tags:
  - operationen
  - aussagen
  - logik
flashcard: false
source: Skript p. 8
date created: 2024-04-09
types: 
examples: 
constructions: 
generalizations: 
justifications:
  - "[[Aussagen]]"
---
***
#### Definition

> [!definition] Junktoren
> Seien $A$ und $B$ [[Aussagen]].
> 
> 1. **Negation** ($\neg$): Die Aussage $\neg A$ ist wahr, falls $A$ falsch ist, und sie ist falsch, falls $A$ wahr ist. Dies kann als *Wahrheitstafel* geschrieben werden
> 
> $$
> 
\begin{array}{c|c}
A & \neg A \\
\hline \mathrm{w} & \mathrm{f} \\
\mathrm{f} & \mathrm{w}
\end{array}
> $$
> 
> 2. **Konjunktion** ($\wedge$): Die Aussage $A \wedge B$ ("$A$ und $B$") ist wahr, wenn die Aussagen einzeln wahr sind.
> 3. **Disjunktion** ($\vee$): Die Aussage $A \vee B$ ("$A$ oder $B$") ist wahr, wenn **mindestens** eine der Aussagen $A$ und $B$ wahr ist.
> 4. **Implikation** ($\implies$): Die Aussage $A \implies B$ ("Aus $A$ folgt $B$) ist falsch, falls $A$ wahr und $B$ falsch ist. Anderfalls ist $A \implies B$ stets wahr.
> 5. **Äquivalenz** ($\Leftrightarrow$): Es gilt $A \Leftrightarrow B$, falls $A$ und $B$ immer den gleichen Wahrheitswert haben. Insbesondere ist $A \Leftrightarrow B$ genau dann wahr, wenn $A \implies B$ und $B \implies A$ wahr sind.

***
#### Eigenschaften

> [!remark] "Und"-Aussagen
> Das "und" zwischen Aussagen wird oft nur als Komma geschrieben, z.B. beim Abgeschlossenen Intervall $[0,1] = \{ x \in \mathbb{R} \mid x \geq 0, x \leq 1 \}$.

> [!remark] Geläufige Formulierungen für Implikationen & Äquivalenzen
> 1. Andere Formulierungen für $A \implies B$ sind:
> 	- "$B$ gilt, wenn $A$ gilt",
> 	- "$A$ ist hinreichend für $B$",
> 	- "$B$ ist notwendig für $A$"
> 
> 2. Andere Formulierungen für $A \Leftrightarrow B$ sind:
> 	- "$A$ gilt genau dann, wenn $B$ gilt",
> 	- "$A$ gilt dann und nur dann, wenn $B$ gilt",
> 	- "$A$ ist notwendig und hinreichend für $B$"

> [!remark] Satz vom ausgeschlossenen Dritten, Kommutativität & Assoziativität
> Seien $A$, $B$ und $C$ Aussagen.
> 
> 1. Es ist immer entweder $A$ oder $\neg A$ wahr. Dies wird als *Satz vom ausgeschlossenen Dritten* bezeichnet. Insbesondere ist $A \vee \neg A$ immer wahr und $A \wedge \neg A$ immer falsch.
> 2. Konjunktion und Disjunktion sind *kommutativ*, d.h. es gelten
> 
> $$
> A \wedge B \Leftrightarrow B \wedge A \quad \text{ und } \quad A \vee B \Leftrightarrow B \vee A
> $$
> 
> 3. Desweiteren sind Konjunktion und Disjunktion auch *assoziativ*, d.h. es gelten
> 
> $$
> (A \wedge B) \wedge C \Leftrightarrow A \wedge (B \wedge C) \quad \text{ und } \quad (A \vee B) \vee C \Leftrightarrow A \vee (B \vee C)
> $$
> 
> 4. Die Implikation ist **nicht** kommutativ, und wird daher mit einem **einseitigen** Pfeil notiert:
> 
> $$
> \text{ Es gilt } x \in \mathbb{N} \implies x \in \mathbb{Z}, \text{ aber aus } x \in \mathbb{Z} \text{ folgt trotzdem nicht } x \in \mathbb{N} 
> $$

###### Wahrheitstafel für Konjunktion, Disjunktion, Implikation und Äquivalenz:

$$
\begin{array}{c|c|c|c|c|c}
A & B & A \wedge B & A \vee B & A \Rightarrow B & A \Leftrightarrow B \\
\hline \mathrm{w} & \mathrm{w} & \mathrm{w} & \mathrm{w} & \mathrm{w} & \mathrm{w} \\
\mathrm{w} & \mathrm{f} & \mathrm{f} & \mathrm{w} & \mathrm{f} & \mathrm{f} \\
\mathrm{f} & \mathrm{w} & \mathrm{f} & \mathrm{w} & \mathrm{w} & \mathrm{f} \\
\mathrm{f} & \mathrm{f} & \mathrm{f} & \mathrm{f} & \mathrm{w} & \mathrm{w}
\end{array}
$$

***
#### Beispiele

> [!exm]  
> 1. Die Aussage "Es existiert ein $x \in \mathbb{R}$ mit $x^{2} = -1$" ist falsch. Die zugehörige Negation "$\forall x \in \mathbb{R}: x^{2} \neq -1$" ist wahr.
> 2. $-1 \in \mathbb{N} \wedge 2 \in \mathbb{Z}$ ist falsch, da $-1 \notin \mathbb{N}$.
> 3. $1 \in \mathbb{N} \wedge 2 \in \mathbb{Z}$ ist wahr, da $1 \in \mathbb{N}$ und $2 \in \mathbb{Z}$ wahr sind.
> 4. $x \in \mathbb{N} \implies x \in \mathbb{Z}$ ist wahr.
> 5. $x \in \mathbb{Z} \implies x \in \mathbb{N}$ ist falsch. Damit ist auch $x \in \mathbb{Z} \Leftrightarrow x \in \mathbb{N}$ falsch.

***
