---
tags:
  - reihen
week: 2023-11-21
flashcard: true
---
***

> [!def] Konvergenzkriterien für Reihen
> Damit eine [[Reihen|Reihe]] $\left(s_n\right)$ konvergiert, ist es notwendig, dass $a_n$ gegen null konvergiert. Also gilt
> $$
> \left(s_n\right) \text { konvergent } \Rightarrow \lim _{n \rightarrow \infty} a_n=0
> $$

**Wichtig:**
Das notwendige Kriterium ist nicht hinreichend!

Die harmonische Reihe $\displaystyle \sum_{i=1}^{\infty} \frac{1}{i}$ erfüllt zwar $a_n=\frac{1}{n} \stackrel{n \rightarrow \infty}{\longrightarrow} 0$, aber die Reihe ist divergent.

**Bemerkung:**
Die Aussage des notwendigen Kriteriums ist äquivalent zu
$$
\lim _{n \rightarrow \infty} a_n \neq 0 \Rightarrow\left(s_n\right) \text{ ist divergent }
$$
***
### Einfache Konvergenzkriterien

> [!axm] Beschränktheitskriterium
> Es gelte $a_n \geq 0, n \in \mathbb{N}$.
> Dann ist die Reihe $\displaystyle \sum_{n=1}^{\infty} a_n$ genau dann konvergent, wenn $\left(s_n\right)$ beschränkt ist.

> [!axm] Majorantenkriterium
> Für $\left(a_n\right)$ und $\left(b_n\right)$ gelte $\left|a_n\right| \leq b_n$ für $n \in \mathbb{N}$. Zusätzlich konvergiere die Reihe $\displaystyle \sum_{n=1}^{\infty} b_n$. Dann konvergiert die Reihe $\displaystyle \sum_{n=1}^{\infty} a_n$ ebenfalls.

**Beispiel:**
Die hyperharmonische Reihe $\displaystyle \sum_{n=1}^{\infty} \frac{1}{n^2}$ konvergiert. Da $\frac{1}{n^2+1}<\frac{1}{n^2}$ für alle $n \in \mathbb{N}$, konvergiert die Reihe $\displaystyle \sum_{n=1}^{\infty} \frac{1}{n^2+1}$ ebenfalls.

> [!axm] Quotientenkriterium
> Es sei $\left(a_n\right)$ eine Folge. Gilt
> $$
> \lim _{n \rightarrow \infty}\left|\frac{a_{n+1}}{a_n}\right|=q<1,
> $$
> so ist die Reihe $\displaystyle \sum_{n=1}^{\infty} a_n$ konvergent.

> [!axm] Wurzelkriterium
> Es sei $\left(a_n\right)$ eine Folge. Gilt
> $$
> \lim _{n \rightarrow \infty} \sqrt[n]{\left|a_n\right|}=q<1
> $$
> so ist die Reihe $\displaystyle \sum_{n=1}^{\infty} a_n$ konvergent.

- Gilt $\displaystyle \lim _{n \rightarrow \infty}\left|\frac{a_{n+1}}{a_n}\right|=q>1$, dann ist die Reihe divergent.
- Gilt $\displaystyle \lim _{n \rightarrow \infty} \sqrt[n]{\left|a_n\right|}=q>1$, dann ist die Reihe divergent.
- Im Falle $\displaystyle \lim _{n \rightarrow \infty}\left|\frac{a_{n+1}}{a_n}\right|=1 \quad$ bzw. $\quad \lim _{n \rightarrow \infty} \sqrt[n]{\left|a_n\right|}=1 \quad$ kann man keine Aussage treffen.
