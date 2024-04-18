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

`\end{proof}`