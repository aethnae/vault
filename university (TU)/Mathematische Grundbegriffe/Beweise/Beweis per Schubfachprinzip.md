---
tags:
  - Beweise
  - Logik
flashcard: false
source: 
date created: 
types: 
examples: 
constructions:
  - "[[Beweis per Kontradiktion]]"
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Schubfachprinzip
> Das *Schubfachprinzip* basiert auf folgender elementarer Beobachtung: Seien $m,n \in \mathbb{N}$ gegeben. Werden $mn + 1$ Kugeln auf $n$ Schubfächer verteilt, so gibt es ein Schubfach, in dem sich mindestens $m + 1$ Kugeln befinden.
> Ein Alltagsbeispiel hierfür ist: "*Für jede Gruppe von 25 Menschen gibt es einen Monat, in dem mindestens drei dieser Menschen Geburtstag haben.*"

***
#### Eigenschaften

- Das Beweisprinzip der [[Beweis per Kontradiktion|Kontradiktion]] basiert teilweise auf dem Schubfachprinzip

***
#### Beispiele

> [!exm|*] Beispielbeweis mithilfe des Schubfachprinzips 
> Ein gleichseitiges Dreieck $\Delta A$ kann nicht in zwei (kleinere) gleichseitige Dreiecke $\Delta A_{1}$ und $\Delta A_{2}$ zerlegt werden.
> 
> `\begin{proof}`
> Sei $\Delta A$ ein gleichseitiges Dreieck mit Seitenlänge $a > 0$. Angenommen es existiert eine Zerlegung von $\Delta A$ in zwei gleichseitige Dreiecke $\Delta A_{1}$ und $\Delta A_{2}$ mit den Seitenlängen $a_{1} > 0$ und $a_{2} > 0$. Insbesondere gilt dann $a > a_{1}$ und $a > a_{2}$. Nach dem Schubfachprinzip muss entweder $\Delta A_{1}$ oder $\Delta A_{2}$ mindestens zwei der drei Eckpunkte von $\Delta A$ enthalten. Diese Eckpunkte haben aber den Abstand $a$. Dies ist ein Widerspruch zu $a > a_{1}$, bzw. $a > a_{2}$. Somit existieren $\Delta A_{1}$ und $\Delta A_{2}$ nicht.
> `\end{proof}`
