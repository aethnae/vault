---
tags:
  - nachfrage
  - funktionen
week: 2023-11-08
flashcard: false
publish: true
---
***

> [!important] Definition
> Jene Funktion, welche die [[Optimale Entscheidung|optimale Wahl]] - die **nachgefragten Mengen** - zu den verschiedenen Werten von Preisen und Einkommen in Beziehung setzt, wird **Nachfragefunktion** genannt.

***
#### Beispiele für konkrete Nachfragefunktionen
##### Perfekte Substitute
Für [[Indifferenzkurven#Perfekte Substitute|perfekte Substitute]] gibt es immer drei Möglichkeiten: Wenn $p_2>p_1$ dann ist die Steigung der Budgetgeraden flacher als die Steigung der Indifferenzkurven. Im Optimum gibt die Konsumentin ihr ganzes Geld für Gut 1 aus. Wenn $p_1>p_2$ dann kauft die Konsumentin nur Gut 2. Wenn schließlich $p_1=p_2$, dann gibt es einen großen Bereich optimaler Wahlmōglichkeiten - in diesem Fall ist jede Mengenkombination der beiden Guter optimal, welche die Budgetbeschrânkung erfüllt. Die Nachfragefunktion für Gut 1 lautet daher

$$
x_1= \begin{cases}m / p_1 & \text { wenn } p_1<p_2 ; \\ \text { jede Zahl zwischen } 0 \text { und } m / p_1 & \text { wenn } p_1=p_1 ; \\ 0 & \text { wenn } p_1>p_2 .\end{cases}
$$

Entsprechen diese Ergebnisse gesundem Menschenverstand? Sie besagen lediglich, dass bei perfekten Substituten die Konsumentin das billigere Gut kaufen wird, Wenn beide Güter denselben Preis haben, ist es der Konsumentin egal, welches sie kauft.

##### Perfekte Komplemente
Im Falle [[Indifferenzkurven#Perfekte Komplemente|perfekter Komplemente]] liegt die optimale Entscheidung immer auf der Diagonale, da die Konsumentin von beiden Gütern immer die selbe Menge kauft.

Lösen wir das Beispiel algebraisch. Wir wissen, dass diese Konsumentin unabhängig von den Preisen von beiden Gütern immer dieselbe Menge kauft. Wir wollen diese Menge mit $x$ bezeichnen. Die Lösung muss der [[Budgetbeschränkung]] genügen

$$
p_1 x+p_2 x=m
$$

Auflösung nach $x$ ergibt als optimale Mengen der Güter 1 und 2:

$$
x_1=x_2=x=\frac{m}{p_1+p_2} .
$$

Die Nachfragefunktion entspricht vollständig der Intuition. Da die beiden Guter immer gemeinsam konsumiert werden, ist das genau so, als würde die Konsumentin ihr ganzes Geld für ein einziges Gut ausgeben, das einen Preis von $p_1+p_2$ hat.

##### Neutrale Güter und Ungüter
Im Fall eines Gutes, welchem die Konsumentin gegenüber neutral ist, wendet sie ihr ganzes Geld für den Konsum jenes Gutes auf, das sie mag, und kauft überhaupt nicht vom neutralen Gut. Dasselbe geschieht, wenn ein Gut ein „Ungut“ ist. Wenn als Ware 1 ein Gut und Ware 2 ein "Ungut" ist, dann werden die Nachfragefunktionen
$$
\begin{aligned}
& x_1=\frac{m}{P_1} \\
& x_2=0
\end{aligned}
$$
lauten.

##### Unteilbare Güter
Angenommen Gut 1 ist ein unteilbares Gut, das nur in ganzahligen Einheiten verfügbar ist, während Gut 2 das Geld ist, das für alles Übrige ausgegeben wird. Wenn die Konsumentin
1, 2, 3, ... Einheiten des Gutes 1 wählt, wählt sie implizit die Konsumbündel $\left(1, m-p_1\right),\left(2, m-2 p_1\right),\left(3, m-3 p_1\right)$ usw. Wir können einfach den Nutzen dieser Bündel miteinander vergleichen und herausfinden, welches den höchsten Nutzen stiftet.

##### Konkave Präferenzen
Für diese Präferenzen ist die optimale Entscheidung stets eine Randlösung, wie z. B. das Bündel Z. Überlege, was [[Konvexität|nicht-konvexe]] Präferenzen bedeuten. Wenn man sein Geld zum Kauf von Eiscreme und Oliven ausgeben kann, man diese beiden Güter jedoch nicht gemeinsam konsumieren will, dann wird man das ganze Geld entweder für das eine oder das andere verwenden.

##### Cobb-Douglas-Präferenzen
Angenommen die [[Nutzenfunktionen|Nutzenfunktion]] hat die Cobb-Douglas-Form $u(x_{1}, x_{2}) = x_{1}^{c}x_{2}^{d}$. Die Lösung lautet
$$
\begin{aligned}
& x_1=\frac{c}{c+d} \frac{m}{p_1} \\
& x_2=\frac{d}{c+d} \frac{m}{p_2}
\end{aligned}
$$

Cobb-Douglas-Präferenzen haben eine bemerkenswerte Eigenschaft. Betrachte den Einkommensanteil, den eine Cobb-Douglas-Konsumentin für Gut 1 ausgibt. Wenn sie $x_{1}$ Einheiten des Gutes 1 konsumiert, kostet sie das $p_1 x_1$, was einen Anteil von $\frac{p_{1} x_{1}}{m}$ ihres Gesamteinkommens darstellt. Wenn wir für $x_{1}$ die Nachfragefunktion einsetzen, erhalten wir
$$
\frac{p_1 x_1}{m}=\frac{p_1}{m} \frac{c}{c + d} \frac{m}{p_{1}}=\frac{c}{c+d}
$$

Analog dazu ist der Einkommensanteil, den die Konsumentin für Gut 2 ausgibt, $\frac{d}{c + d}$.

Die Cobb-Douglas-Konsumentin gibt daher für jedes Gut immer einen konstanten Anteil ihres Einkommens aus. Die Höhe dieser Anteile wird durch die Exponenten der Cobb-Douglas-Funktion bestimmt.

Deswegen ist es oft zweckmäßig, eine Darstellung der Cobb-Douglas-Nutzenfunktion zu wählen, bei der sich die Exponenten zu 1 addieren. Wenn $u\left(x_1, x_2\right)=x_{1}^{a} x_{2}^{1 - a}$, dann können wir $a$ unmittelbar als den für Gut 1 ausgegebenen Einkommensanteil interpretieren.