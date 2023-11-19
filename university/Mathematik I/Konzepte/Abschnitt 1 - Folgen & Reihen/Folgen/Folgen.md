---
tags:
  - folgen
week: 
flashcard: false
---
***

```ad-important
title: Definition
Eine (reellwertige) Folge ist eine Funktion $a: \mathbb{N} \rightarrow \mathbb{R}$ 
(*Allgemeiner auch $a: \mathbb{N} \cup\{0\} \rightarrow \mathbb{R}$ bzw. $a: D \rightarrow \mathbb{R}$ mit $D \subseteq \mathbb{N} \cup\{0\}$*).

```

- Kurzschreibweisen für Folgen: $(a_{n})_{n \geq 1} \text{ oder } (a_{n}, n \in \mathbb{N})$
##### Beispiel:

Folge $a : \mathbb{N} \rightarrow \mathbb{R}, n \mapsto \frac{1}{n}$.

**Kurzschreibweise**:

$$
\left( \frac{1}{n} \right)_{n \geq 1} \text{ oder } a_{n} = \frac{1}{n}, n \in \mathbb{N}
$$

![[Pasted image 20231114194853.png|450]]

***
### Bildungsgesetze für Folgen

- Eine Folge kann auf verschiedene Arten beschrieben werden

```ad-note
title: Explizites Bildungsgesetz
$$
a_n=f(n) \quad \text{ für alle } n \in \mathbb{N}
$$
- Explizite Formel für jedes Folgenglied

**Beispiel**:
$$
a_n=\frac{128}{2^n}+64, \quad n \in \mathbb{N}
$$
```

```ad-note
title: Rekursives Bildungsgesetz
$$
\begin{aligned}
a_1 & =c \\
a_{n+1} & =f\left(a_n\right) \quad \text { für alle } n \in \mathbb{N}
\end{aligned}
$$
- Expliziter Anfangswert $a_1$
- Formel für aufeinanderfolgende Folgenglieder

**Beispiel**:

$$
\begin{aligned}
a_1 & =128 \\
a_{n+1} & =\frac{a_n}{2}+32
\end{aligned}
$$
```
