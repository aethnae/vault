---
tags:
  - gewinn
week: 2023-12-20
flashcard: false
publish: true
source: pp. 409 ff.
date created: Wednesday, January 3rd 2024, 3:00:44 pm
date modified: Wednesday, January 3rd 2024, 3:01:01 pm
---
***

Da ein Problem innerhalb einer kurzen Frist betrachtet wird, muss Input 2 auf einem bestimmten Niveau $\bar{x}_{2}$ fixiert werden. Die Unternehmung habe die Produktionsfunktion $f(x_{1},x_{2})$, $p$ sei der Preis des Outputs, $w_{1}$ und $w_{2}$ die Preise der beiden Inputs. Das **Gewinnmaximierungsproblem** kann dann als

$$
\max_{x_{1}} pf(x_{1}, \bar{x}_{2}) - w_{1}x_{1}-w_{2}\bar{x}_{2}
$$

angeschrieben werden.
Wenn $x_{1}^{*}$ die Gewinn maximierende Menge des Faktors 1 ist, dann muss

$$
pMP_{1}(x_{1}^{*},\bar{x}_{2})=w_{1}
$$

bzw. unter Verwendung der Differentialrechnung

$$
p\frac{ \partial f(x_{1}^{*},\bar{x}_{2}) }{ \partial x_{1} } -w_{1}=0
$$

gelten.

> [!axiom|*] Kurzfristige Gewinnmaximierung
> **Der Wert des Grenzprodukts eines Faktors sollte gleich seinem Preis sein.**

> [!remark|*]- Herleitung
> Um diese Regel zu verstehen, braucht man sich nur zu überlegen, ein wenig mehr vom Faktor 1 einzusetzen. Wenn man ein wenig davon hinzufügt, $\Delta x_{1}$, erzeugt man $\Delta y = MP_{1}\Delta x_{1}$ zusätzlichen Output, der $pMP_{1}\Delta x_{1}$ wert ist. Die Erzeugung dieses zusätzlichen Outputs kostet jedoch $w_{1}\Delta x_{1}$.
> 
> Wenn der Wert des [[university (HU)/Mikroökonomie I/Konzepte/Kapitel 19 - Technologie/Grenzprodukt|Grenzprodukts]] dessen Kosten übersteigt, dann können die Gewinne durch **Erhöhung** des Inputs 1 gesteigert werden. Ist der Wert des Grenzprodukts jedoch geringer als dessen Kosten, so können die Gewinne durch **Senkung** der Menge des Inputs 1 gesteigert werden.
> 
> Wenn die Gewinne der Unternehmung so groß wie möglich sind, dann sollten sie nicht steigen, wenn wir den Input 1 erhöhen oder senken. Das bedeutet, dass bei der Gewinn maximierenden Entscheidung bezüglich Inputs und Outputs der Wert des Grenzprodukts $pMP_{1}(x_{1}^{*},\bar{x}_{2})$, gleich dem Faktorpreis $w_{1}$ sein sollte.

Grafisch kann dieser Satz ebenso hergeleitet werden, indem Gewinne durch

$$
\pi = pyn-w_{1}x_{1} - w_{2}\bar{x}_{2}
$$

angeschrieben werden. Diese Gleichung kann nach $y$ gelöst werden, um den Output als eine Funktion von $x_{1}$ auszudrücken:

> [!theorem|*] Isogewinnlinien
> $$
> y = \frac{\pi}{p} + \frac{w_{2}}{p}\bar{x}_{2} + \frac{w_{1}}{p}x_{1}
> $$

^2ba772

Diese Gleichung beschreibt die **Isogewinnlinien**, also alle Kombinationen der Inputs und des Outputs, die ein konstantes Gewinnniveau $\pi$ ergeben. Wenn $\pi$ variiert, erhalten wir eine Schar paralleler Geraden, mit einer Steigung von jeweils $\frac{w_{1}}{p}$ und einem (vertikalen) Ordinatenabschnitt von
$\frac{\pi}{p} + \frac{w_{2}\bar{x}_{2}}{p}$, der den Gewinn zuzüglich der fixen Kosten des Unternehmens misst.

Das Gewinnmaximierungsproblem besteht darin, jenen Punkt auf der Produktionsfunktion zu finden, der auf der höchsten Isogewinnlinie liegt. Wie üblich wird er durch eine [[Tangentialbedingung]] charakterisiert: Die Steigung der Produktionsfunktion (das [[university (HU)/Mikroökonomie I/Konzepte/Kapitel 19 - Technologie/Grenzprodukt|Grenzprodukt]]) sollte gleich der Steigung der Isogewinnlinie ($\frac{w_{1}}{p}$) sein, also gilt

$$
\begin{align}
 MP_{1} &  = \frac{w_{1}}{p} \\
 pMP_{1} &  = w_{1}
\end{align}
$$

***
#### Komparative Statik

Ändert man z.B. den Preis $w_{1}$ des Faktors 1, ist mit Bezug auf die [[#^2ba772|Isogewinnlinien]] zu erkennen, dass die Steigung mit steigendendem Preis auch steigt, und mit fallendem Preis genauso fällt. Steigt oder fällt die Steigung der Isogewinnlinien, verschiebt sich der Berührungspunkt mit der [[university (HU)/Mikroökonomie I/Konzepte/Kapitel 19 - Technologie/Produktionsfunktion|Produktionsfunktion]] nach links bzw. rechts.
Das bedeutet einfach, dass bei einem Ansteigen bzw. Fallen des Preises des Faktors 1 die Nachfrage nach Faktor 1 sinken bzw. steigen muss.

Das selbe gilt in umgekehrter Richtung für steigende bzw. fallende Outputpreise $p$.

Schließlich können wir noch fragen, was geschieht, wenn sich der Preis des Faktors 2 ändert. Da wir derzeit die kurze Periode analysieren, wird eine Änderung des Preises des Faktors 2 die Entscheidung der Unternehmung hinsichtlich des Faktors 2 nicht verändern - kurzfristig ist das Niveau des Faktors 2 bei $\bar{x}_2$ fixiert. Eine Veränderung des Preises des Faktors 2 hat keine Auswirkung auf die Steigung der Isogewinnlinie. Weder die optimale Wahl des Faktors 1 noch das Angebot des Outputs werden sich ändern. Lediglich die Gewinne der Unternehmung ändern sich.