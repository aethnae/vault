---
tags:
- Ringe
flashcard: false
source: 
date created: 2024-10-29
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Ring
> Ein Ring ist eine Menge $R$ mit zwei Abbildungen, genannt Operationen oder Verknüpfungen,
> $$
> \begin{aligned}
> & +: R \times R \rightarrow R, \quad(a, b) \mapsto a+b, \quad \text { (Addition) } \\
> & \text { * : } R \times R \rightarrow R, \quad(a, b) \mapsto a * b, \quad \text { (Multiplikation) }
> \end{aligned}
> $$
> 
> für die folgende Regeln erfüllt sind:
> 1. $(R,+)$ ist eine kommutative Gruppe.
>    (Wir nennen das neutrale Element bzgl. der Addition Null, bezeichnen es mit 0, und bezeichnen das zu $a \in R$ inverse Element mit $-a$. Wir schreiben $a-b$ anstatt $a+$ $(-b)$.)
> 2. Die Multiplikation * ist assoziativ, d. h. $(a * b) * c=a *(b * c)$ gilt für alle $a, b, c \in R$.
> 3. Es gelten die Distributivgesetze, d. h. für alle $a, b, c \in R$ gelten
> 
> $$
> \begin{aligned}
> & a *(b+c)=a * b+a * c \\
> & (a+b) * c=a * c+b * c
> \end{aligned}
> $$

- Ein Ring heißt *kommutativ*, falls $a \cdot b = b \cdot a$ für alle $a,b \in \mathbb{R}$ gilt.
- Ein Element $1 \in \mathbb{R}$ heißt *Einselement* (kurz: Eins), falls $1 \cdot a = a \cdot 1 = a$ für alle $a \in \mathbb{R}$ gilt. In diesem Fall nennen wir den Ring einen *Ring mit Eins*.

***

> [!theorem] Ringeigenschaften
> Ist $R$ ein Ring mit Eins, dann gelten folgende Aussagen:
> 1. Das Einselement in $R$ ist eindeutig bestimmt.
> 2. Es gilt $1 = 0$ genau dann, wenn $R$ der [[Nullring]] ist.

`\begin{proof}`
1. Sind $1, e \in R$ mit $1 * a=a * 1=a$ und $e * a=a * e=a$ für alle $a \in R$, dann gilt $1=e * 1=e$.
2. Übungsaufgabe.

`\end{proof}`
<br> 
****

> [!theorem] Weitere Ringeigenschaften
> In jedem Ring $R$ gelten folgende Eigenschaften
> 1. $0 \cdot a = a \cdot 0 = 0$ für alle $a \in \mathbb{R}$.
> 2. $a \cdot (-b) = -(a \cdot b) = (-a) \cdot b$ und $(-a) \cdot (-b) = a \cdot b$, für alle $a,b \in \mathbb{R}$.

`\begin{proof}`
1. Für jedes $a \in R$ gilt $0 * a=(0+0) * a=(0 * a)+(0 * a)$. Addieren wir $-(0 * a)$ auf der linken und rechten Seite dieser Identität, so erhalten wir $0=0 * a$. Genauso zeigt $\operatorname{man} a * 0=0$ für alle $a \in R$.
2. Es gilt $(a * b)+(a *(-b))=a *(b+(-b))=a * 0=0$, also ist $a *(-b)$ das $\mathrm{zu} a * b$ (eindeutig bestimmte) additiv inverse Element, d. h. $a *(-b)=-(a * b)$. Ähnlich zeigt man $(-a) * b=-(a * b)$. Zudem gilt
   $$
   \begin{aligned}
   -(a * b)+(-a) *(-b) & =a *(-b)+(-a) *(-b) \\
   & =(a+(-a)) *(-b)=0 *(-b)=0
   \end{aligned}
   $$
   
   und Addition von $a * b$ auf der linken und rechten Seite zeigt $(-a) *(-b)=a * b$.
Zwar gilt $a * 0=0 * a=0$ in jedem Ring $R$, aber aus $a * b=0$ muss nicht unbedingt $a=0$ oder $b=0$ folgen. Ein Element $a \in R$ heißt **Teiler der Null** oder **Nulleiler**, wenn ein $b \in R \backslash\{0\}$ mit $a * b=0$ existiert. Das Element $a=0$ (also die Null selbst) wird als der *triviale* Nullteiler bezeichnet.

`\end{proof}`

<br> 

***

> [!definition] Invertierbarkeit in Ringen
> Sei $(R,+, *)$ ein Ring mit Eins. Ein Element $b \in R$ heißt *invers* zu $a \in R$, falls $a * b=b * a=1$ gilt. Falls es zu $a \in R$ ein inverses Element $b \in R$ gibt, dann nennen wir $a$ invertierbar.

> [!remark] Existenz der Invertierbarkeit in Ringen
> Nicht jedes Element in einem Ring muss invertierbar sein. Ist zum Beispiel $R$ ein Ring mit Eins und $1 \neq 0$, dann ist $0 \in R$ nicht invertierbar, denn es gilt $0 * b=0 \neq 1$ für alle $b \in R$.

Ist ein Ringelement invertierbar, dann ist das zugehörige inverse Element eindeutig, wie der folgende Satz zeigt.

> [!theorem] Eindeutigkeit des inversen Elements in Ringen, Invertierbarkeit von Produkten
> Sei $(R, +, \ast)$ ein Ring mit Eins.
> 1. Falls zu $a \in R$ ein inverses Element (bezüglich *) existiert, so ist dieses eindeutig. Wir bezeichnen es dann mit $a^{-1}$.
> 2. Sind $a, b \in R$ invertierbar, so ist $a * b$ invertierbar und $(a * b)^{-1}=b^{-1} * a^{-1}$.

`\begin{proof}`
1. Ist $a \in R$ und sind $b, \tilde{b} \in R$ invers zu $a$, dann gilt $b=b * 1=b *(a * \tilde{b})=(b * a) * \tilde{b}=$ $1 * \tilde{b}=\tilde{b}$.
2. Da $a$ und $b$ invertierbar sind, ist $b^{-1} * a^{-1} \in R$ wohldefiniert. Es gilt
   $$
   \left(b^{-1} * a^{-1}\right) *(a * b)=\left(\left(b^{-1} * a^{-1}\right) * a\right) * b=\left(b^{-1} *\left(a^{-1} * a\right)\right) * b=b^{-1} * b=1.
   $$
   
   Genauso zeigt man $(a * b) *\left(b^{-1} * a^{-1}\right)=1$. Es folgt $(a * b)^{-1}=b^{-1} * a^{-1}$.

`\end{proof}`
