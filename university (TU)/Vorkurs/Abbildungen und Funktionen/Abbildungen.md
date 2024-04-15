---
tags:
- Abbildungen
- Funktionen
flashcard: false
source: "Skript p. 27"
date created: 2024-04-15
types: 
examples: 
- "[[Rationale Funktionen]]"
- "[[Logistische Funktionen]]"
- "[[Reellwertige Funktionen]]"
- "[[Polynomfunktionen]]"
constructions: 
- "[[Eigenschaften reeller Funktionen]]"
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Abbildungen
> Seien $X$ und $Y$ nichtleere [[university (TU)/Vorkurs/Mengen/Mengen|Mengen]]. Eine *Abbildung* $f$ von $X$ nach $Y$ ist eine Vorschrift, die jedem $x \in X$ genau ein $y = f(x) \in Y$ zuordnet. Wir schreiben kurz
> 
> $$
> f : X \rightarrow Y, \quad x \mapsto f(x),
> $$
> 
> und nennen $X$ den **Definitionsbereich**, $Y$ den **Wertebereich**, $x$ das **Argument** von $f$ und $f(x)$ das *Bild von $x$ unter $f$* (bzw. den *Funktionswert von $f$ an der Stelle $x$*).

^1c0295

> [!definition] Funktionsgraphen
> Für eine [[#^1c0295|Abbildung]] $f : X \rightarrow Y$ heißt
> 
> $$
> \Gamma_{f} \coloneqq \{ (x, f(x)) \mid x \in X \} \subseteq X \times Y
> $$
> 
> *Graph* oder *Funktionsgraph* von $f$.

***
#### Eigenschaften

- Eine Abbildung ordnet jedem zulässigen Input ($x \in X$) einen Output ($y \in Y$) zu.

![[Pasted image 20240415180142.png|center|400]]

> [!remark] Schreibweisen von Abbildungen
> Abbildungen werden beispielsweise durch
> 
> $$
> f : \mathbb{R} \setminus \{ 2 \} \rightarrow \mathbb{R}, \quad x \mapsto \frac{1}{x-2}, \quad \text{ oder } \quad f : \mathbb{R} \setminus \{ 2 \} \rightarrow \mathbb{R}, \quad f(x) \coloneqq \frac{1}{x-2}
> $$
> 
> definiert. Falls es aus dem Kontext klar ist, kann auf die Angabe von Definitions- und Wertebereich verzichtet werden, und es wird die Notation
> 
> $$
> f(x) \coloneqq \frac{1}{x-2}
> $$
> 
> genutzt.

***
#### Beispiele

> [!exm|*] Beispiele für Abbildungen 
> Abbildungen von $\mathbb{R}$ nach $\mathbb{R}$ werden auch **Funktionen** genannt.
> 
> $$
> \begin{align}
> & f_{1} : \mathbb{R} \rightarrow \mathbb{R}, \quad x \mapsto \frac{1}{4}x^{3} \\
> & f_{2} : \mathbb{R} \rightarrow [-1, \infty[, \quad x \mapsto \lvert x \rvert - 1 \\
> & f_{3} : \mathbb{R} \setminus \{ 1 \} \rightarrow \mathbb{R}, \quad x \mapsto \frac{1}{x-1}
> \end{align}
> $$
> 
> Die Funktion $f_{3}$ ist an $x = 1$ nicht definiert, da nicht durch $0$ geteilt werden kann. Einen solchen Punkt nennen wir [[Polstellen|Polstelle]].

> [!exm|*] Beispiele für unreguläre Abbildungen 
> 1. *Abbildung zwischen endlichen Mengen*
> 	Seien $X = \{ 1,2,3 \}, Y = \{ a,b,c,d \}$ und $f : X \rightarrow Y$ mit $f(1) = a, \quad f(2) = b, \quad f(3) = a$
> 	
> 	![[Pasted image 20240415183757.png|150]]
> 
> 2. *Identitätsabbildung*
> 	Sei $X \neq \varnothing$ eine Menge. Dann ist
> 	
> 	$$
> 	\text{id}_{x} : X \rightarrow X, \quad x \mapsto x
> 	$$
> 	
> 	die **Identitätsabbildung** oder **Identität** auf $X$
> 
> 3. Auf- und Abrunden
> 	$$
> 	\begin{array}{ll}
\lceil\cdot\rceil: \mathbb{R} \rightarrow \mathbb{Z}, & x \mapsto \min \{z \in \mathbb{Z} \mid z \geq x\} \\
\lfloor\cdot\rfloor: \mathbb{R} \rightarrow \mathbb{Z}, & x \mapsto \max \{z \in \mathbb{Z} \mid z \leq x\} \\
\end{array}
> 	$$
> 	(Hierbei steht der Punkt „"“ als Platzhalter für den Input. Für $D \subseteq \mathbb{R}$ ist $x \in D$ das **Minimum**, $\text{kurz } x=\min D$, (bzw. **Maximum**, ${} \text{kurz } x=\max D {}$ ) von $D$, falls $x<y$ (bzw. $x>y$ ) für alle $y \in D \backslash\{x\}$ gilt.)
> 	
> 	Beispiel: $\lceil \pi \rceil = 4$ und $\lfloor \pi \rfloor = 3$.
> 
> 4. Parabelfunktion im $\mathbb{R}^{2}$
> 	$$
> 	f : \mathbb{R}^{2} \mapsto \mathbb{R}, \quad (x,y) \mapsto x^{2} + y^{2}
> 	$$
> 	
> 	Beispiel: $f(3,1) = 3^{2} + 1^{2} = 10$
***
