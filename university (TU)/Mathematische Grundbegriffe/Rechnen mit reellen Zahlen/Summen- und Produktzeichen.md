---
tags:
  - summen
  - produkte
  - reell
flashcard: false
source: Skript p. 14
---

***
#### Definition

> [!definition] Summen- und Produktzeichen
> Seien $m,n \in \mathbb{Z}$ und $x_{k} \in \mathbb{R}$ für $k = m, m + 1, \ldots, n$.
> 
> 1. Für $m \leq n$ definieren wir
>
> $$
> \sum_{k = m}^{n} x_{k} \coloneqq x_{m} + x_{m + 1} + \ldots + x_{n} \quad \text{ ("Die Summe der $x_{k}$ für $k$ von $m$ bis $n$") }
> $$
>
> $$
> \prod_{k = m}^{n} x_{k} \coloneqq x_{m} \cdot x_{m+1} \cdot \ldots \cdot x_{n} \quad \text{ ("Das Produkt der $x_{k}$ für $k$ von $m$ bis $n$") }
> $$
>
> 2. Für $m > n$, d.h. falls die untere Grenze größer als die obere ist, definieren wir
>
> $$
> \sum_{k = m}^{n} x_{k} \coloneqq 0 \quad \text{ (leere Summe) } \quad \text{ und } \quad \prod_{k = m}^{n} x_{k} \coloneqq 1 \quad \text{ (leeres Produkt) }
> $$

^e5ff16

***
#### Eigenschaften

Die Zahl $k$ in [[#^e5ff16|Definition 1]] nennen wir *Laufindex* der Summe oder des Produkts.
Die folgenden Rechenregeln für Summen und Produkte sind eine Konsequenz aus dem Distributivgesetz sowie den Assoziativ- und Kommutativgesetzen.

> [!theorem] Rechenregeln für Summen und Produkte
> Seien $m,n \in \mathbb{Z}$ mit $n \geq m$ und $x_{k}, y_{k}, c \in \mathbb{R}$. Dann gilt
>
> $$
> \begin{align}
 & 1. \sum_{k = m}^{n} (c \cdot x_{k}) = c \cdot \sum_{k = m}^{n} x_{k} \\
 & 2. \sum_{k = m}^{n} (x_{k} + y_{k}) = \sum_{k = m}^{n} x_{k} + \sum_{k = m}^{n} y_{k} \\
 & 3. \prod_{k = m}^{n} (c \cdot x_{k}) = c^{n - m + 1} \cdot \prod_{k = m}^{n} x_{k} \\
 & 4. \prod_{k = m}^{n} (x_{k} \cdot y_{k}) = \prod_{k = m}^{n} x_{k} \cdot \prod_{k = m}^{n} y_{k}
\end{align}
> $$

> [!definition] Indexverschiebung
> Als *Indexverschiebung* bezeichnen wir bei Summen oder Produkten eine Substitution des *Laufindex* der Form
>
> $$
> \sum_{k = m}^{n} x_{k} = \sum_{k = m + \ell}^{n + \ell} x_{k - \ell}, \quad \prod_{k = m}^{n} x_{k} = \prod_{k = m + \ell}^{n + \ell} x_{k - \ell}, \quad \ell \in \mathbb{Z} 
> $$
>
> Der Wert der Summe oder des Produkts ändert sich hierbei nicht. Das Ziel einer solchen Indexverschiebung ist meist weitere Rechnungen zu vereinfachen.

***
#### Beispiele

> [!exm|*] Beispiel einer Indexverschiebung 
> $$
> \sum_{k = -2}^{2} (k^{2} + 4k + 4) = \sum_{k = -2}^{2} (k+2)^{2} = \sum_{k = -2+2}^{2+2} (k-2+2)^{2} = \sum_{k = 0}^{4} k^{2} = 30
> $$

***
