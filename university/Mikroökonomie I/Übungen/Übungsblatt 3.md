---
tags:
  - präferenzen
  - nutzen
  - übung
week: 2023-11-01
---
***

##### Aufgabe 1 | Von Präferenzen zur Nutzenfunktion

**a)**
*Wie lauten die Defintionen von Vollständigkeit und Transitivität?*

```ad-note
title: Definition
**Vollständigkeit:**
Für zwei beliebige Bündel $a$ und $b$ gilt entweder

$$
a \succeq b \quad \text{oder} \quad b \succeq a \quad \text{(oder beides)}
$$

```


```ad-note
title: Definition
**Transitivität:**
Für drei beliebige Bündel $a, b, c$ gilt:

$$
\text{ Wenn } a \succeq b \text{ und } b \succeq c, \text{ dann muss } a \succeq c 
$$

```

**b)**
*Angenommen auf dem Markt gibt es nun eine Banane und eine Kiwi. Können Sie anhand des Zettels entscheiden, welches Obst Sie für Konni auswählen sollten? Erfüllt diese Regel Vollständigkeit?*

$$
\begin{aligned}
& \text { Apfel } \succ \text { Banane } \\
& \text { Apfel } \succ \text { Kiwi }
\end{aligned}
$$

Nein, anhand des Zettels kann nicht entschieden werden, da er das Kriterium der Vollständigkeit nicht erfüllt. Das Kriterium der Vollständigkeit ist nicht erfüllt, da keine Präferenz zwischen Banane und Kiwi erkennbar ist.

**c)**
*Wider Erwarten gibt es nun alle drei Obstsorten auf dem Markt. Können Sie diesmal anhand des neuen Zettels entscheiden, welches Obst Sie mitbringen sollen? Erfüllt diese Regel Transitivität?*

$$
\begin{aligned}
\text { Apfel } & \succ \text { Banane } \\
\text { Banane } & \succ \text { Kiwi } \\
\text { Kiwi } & \succ \text { Apfel }
\end{aligned}
$$

Nein, da das Kriterium der Transitivität nicht erfüllt ist: Aus $\text { Apfel } \succ \text { Banane }$ und $\text { Banane } \succ \text { Kiwi }$ müsste $\text { Apfel }  \succ \text { Kiwi }$ folgen, allerdings ist laut Konnis Zettel $\text { Kiwi } \succ \text { Apfel }$.

**d)**
*Einen letzten Versuch unternimmt Konni um Ihnen einen hilfreichen Zettel mitgeben zu können. Um sicher zugehen, schauen Sie sich den Zettel genauer an bevor Sie auf den Markt (auf dem nun potentiell sogar vier Obstsorten angeboten werden!) gehen. Handelt es sich hierbei um eine Präferenzrelation?*

$$
\begin{aligned}
\text { Banane } & \succ \text { Apfel } \\
\text { Banane } & \succ \text { Birne } \\
\text { Banane } & \succ \text { Kiwi } \\
\text { Apfel } & \sim \text { Birne } \\
\text { Apfel } & \succ \text { Kiwi } \\
\text { Birne } & \succ \text { Kiwi }
\end{aligned}
$$

Hierbei handelt es sich um eine Präferenzrelation, da jedes mögliche Verhältnis beachtet wurde. Auch ist diese Transitiv, da keine Widersprüche entstehen.

**e)**
*Betrachten Sie erneut Regel 3. Können Sie eine Funktion finden, die jedem Element aus X einen Zahlenwert zuordnet, sodass ein höherer Funktionswert bedeutet, dass Konni die Frucht bevorzugt? Wie viele mögliche Funktionen gibt es?*

Ja, zum Beispiel:

$$
\begin{aligned}
u(apfel) = 5 \\
u(Birne) = 5 \\
u(Banane) = 6 \\
u(Kiwi) = 4
\end{aligned}
$$

Es bestehen unendlich viele Mögliche Funktionen, da $f(x) = k \cdot u(x)$. Diese sind allerdings nur ordinal.

##### Aufgabe 2 | Von Nutzenfunktionen zu Indifferenzkurven
*$x_{i j}$ sei die Menge von Gut $\mathrm{j}$ in einem Konsumbündel i. Betrachten Sie eine Relation, die alle möglichen Konsumbündel wie folgt ordnet: $\left(x_{A 1} ; x_{A 2}\right) \succsim\left(x_{B 1} ; x_{B 2}\right)$ genau dann, wenn $x_{A 1}^2 x_{A 2} \geq x_{B 1}^2 x_{B 2}$*

**a)**
*Zeigen Sie, dass es sich bei $x_{ij}$ um eine Präferenzrelation handelt, dass sie also vollständig und transitiv ist.*

$x_{ij}$ ist vollständig, da $x^{2}_{A1}x_{A2} \geq x^{2}_{B1}x_{B2}$, und transitiv, da $\left(x_{A 1} ; x_{A 2}\right) \succsim\left(x_{B 1} ; x_{B 2}\right)$.

**b)**
*Nennen Sie ein Beispiel für eine Nutzenfunktion, die diese Präferenzrelation beschreibt.*

$$
U(x_{1},x_{2}) = x_{1}^2x_{2}
$$

**c)**
*Gegeben sei ein Nutzenwert $\bar{u} = 9$. Zeichnen Sie für diesen Nutzenwert die entsprechende Indifferenzkurve in ein $x_{1}−x_{2}$ Diagramm, die sich aus der von Ihnen gewählten Nutzenfunktion ergibt.*

![[Pasted image 20231112203600.png|center|400]]

**d)**
*Berechnen sie die Grenzrate der Substitution. Was sagt diese aus?*

Die Grenzrate der Substitution ([[university/Mikroökonomie I/Konzepte/Kapitel 3 - Präferenzen/Grenzrate der Substitution|MRS]], von englisch "marginal rate of substitution") gibt Antwort auf die Frage: Wieviel von Gut 2 ist der Konsument bereit, für eine zusätzliche (marginale) Einheit von Gut 1 höchstens, d.h. bei gleichbleibendem Nutzen, aufzugeben? Die [[university/Mikroökonomie I/Konzepte/Kapitel 3 - Präferenzen/Grenzrate der Substitution|MRS]] ist somit die negative Steigung der Indifferenzkurve. In unserem speziellen Beispiel ist die [[university/Mikroökonomie I/Konzepte/Kapitel 3 - Präferenzen/Grenzrate der Substitution|MRS]] also

$$
M R S=\frac{\frac{\partial u}{\partial x_1}}{\frac{\partial u}{\partial x_2}}=\frac{2 x_1 x_2}{x_1^2}=\frac{2 x_2}{x_1}
$$

Die Grenzrate der Substitution ist also nicht konstant, sondern hängt vom Güterbündel ab, von dem man ausgeht: je mehr ein Konsument von Gut 1 bereits konsumiert, desto weniger wird ein solcher Konsument von Gut 2 für (noch) mehr von Gut 1 aufzugeben bereit sein.
Umgekehrt wird er umso mehr von Gut 1 im Austausch für Gut 2 aufgeben. Dies ist ein klassischer Fall von abnehmender Grenzrate der Substitution, wo der Konsument Mischungen (ausgewogene Bündel) bevorzugt.