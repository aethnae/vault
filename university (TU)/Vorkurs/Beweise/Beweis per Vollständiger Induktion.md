---
tags:
- Beweise
- Logik
flashcard: false
source: "Skript p. 23 ff."
date created: 2024-04-11
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

Beim Prinzip der "vollständigen Induktion" beweisen wir eine Aussage für alle natürlichen Zahlen $n \in \mathbb{N}$, die größer oder gleich einem bestimmten Startwert $n_{0} \in \mathbb{N}$ sind, z.b.

$$
\sum_{k = 1}^{n} k = \frac{n(n+1)}{k}, \quad \text{ für alle } n \in \mathbb{N}, n \geq 1
$$

Da es sich hierbei um eine Aussage fur unendlich viele verschiedene Zahlen handelt, kann die Aussage nicht für jede Zahl einzeln bewiesen werden. Stattdessen nutzen wir das Prinzip der vollständigen Induktion, welches auf folgender Feststellung zu den natürlichen Zahlen beruht. Ist $A(n)$ eine Aussage, die für $n = 0$ wahr ist, und beim "Weiterzählen" wahr bleibt, so gilt sie für alle natürlichen Zahlen.

> [!definition] Prinzip der vollständigen Induktion
> Um eine Aussage $A(n)$ für alle $n \in \mathbb{N}$ mit $n \geq n_{0}$ (also ab einem **Startwert** $n_{0}$) zu beweisen, gehen wir folgendermaßen vor.
> 
> 1. *Induktionsanfang* (IA): Wir zeigen, dass $A(n_{0})$ gilt.
> 2. *Induktionsvoraussetzung* (IV): Wir nehmen an, dass $A(n)$ für ein festes, aber beliebiges $n \geq n_{0}$ richtig ist.
> 3. *Induktionsschritt* (IS): Wir zeigen "$A(n) \implies A(n+1)$", also dass **aus** der Richtigkeit von $A(n)$ die Richtigkeit von $A(n+1)$ folgt.
> 
> Zusammen ist die Aussage dann für alle $n \geq n_{0}$ bewiesen.

***
#### Eigenschaften

- Der Beweis per vollständiger Induktion gehört zu den wenigen Ausnahmen, bei denen nach einem festen Schema bewiesen wird.
- Er kann analog zu einem "Dominoeffekt" beschrieben werden: Wenn der erste umgestoßene Dominostein das Umfallen eines weiteren verursacht, fällt irgendwann jeder der unendlich vielen Dominosteine um

***
#### Beispiele

> [!exm|*] Beweis der Gauß'schen Summenformel per vollständiger Induktion 
> Für alle $n \in \mathbb{N}, n \geq 1$ gilt
> 
> $$
> \sum_{k = 1}^{n} k = 1 + 2 + \ldots + n = \frac{n(n + 1)}{2}
> $$
> 
> `\begin{proof}`
> Wir beweisen den Satz per vollständiger Induktion über $n$.
> 
> 1. **IA**: Für $n = 1$ ist $\sum_{k = 1}^{n}k = 1 = \frac{1(1+1)}{2}$.
> 2. **IV**: Für ein $n \in \mathbb{N}, n \geq 1$, gelte $\sum_{k = 1}^{n}k = \frac{n(n+1)}{2}$.
> 3. **IS**: Wir zeigen, dass die Behauptung auch für $n+1$ gilt, d.h. $\sum_{k = 1}^{n}k = \frac{(n+1)(n+2)}{2}$
>    
> $$
> \begin{align}
\sum_{k = 1}^{n+1} k &  = \sum_{k = 1}^{n} k + (n+1) = \frac{n(n+1)}{2} + (n+1) \\ \\
 & = \frac{n(n+1)}{2} + \frac{2(n+1)}{2} \\
 & = \frac{n(n+1) + 2(n+1)}{2} = \frac{(n+1)(n+2)}{2}
\end{align}
> $$
> 
> `\end{proof}`

***

