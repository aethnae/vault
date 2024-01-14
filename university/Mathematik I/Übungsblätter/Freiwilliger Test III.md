---
tags:
  - übung
week: 2024-01-14
flashcard: false
publish: true
source: 
date created: Sunday, January 14th 2024, 9:39:39 pm
date modified: Sunday, January 14th 2024, 9:39:58 pm
---
***
##### 1. Aufgabe
*Gegeben sei die Funktion $f(x)=\ln \left(\frac{e^{2 x+3}}{\sqrt{x}}\right)$ für $x>0$.*
*Beweisen Sie die Gültigkeit der Beziehung*

$$
\frac{f^{\prime}(x)}{\sqrt{f^{\prime \prime}(x)}}=\frac{\sqrt{2}}{2} \cdot(4 x-1)
$$

*Hinweis: Nutzen Sie Logarithmengesetze und beachten Sie, dass $\sqrt{x}=x^{\frac{1}{2}}$.*

Zunächst werden die ersten beiden Ableitungen unter Anwendung der Logarithmengesetze gebildet:

$$
\begin{align}
f(x) & = \ln(e^{ 2x+3 } - \ln(\sqrt{ x }) = 2x+3 - \ln(\sqrt{ x }) \\
f'(x) & = 2 - \frac{1}{\sqrt{ x }} \cdot \frac{1}{2\sqrt{ x }} = 2 - \frac{1}{2x} \\
f''(x) & = -\frac{1}{2} \cdot (-x^{-2}) = \frac{1}{2x^{2}} \\
\end{align}
$$

Um die Beziehung aus der Aufgabenstellung zu beweisen, muss eingesetzt und umgeformt werden:

$$
\begin{align}
\frac{f'(x)}{\sqrt{ f''(x) }}  & = \frac{2 - \frac{1}{2x}}{\sqrt{ \frac{1}{2x^{2}} }} \\
 & = \frac{2}{\sqrt{ \frac{1}{2x^{2}} }} - \frac{(2x)^{-1}}{\sqrt{ \frac{1}{2x^{2}} }} \\
 & = \frac{2}{\frac{1}{\sqrt{ 2 }x}} - \frac{(2x)^{-1}}{\frac{1}{\sqrt{ 2 }x}} \\
 & = 2\sqrt{ 2 }x - \frac{1}{2x} \cdot \sqrt{ 2 }x \\
 & = 2\sqrt{ 2 }x - \frac{\sqrt{ 2 }}{2} \\
 & = \frac{4\sqrt{ 2 }x}{2} - \frac{\sqrt{ 2 }}{2} \\
 & = \frac{\sqrt{ 2 }}{2} \cdot (4x - 1)
\end{align}
$$

***
##### 2. Aufgabe
*Gegeben ist die Funktion $f(x)=\sqrt{1+x}$ mit $x \geq-1$.*

**(a)**
*Berechnen Sie das Taylorpolynom dritter Ordung $T_{3,0}(x)$ von $f$ für den Entwicklungspunkt $x_0=0$.*

**(b)**
*Berechnen Sie den folgenden Grenzwert mit der Regel von L'Hospital.*

$$
\lim _{x \rightarrow 0} \frac{2-\cos (x)-e^{2 x}+2 x}{\sin (x)+e^{-x}-1}
$$

**(a)**

Zunächst müssen die ersten drei Ableitungen von $f(x)$ gebildet werden:

$$
\begin{align}
f'(x) & = \frac{1}{2\sqrt{ 1+x }} \\
f''(x) & = \frac{1}{2} \cdot \left( -\frac{1}{2} (1+x)^{-3/2} \right) = \frac{1}{4\sqrt{ (1+x)^{3} }} \\
f'''(x) & = -\frac{1}{4} \cdot \left( -\frac{3}{2}(1+x)^{-5/2} \right) = \frac{3}{8} \cdot \frac{1}{\sqrt{ (1+x)^{5} }} = \frac{3}{8\sqrt{ (1+x)^{5} }}
\end{align}
$$

Damit kann nun das Taylorpolynom dritter Ordnung gebildet werden:

$$
\begin{align}
T_{3,0} & = \sum_{k = 0}^{3} \frac{f^{(k)}(0)}{k!} \cdot x^{k} \\
 & = 1 + 0,5x + \frac{0,25}{2} \cdot x^{2} + \frac{\frac{3}{8}}{6} \cdot x^{3} \\
 & = \frac{1}{16}x^{3}+\frac{1}{8}x^{2}+\frac{1}{2}x+\frac{1}{2}
\end{align}
$$

**(b)**

$$
\begin{align}
& \lim_{ x \to 0 }  \frac{2-\cos(x)-e^{ 2x }+2x}{\sin(x) + e^{ -x } - 1} \\
 & = \lim_{ x \to 0 } \frac{\sin(x) -2e^{ 2x }+ 2}{\cos(x) -e^{ -x }} \\
 & = \lim_{ x \to 0 } \frac{\cos(x) -4e^{ 2x }}{-\sin(x) + e^{ -x }} \stackrel{x \rightarrow 0}{\longrightarrow} \frac{1 - 4 \cdot e^{ 0 }}{0 + e^{ 0 }} = -3
\end{align}
$$
