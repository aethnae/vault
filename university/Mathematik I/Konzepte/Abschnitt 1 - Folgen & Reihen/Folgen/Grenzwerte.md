---
tags:
  - folgen
week: 2023-11-14
flashcard: true
---
***

> [!def] Grenzwerte von Folgen
> Die Zahl $a \in \mathbb{R}$ heißt Grenzwert der Folge $\left(a_n\right)$, wenn es für jedes (noch so kleine) $\epsilon>0$ einen Index $n_0$ gibt, sodass
> $$
> \left|a_n-a\right|<\epsilon \quad \text { für } n \geq n_0
> $$
> gilt.

^58a6a3

- Der Grenzwert a heißt auch Limes der Folge $\left(a_n\right)$
- Wenn der Grenzwert existiert schreiben wir
$$
a=\lim _{n \rightarrow \infty} a_n \quad \text { oder } \quad a_n \stackrel{n \rightarrow \infty}{\longrightarrow} a
$$
und sagen, die Folge ist konvergent
- Existiert kein Grenzwert, dann heißt die Folge **divergent**

![[Pasted image 20231118131250.png|center|350]]

***
### Zusammenhang Grenzwerte & [[Häufungspunkte]]

- Wenn ein Grenzwert a einer Folge $\left(a_n\right)$ existiert, dann ist $a$ auch der einzige Häufungspunkt von $\left(a_n\right)$
- Wenn eine Folge $\left(a_n\right)$ genau einen Häufungspunkt $a$ hat und beschränkt ist, dann ist $a$ auch der Grenzwert von $\left(a_n\right)$

Außerdem gilt folgender Satz

> [!axm] Konvergenz
> *Jede beschränkte und monotone Folge ist konvergent.*

***
### Grenzwertrechenregeln
*Für Grenzwertrechenregeln, siehe [[university/Mathematik I/Rechengesetze#Grenzwerte|Rechengesetze]].*

> [!remark] Wichtige Grenzwerte
> *Es gilt*
> $$
> \begin{aligned}
> & \lim _{n \rightarrow \infty} \frac{1}{n^p}=0 \quad \text { für } p>0 \\
> & \lim _{n \rightarrow \infty} \sqrt[n]{c}=1 \quad \text { für } c>0 \text {, } \\
> & \lim _{n \rightarrow \infty} \sqrt[n]{n}=1 \\
> & \lim _{n \rightarrow \infty}\left(1+\frac{x}{n}\right)^n=e^x \quad \text { für } x \in \mathbb{R} \\
> &
> \end{aligned}
> $$
> Speziell für $x=1$ folgt aus dem letzten Grenzwert
> $$
> \lim _{n \rightarrow \infty}\left(1+\frac{1}{n}\right)^n=e \approx 2,71828 \ldots
> $$
