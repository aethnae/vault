---
tags:
  - ableitungen
  - kosten
week: 2023-12-20
flashcard: false
publish: true
source: pp. 443 ff.
date created: Friday, January 5th 2024, 6:06:50 pm
date modified: Friday, January 5th 2024, 6:06:54 pm
---
***

> [!definition|*] Grenzkostenkurve
> Die **Grenzkostenkurve** misst die *Änderung* der Kosten für eine gegebene Änderung des Outputs. Das heißt, bei jedem gegebenen Outputniveau $y$ können wir fragen, wie sich die Kosten ändern werden, wenn wir den Output um eine gewisse Menge $\Delta y$ ändern:
> 
> $$
> \mathrm{MC}(y) = \frac{\Delta c(y)}{\Delta y} = \frac{c(y+\Delta y) - c(y)}{\Delta y}
> $$
> 
> Oder unter Verwendung der [[Durchschnittskosten|variablen Kostenfunktion]]:
> 
> $$
> \mathrm{MC}(y) = \frac{\Delta c_{v(y)}}{\Delta y} = \frac{c_{v}(y+\Delta y)-c_{v}(y)}{\Delta y}
> $$

***
#### Grafische Darstellung

Definitionsgemäß sind die [[Durchschnittskosten|variablen Kosten]] Null, wenn Null Outputeinheiten erzeugt werden. Daher gilt für die erste produzierte Outputeinheit

$$
\mathrm{MC}(1) = \frac{c_{v}(1)+F-c_{v}(0)-F}{1} = \frac{c_{v}(1)}{1} = \mathrm{AVC}(1)
$$

Die Grenzkosten für die erste kleine Outputmenge sind daher gleich den variablen Kosten für eine Einheit des Outputs.

- In Bereichen, in dem die *durchschnittlichen variablen Kosten* fallen, müssen die *Grenzkosten* kleiner sein als die durchschnittlichen variablen Kosten, denn ein Durchschnitt wird durch hinzuaddieren kleinerer Zahlen als der Durchschnitt nach unten gedrückt
- In Bereichen, in dem die *durchschnittlichen variablen Kosten* steigen, müssen die *Grenzkosten* größer sein als die durchschnittlichen variablen Kosten, denn ein Durchschnitt wird durch hinzuaddieren größerer Zahlen als der Durchschnitt nach oben gedrückt

Somit muss die Grenzkostenkurve links vom Minimum der Kurve der durchschnittlichen variablen Kosten unterhalb dieser Kurve liegen, und rechts davon oberhalb. Das impliziert, dass die Grenzkostenkurve die Kurve der durchschnittlichen variablen Kosten in ihrem Minimum schneidet.

- Genau die selben Überlegungen gelten auch für die Durchschnittskostenkurve $\longrightarrow$ auch diese wird durch die Grenzkostenkurve in ihrem Minimum geschnitten

Diese Überlegungen erlauben uns, die Grenzkostenkurve grafisch darzustellen:

![[Pasted image 20240105183729.png|center|600]]

***
#### Grenzkosten und variable Kosten

> [!note] Beziehung zwischen Grenz- und variablen Kosten 
> Es zeigt sich, dass die Fläche unterhalb des Graphen der Grenzkosten bis $y$ die variablen Kosten der Erzeugung von $y$ Outputeinheiten angibt.
> 
> Unter Anwendung der Infinitesimalrechnung ergibt sich:
> 
> $$
> c_{v}(y) = \int_{0}^{y} \frac{ \mathrm{d} c_{v}(x) }{ \mathrm{d} x } \, dx = c_{v}(y) - c_{v}(0) = c_{v}(y)
> $$

- Dies ist der Fall, da die Grenzkostenkurve die Produktion jeder zusätzlichen Outputeinheit misst. Wenn wir die Produktionskosten jeder Outputeinheit addieren, erhalten wir die gesamten Produktionskosten - mit Ausnahme der Fixkosten
