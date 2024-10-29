---
tags:
  - Rationale_Zahlen
flashcard: false
source: 
date created: 2024-10-24
types: 
examples: 
constructions: 
generalizations: 
justifications:
  - "[[Beschränktheit & Supremum]]"
---
***
#### Definition

> [!axiom] Vollständigkeitsaxiom
> Jede nichtleere, nach oben [[Beschränktheit & Supremum|beschränkte]] Menge $M \subseteq \mathbb{R}$ hat ein Supremum.

^81c469

> [!theorem] Satz über das Vollständigkeitsaxiom
> Sei $M \subseteq \mathbb{R}$ nichtleer und nach oben beschränkt und sei $s \in \mathbb{R}$. Dann sind folgende Aussagen äquivalent:
> 1. $s=\sup M$.
> 2. $s$ ist eine obere Schranke von $M$ und zu jedem $\varepsilon>0$ gibt es ein $x \in M$ mit $s-\varepsilon<x$. (In diesem Fall gilt sogar $s-\varepsilon<x \leq s$, da s eine obere Schranke von $M$ ist.)

`\begin{proof}`
"i) $\Rightarrow$ ii)":

Es gelte $s=\sup M$. Dann ist $s$ eine obere Schranke von $M$. Angenommen, ii) gilt nicht, d.h. es gibt ein $\varepsilon>0$, so dass für alle $x \in M$ gilt, dass $x \leq s-\varepsilon$. Dies bedeutet aber gerade, dass $s-\varepsilon$ eine weitere obere Schranke ist, und wegen $s-\varepsilon<s$ steht dies im Widerspruch zur Supremumseigenschaft von i). Folglich war unsere Annahme falsch und daher gilt ii).

"ii) $\Rightarrow$ i)":

Es gelte ii), dann ist $s$ insbesondere eine obere Schranke von $M$ und wir müssen nur noch zeigen, dass $s$ auch die kleinste obere Schranke von $M$ ist. Sei also $\widetilde{s}$ eine weitere obere Schranke von $M$. Wir zeigen $s \leq \widetilde{s}$. Angenommen $\tilde{s}<s$. Dann gilt $\varepsilon:=s-\widetilde{s}>0$ und $\widetilde{s}=s-\varepsilon$. Nach Voraussetzung in ii) gibt es ein Element $x \in M$ mit $\widetilde{s}=s-\varepsilon<x$ im Widerspruch dazu, dass $\widetilde{s}$ eine obere Schranke von $M$ ist. Also folgt $s \leq \widetilde{s}$. Da dies für beliebige obere Schranken von $\widetilde{s}$ gilt, folgt, dass $s$ das Supremum von $M$ ist.

In Worten ausgedrückt verdeutlicht der Satz noch einmal die Interpretation des Supremums als "kleinste obere Schranke": Jede Verkleinerung von einem Supremum $s$ um $\varepsilon>0$ führt dazu, dass $s-\varepsilon$ für die betrachtete Menge keine obere Schranke mehr ist.

`\end{proof}`

<br> 

***

> [!corollary] Analoger Fall für das Infimum
> Sei $M \subseteq \mathbb{R}$ eine nichtleere Teilmenge und sei $s \in \mathbb{R}$. Dann sind die folgenden Aussagen äquivalent:
> 1. $s=\inf M$.
> 2. $s$ ist eine untere Schranke von $M$ und zu jedem $\varepsilon>0$ gibt es ein $x \in M$ mit $s+\varepsilon>x$

***
#### Beschränktheit der natürlichen Zahlen

> [!theorem] Beschränktheit der natürlichen Zahlen
> Die Menge $\mathbb{N}$ der natürlichen Zahlen ist nicht nach oben beschränkt.

^0289b7

`\begin{proof}`
Angenommen, $\mathbb{N}$ ist nach oben beschränkt. Dann hat $\mathbb{N}$ nach dem [[#^81c469]]  ein Supremum $s:=\sup \mathbb{N} \in \mathbb{R}$. Da $s$ eine obere Schranke von $\mathbb{N}$ ist, gilt insbesondere

$$
n \leq s \text { für alle } n \in \mathbb{N} \text {. }
$$


Weiter existiert nach Satz $1.51 \mathrm{zu} \varepsilon=1$ ein $n_0 \in \mathbb{N}$ mit $s-\varepsilon=s-1<n_0$. Daraus folgt aber

$$
s<n_0+1 \in \mathbb{N}
$$

im Widerspruch zu (1.5). Demnach war unsere Annahme falsch und $\mathbb{N}$ ist nicht nach oben beschränkt.

`\end{proof}`

<br> 

***
#### Archimedisches Axiom

> [!axiom] Archimedisches Axiom
> Zu je zwei reellen Zahlen $a, b$ mit $a>0$ gibt es eine natürliche Zahl $n$, so dass $a \cdot n>b$.

`\begin{proof}`
Angenommen, die Aussage des Satzes ist falsch, dann gilt $a \cdot n \leq b$ für alle $n \in \mathbb{N}$.
Wegen $a>0$ erhalten wir daraus

$$
n \leq \frac{b}{a} \text { für alle } n \in \mathbb{N}
$$


Dann ist $\mathbf{N}$ aber nach oben beschränkt im Widerspruch zu [[#^0289b7]] . Folglich ist die Aussage des Satzes wahr.

`\end{proof}`