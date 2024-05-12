***
##### Aufgabe 0.1: Satz 0.3 - *De Morgan'sche Regeln*

Zeigen Sie die Aussagen 5) und 6) aus  dem Skript des Satzes 0.3.

a) $(\neg(A \vee B)) \Leftrightarrow ((\neg A) \wedge (\neg B))$
b) $(\neg (A \wedge B)) \Leftrightarrow ((\neg A)  \vee (\neg B))$

Der Beweis wird mithilfe einer Wahrheitstafel geführt. Seien $A, B$ Aussagen.

`\begin{proof}`
$$
\begin{array}{c|c|c|c|c|c}
A & B & \neg A & \neg B & \neg (A \vee B) & ((\neg A)\wedge (\neg B)) \\
\hline w & w & f & f & f & f \\
w & f & f & w & f & f \\
f & w & w & f & f & f \\
f & f & w & w & w & w
\end{array}
$$

Anhand der Wahrheitstafel lässt sich Aussage 5) beweisen. Um den Beweis für 6) zu führen, muss diese modifiziert werden:

$$
\begin{array}{c|c|c|c|c|c}
A & B & \neg A & \neg B & \neg (A \wedge B) & ((\neg A) \vee (\neg B)) \\
\hline w & w & f & f & f & f \\
w & f & f & w & w & w \\
f & w & w & f & w & w \\
f & f & w & w & w & w
\end{array}
$$

Somit ist auch 6) eindeutig bewiesen.
`\end{proof}`

***
##### Aufgabe 0.2: Satz 0.13 - *Absorptionsgesetze und De Morgan'sche Regeln*

Zeigen Sie die Aussagen 4) und 5) aus dem Skript des Satzes 0.13: Seien $A, B$ und $C$ Mengen. Dann gelte:

a) $A \cap (A \cup B) = A$,
b) $A \cup (A \cap B) = A$,
c) $A \setminus (B \cap C) = (A \setminus B) \cup (A \setminus C)$,
d) $A \setminus (B \cup C) = (A \setminus B) \cap (A \setminus C)$.

`\begin{proof}`
Für alle $x$ gilt somit, dass:

$$
\begin{align}
x \in A & \implies x \in A \wedge x \in (A \cup B) \\
 & \implies x \in A \wedge (x \in A \vee x \in B) \\
 & \implies x \in A
\end{align}
$$

Damit ist Aussage a) eindeutig bewiesen.

$$
\begin{align}
x \in A  & \implies x \in A \vee x \in (A \cap B) \\
 & \implies x \in A \vee (x \in A \wedge x \in B) \\
 & \implies \ldots 
\end{align}
$$

Bereits aus der ersten Aussage lässt sich der Beweis ableiten.

$$
\begin{align}
x \in A \setminus (B \cap C) & \implies x \in (A \setminus B) \vee x \in (A \setminus C) \\
 & \implies (x \in A \wedge x \notin B) \vee (x \in A \wedge x \notin C) \\
 & \implies x \in A \wedge (x \notin B \vee x \notin C) \\
 & \implies x \in A \wedge x \notin (B \cap C) \\
 & \implies x \in A \setminus (B \cap C) 
\end{align}
$$

Damit ist Aussage c) eindeutig bewiesen.

$$
\begin{align}
x \in A \setminus (B \cup C) & \implies x \in A \setminus B \wedge x \in A \setminus C \\
 & \implies (x \in A \wedge x \notin B) \wedge (x \in A \wedge x \notin C) \\
 & \implies x \in A \wedge (x \notin B \wedge x \notin C) \\
 & \implies x \in A \wedge x \notin (B \cup C) \\
 & \implies x \in A \setminus (B \cup C)
\end{align}
$$

Damit ist abschließend auch Aussage d) bewiesen.
`\end{proof}`

***
##### Aufgabe 0.3: Kubische Funktionen

Wir betrachten in dieser Aufgabe die Funktion $f: \mathbb{R} \mapsto \mathbb{R}, x \mapsto x^3$. Zeigen oder widerlegen Sie folgende Aussagen: Die Funktion

a) $f:[0, \infty) \mapsto \mathbb{R}$ ist bijektiv.
b) $f:(-\infty, 0] \mapsto[0, \infty)$ ist surjektiv.
c) $f:(-\infty, 0] \mapsto(-\infty, 0]$ ist nicht bijektiv.

**a)**

`\begin{proof}`
Um Bijektivität zu zeigen, müssen sowohl In-, als auch Surjektivität für die vorliegene Funktion gelten. Surjektivität liegt in negativen Funktionswerten bei dieser Funktion jedoch nicht vor, etwa für $f(x) = -1$.
`\end{proof}`

**b)**

`\begin{proof}`
Um Surjektivität zu zeigen, muss für alle $y \in B$ *mindestens* ein $x \in A$ vorliegen. In diesem spezifischen Fall ist jedoch $B = [0, \infty)$, und $A = (-\infty, 0]$. Somit existieren $y \in B$, wie zum Beispiel $y = 1$, denen kein $x \in A$ zugeordnet wird. Denn es gilt

$$
f(x) = x^{3} = 1 \Leftrightarrow x = 1 \implies x \notin A
$$

Damit ist $f:(-\infty, 0] \mapsto [0, \infty)$ **nicht** surjektiv.
`\end{proof}`

**c)**

`\begin{proof}`
Um die Behauptung zu widerlegen, muss Bijektivität nachgewiesen werden. Die passiert, indem für $f:(-\infty, 0] \mapsto (-\infty, o]$ Surjektivität *sowie* Injektivität nachgewiesen wird.

**Injektivität**:

Wir prüfen auf Injektivität, indem wir annehmen, dass ein Element aus der Zielmenge von **zwei** Werten $x, y \in A$ getroffen wird.

$$
f(x) = f(y) \implies x^{3} = y^{3} \implies x = y
$$

Somit gilt im Umkehrschluss auch ${} x \neq y \implies f(x) \neq f(y) {}$. Damit ist $f$ im gegebenen Intervall *injektiv*.

**Surjektivität**:

Wir prüfen auf Surjektivität, indem wir uns ein beliebiges $y = f(x)$ aus der Wertemenge heraussuchen, und eine allgemeine Gleichung für zugehörige Werte aus der Definitionsmenge aufstellen.

$$
y = x^{3} \implies \sqrt[3]{ y } = x
$$

Da $y \in (-\infty, 0]$, muss auch $\sqrt[3]{ y } \in (-\infty, 0]$ sein. Dies ist für $x \in A$ der Fall. Damit ist $f$ auch eine *surjektive* Funktion.

**Bijektivität**:

Da $f$ sowohl in-, als auch surjektiv ist, ist $f:(-\infty, 0] \mapsto (-\infty, 0]$ eine **bijektive** Funktion, und die Aussage **c)** ist widerlegt.
`\end{proof}`

***
##### Aufgabe 0.4: Relationen

Entscheiden Sie ob die nachstehenden Relationen auch Äquivalenzrelationen sind; falls ja, beweisen Sie dies.

- $R_1 = \{(a, b) \in \mathbb{N} \times \mathbb{N}: a<b\}$.
- $R_2=\left\{(A, B) \in\{\text {Personen auf der Erde}\}^2: A\right.$ ist mit $B$ befreundet $\}$
- $R_3=\{(a, b) \in \mathbb{N} \times \mathbb{N}:|a-b| \leq 2\}$.
- $R_4=\left\{(a, b) \in P \times P: a_1 b_2=a_2 b_1\right\}$, wobei $P=\{(z, n) \in \mathbb{Z} \times \mathbb{N}: n \neq 0\}$.

$R_{1}$ ist *keine* Äquivalenzrelation, da das Kriterium der Reflexivität nicht erfüllt ist.

`\begin{proof}`
$R_{1}$ ist irreflexiv, da $aR_{1}a \implies a < a \implies \unicode{10803}$
`\end{proof}`
<br> 

Auch $R_{2}$ ist keine Äquivalenzrelation, da nicht alle Kriterien dieser erfüllt sind.

`\begin{proof}`

- **Ungenau**, da $AR_{2}A$ meint, dass $A$ mit sich selbst befreundet ist?
- **Symmetrisch**, da "Freundschaft" beidseitig angenommen werden muss?
- $AR_{2}B \wedge BR_{2}C \not \Rightarrow AR_{2}C$, also auch **intransitiv**

und damit keine Äquivalenzrelation.
`\end{proof}`
<br>

$R_{3}$ erfüllt bis auf die fehlende Transitivität alle Bedingungen für eine Äquivalenzrelation:

`\begin{proof}`
- **Reflexiv**, da $aR_{3}a \implies \lvert a - a \rvert \leq 2 \implies 0 \leq 2$
- **Symmetrisch**, da $aR_{3}b \implies \lvert a - b \rvert \leq 2 \iff bR_{3}a \implies \lvert b - a \rvert \leq 2$, und somit $\lvert a - b \rvert \iff \lvert b - a \rvert$
- **Intransitiv**, etwa für $a = 2$, $b = 4$, $c = 6$
`\end{proof}`
<br> 

$R_{4}$ ist eine Äquivalenzrelation $\ldots$


