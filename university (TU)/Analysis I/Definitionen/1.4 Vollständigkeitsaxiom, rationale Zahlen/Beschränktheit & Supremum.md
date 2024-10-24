---
tags:
  - Mengen
flashcard: false
source: 
date created: 2024-10-24
types: 
examples: 
constructions: 
generalizations: 
justifications:
  - "[[Rationaler Zahlenraum]]"
---
***
#### Einseitige Beschränktheit

> [!definition] Beschränktheit
> Sei $M \subseteq \mathbb{R}$. Dann gelten
> 
> 1) $M$ heißt nach oben beschränkt, falls es $s \in \mathbb{R}$ gibt, so dass $x \leq s$ für alle $x \in M$ gilt.
> 2) Die Zahl $s \in \mathbb{R}$ aus 1) heißt dann obere Schranke von $M$.

***
#### Beispiele

> [!exm|*] Beispiel für Beschränktheit 
> 1. Die Intervalle $[a, b],[a, b[] a, b],,] a, b[]-,\infty, b]$ und $]-\infty, b[$ sind alle nach oben beschränkt. Eine obere Schranke ist jeweils $b$, aber auch jede reelle Zahl $c \geq b$ ist eine obere Schranke.
> 2. Die Intervalle $[a, \infty[] a,, \infty[$ und $\mathbb{R}$ sind nicht nach oben beschränkt. Wir zeigen dies exemplarisch für das Intervall $[a, \infty[$. Angenommen $s \in \mathbb{R}$ ist eine obere Schranke $s+1 \in[a, \infty[$. Dann ist aber $s$ keine obere Schranke von $[a, \infty[\mathrm{im}$ Widerspruch zur Annahme. Folglich ist $[a, \infty[$ nicht nach oben beschränkt.

***

#### Suprema

> [!definition] Suprema
> Sei $M \subseteq \mathbb{R}$ und sei $s_0 \in \mathbb{R}$ eine obere Schranke von $M$.
> 1. $s_0$ heißt Supremum (oder kleinste obere Schranke) von M, falls für jede obere Schranke $s \in \mathbb{R}$ von $M$ gilt, dass $s_0 \leq s$. Schreibweise: $s_0=\sup M$.
> 2. Ist $s_0$ ein Supremum von $M$ und gilt zusätzlich $s_0 \in M$, so heißt $s_0$ Maximum von M. Schreibweise: $s_0=\max M$.

> [!remark] Bemerkung zu Suprema
> Ist $M \subseteq \mathbb{R}$ nach oben beschränkt, so hat $M$ höchstens ein Supremum, denn sind $s_0$ und $\widetilde{s}_0$ zwei Suprema von $M$, so gilt einerseits $s_0 \leq \widetilde{s}_0$, da $s_0$ Supremum und $\widetilde{s}_0$ eine obere Schranke ist. Andererseits gilt $\widetilde{s}_0 \leq s_0$, da auch $\widetilde{s}_0$ ein Supremum und $s_0$ eine obere Schranke ist. Damit folgt dann aber $s_0=\widetilde{s}_0$.

Analog definieren wir eine *untere* Schranke, nach unten beschränkt, und nennen sie **Infimum** $(\mathrm{inf} M)$ (größte untere Schranke) und ein **Minimum**, geschrieben $\min_{} M$.

***

#### Allgemeine Beschränktheit

> [!definition] Beschränkte Mengen
> Eine Menge $M \subseteq \mathbb{R}$ heißt beschränkt, falls sie nach oben beschränkt und nach unten beschränkt ist, d.h. wenn es $s_1, s_2 \in \mathbb{R}$ gibt, so dass für alle $x \in M$ gilt:
> 
> $$
> s_1 \leq x \leq s_2 \quad
> $$

> [!exm] Beispiele für beschränkte Mengen
> 1. $\varnothing$ ist beschränkt.
> 2. $[a,b]$ ist beschränkt mit $a = \mathrm{inf}[a,b] = \min_{}[a,b], \quad b = \mathrm{sup}[a,b] = \max_{}[a,b]$
> 3. Sei $M = ]-\infty, 1[ = \{ x \in \mathbb{R} \mid x < 1 \}$, dann ist $s_{0} \coloneqq 1$ eine obere Schranke von $M$. Wir zeigen $\sup M = s_{0} = 1$
> 4. $\tilde{M} \coloneqq \{ x \in \mathbb{R} \mid x^{2} < 2 \}$ ist nach oben beschränkt, denn z.b. ist $s = \frac{3}{2}$ eine o.S.: Für alle $x \in \mathbb{R}$ gilt $x > \frac{3}{2} \implies x^{2} > \frac{3}{2}x > \frac{9}{4} > 2$, d.h. $x \notin \tilde{M}$ mit $x \in \tilde{M} \implies x \leq \frac{3}{2}$.

`\begin{proof}`
Beweis für (3) per Kontraposition. Wir zeigen $s < s_{0} \implies s \text{ ist keine obere Schranke von } M$.

Sei $s < s_{0} = 1$. Dann gilt $s < \frac{s+1}{2} < 1$, d.h. $\frac{s+1}{2} \in M$, und wegen $s < \frac{s+1}{2}$ ist $s$ keine obere Schranke von $M$.

`\end{proof}`