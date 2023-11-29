---
tags:
  - übung
week: 2023-11-28
publish: true
---
***
##### 1. Aufgabe
*Gegeben sei die Zahlenfolge*

$$
\left(0, \frac{1}{2}, \frac{3}{4}, \frac{9}{10}, \ldots\right)
$$

**(a)**
*Überprüfen Sie, ob durch*

$$
a_n=\frac{3 n^2-3}{2 n^2+4 n+2}, n \in \mathbb{N}
$$

*das allgemeine Glied der Folge dargestellt werden kann.*

*Hinweis: Berechnen Sie $a_n$ für $n=1,2,3,4$ und vergleichen Sie Ihre Ergebnisse mit der angegebenen Zahlenfolge.*


$$
a_n=\frac{3 n^2-3}{2 n^2+4 n+2}, n \in \mathbb{N}
$$

Berechnung der ersten vier Folgeglieder ergibt

$$
\begin{aligned}
& a_1=\frac{3 \cdot 1^2-3}{2 \cdot 1^2+4 \cdot 1+2}=\frac{0}{8}=0 \\
& a_2=\frac{3 \cdot 2^2-3}{2 \cdot 2^2+4 \cdot 2+2}=\frac{12-3}{8+8+2}=\frac{9}{18}=\frac{1}{2} \\
& a_3=\frac{3 \cdot 3^2-3}{2 \cdot 3^2+4 \cdot 3+2}=\frac{3 \cdot 9-3}{2 \cdot 9+12+2}=\frac{24}{32}=\frac{3}{4} \\
& a_4=\frac{3 \cdot 4^2-3}{2 \cdot 4^2 + 4 \cdot 4 + 2}=\frac{3 \cdot 16-3}{2 \cdot 16+16+2}=\frac{48-3}{32 + 18}=\frac{45}{50}=\frac{9}{10}
\end{aligned}
$$

Diese Lösungen gleichen der Zahlenfolge

$$
\left(0, \frac{1}{2}, \frac{3}{4}, \frac{9}{10}, \ldots\right)
$$

**(b)**
*Berechnen Sie den Grenzwert $\displaystyle \lim _{n \rightarrow \infty} a_n$.*


$$
\lim_{ n \to \infty } a_{n} = \lim_{ n \to \infty } \frac{3n^{2} - 3}{2n^{2} + 4n + 2} = \lim_{ n \to \infty } \frac{n^{2}\left( 3 - \frac{3}{n^{2}} \right)}{n^{2}\left( 2 + \frac{4}{n} + \frac{2}{n^{2}} \right)} = \lim_{ n \to \infty } \frac{3 - \frac{3}{n^{2}}}{2 + \frac{4}{n} + \frac{2}{n^{2}}} \stackrel{n \rightarrow \infty}{\longrightarrow} \frac{3 - 0}{2 + 0 + 0} = \frac{3}{2}
$$

Der Grenzwert der Folge $a_{n}$ beträgt somit $\frac{3}{2} = 1,5$.

**(c)**
*Die Folge $\left(a_n\right)$ ist...*

- [x] konvergent
- [ ] divergent
- [ ] bestimmt divergent
- [x] beschränkt
- [x] monoton

*Kreuzen Sie Zutreffendes an. Sie müssen keine Begründung angeben.*

##### 2. Aufgabe 

**Teil a)**

**(i)**
*Berechnen Sie den Grenzwert der Folge*

$$
a_n=\frac{3 n^2-n}{n^2+2}
$$

$$
\lim_{ n \to \infty } a_{n} = \lim_{ n \to \infty } \frac{3n^{2} - n}{n^{2} + 2} = \lim_{ n \to \infty } \frac{n^{2}\left( 3 - \frac{1}{n} \right)}{n^{2}\left( 1 + \frac{2}{n^{2}} \right)} = \lim_{ n \to \infty } \frac{3 - \frac{1}{n}}{1 + \frac{2}{n^{2}}} \stackrel{n \rightarrow \infty}{\longrightarrow} \frac{3 - 0}{1 + 0} = 3
$$

Der Grenzwert der Folge $a_{n}$ beträgt somit 3.

**(ii)**
*Betrachten Sie die Reihe*

$$
\sum_{j=3}^{\infty} a_j=\sum_{j=3}^{\infty} \frac{3 j^2-j}{j^2+2} .
$$

*Ist die Reihe konvergent? Begründen Sie Ihre Antwort.*

Um auf Konvergenz zu prüfen, wird in diesem Fall das Quotientenkriterium angewandt.
Damit die Reihe konvergent ist, muss die Folge $a_{j}$

$$
\lim _{j \rightarrow \infty}\left|\frac{a_{j+1}}{a_j}\right|=q<1,
$$

erfüllen. Also:

$$
\begin{equation}
\begin{aligned} \displaystyle
& \lim _{j \rightarrow \infty}\left|\frac{a_{j+1}}{a_j}\right| = \lim_{ j \to \infty } \frac{3(j+1)^{2} - (j+1)}{j^{2}+2} \\
& = \lim_{ j \to \infty } \frac{3j^{2} + 6j + 3 - j - 1}{j^{2} + 2} \\
& = \lim_{ j \to \infty } \frac{3j^{2} + 5j + 2}{j^{2} + 2} \\
& = \lim_{ j \to \infty } \frac{j^{2}\left( 3 + \frac{5}{j} + \frac{2}{j^{2}} \right)}{j^{2}\left( 1 + \frac{2}{j^{2}} \right)} \\
& = \lim_{ j \to \infty } \frac{3 + \frac{5}{j} + \frac{2}{j^{2}}}{1 + \frac{2}{j^{2}}} \stackrel{j \rightarrow \infty}{\longrightarrow} \frac{3 + 0 + 0}{1 + 0} = 3 = q > 1
\end{aligned}
\end{equation}
$$

Aufgrund dessen, dass $q > 1$, ist das Quotientenkriterium nicht erfüllt, somit divergiert die Reihe $\displaystyle \sum_{j=3}^{\infty} a_j$.


**Teil b)**
*Beweisen Sie mit dem Quotientenkriterium, dass die unendliche Reihe*

$$
\sum_{k=1}^{\infty} \frac{k}{2^k}=\lim _{n \rightarrow \infty} \sum_{k=1}^n \frac{k}{2^k}
$$

*konvergent ist.*

Um auf Konvergenz zu prüfen, wird in diesem Fall das Quotientenkriterium angewandt.
Damit die Reihe konvergent ist, muss die Folge $a_{k}$

$$
\lim_{k \rightarrow \infty}\left|\frac{a_{k+1}}{a_k}\right|=q<1,
$$

erfüllen. Also

$$
\begin{equation}
\begin{aligned} \displaystyle
& \lim_{k \rightarrow \infty}\left|\frac{a_{k+1}}{a_k}\right|= \lim_{ k \to \infty } \frac{\frac{k+1}{2^{k+1}}}{\frac{k}{2^{k}}} = \lim_{ k \to \infty } \frac{k+1}{2^{k+1}} \cdot \frac{2^{k}}{k} = \lim_{ k \to \infty } \frac{2^{k}}{2^{k+1}} \cdot \frac{k+1}{k} = \lim_{ k \to \infty } \frac{k + 1}{2k} \\
& = \lim_{ k \to \infty } \frac{k\left( 1 + \frac{1}{k} \right)}{k(2)} \\
& = \lim_{ k \to \infty } \frac{1 + \frac{1}{k}}{2} \stackrel{k \rightarrow \infty}{\longrightarrow} \frac{1 + 0}{2} = \frac{1}{2} = q < 1
\end{aligned}
\end{equation}
$$

Aufgrund dessen, dass $q < 1$, ist das Quotientenkriterium erfüllt. Die Reihe $\displaystyle \sum_{k=1}^{\infty} \frac{k}{2^k}$ konvergiert also.