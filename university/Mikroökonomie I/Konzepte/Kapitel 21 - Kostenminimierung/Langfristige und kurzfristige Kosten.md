---
tags:
  - kosten
  - fristen
week: 2023-12-20
flashcard: false
publish: true
source: pp. 432 ff.
date created: Thursday, January 4th 2024, 7:13:04 pm
date modified: Friday, January 5th 2024, 4:07:37 pm
---
***
#### Kurzfristige und langfristige Kostenfunktionen

Es ist häufig wichtig, zwischen jenen minimalen Kosten zu unterscheiden, bei denen das Unternehmen alle seine Produktionsfaktoren anpassen kann, und jenen Minimalkosten, bei denen das Unternehmen nur einige seiner Faktoren anpassen kann.
$\longrightarrow$ siehe hierzu auch [[Kurze und lange Fristen]]

> [!definition|*] Kurzfristige Kostenfunktion
> Die **kurzfristige Kostenfunktion** ist durch die minimalen Kosten der Erzeugung eines vorgegebenen Outputniveaus definiert, wobei lediglich die [[Fixe und variable Faktoren#^cdde8e|variablen Produktionsfaktoren]] angepasst werden können.

^28a7a3

> [!definition|*] Langfristige Kostenfunktion
> Die  **langfristige Kostenfunktion** gibt demnach die minimalen Kosten der Produktion eines gegebenen Outputniveaus an, wenn *alle* Produktionsfaktoren angepasst werden können.

^f47239

***
#### Anwendung

- Nehmen wir an, dass der Faktor 2 kurzfristig auf ein Niveau $\bar{x}_{2}$ fixiert ist, langfristig hingegen frei variiert werden kann.

##### Kurzfristige Kostenfunktion

Die [[#^28a7a3|kurzfristige Kostenfunktion]] ist dann definiert durch

$$
c_{s}(y, \bar{x}_{2}) = \min_{x_{1}} w_{1}x_{1} + w_{2}\bar{x}_{2} \quad \ni \quad f(x_{1},\bar{x}_{2}) = y
$$

> [!caution] Achtung 
> Beachte, dass im Allgemeinen die Minimalkosten der Produktion von $y$ Outputeinheiten von der vorhandenen Menge und den Kosten des fixen Faktors abhängen werden.

- Für den Fall von zwei Faktoren ist dieses Minimierungsproblem leicht lösbar: Wir suchen einfach den kleinsten Wert von $x_{1}$, sodass $f(x_{1},\bar{x}_{2}) = y$ ist

oder unter Bezugnahme auf die [[#^eebf49|kurzfristigen Faktornachfragen]] (siehe unten):

$$
c_{s}(y,\bar{x}_{2}) = w_{1}x_{1}^{s}(w_{1},w_{2},\bar{x}_{2},y) + w_{2}\bar{x}_{2}
$$

Das besagt einfach, dass die Mininmalkosten der Produktion eines Outputs von $y$ jene Kosten sind, die sich bei der Verwendung der Kosten minimierenden Inputmengen ergeben.

##### Langfristige Kostenfunktion

Die [[#^f47239|langfristige Kostenfunktion]] ist in diesem Beispiel definiert durch

$$
c(y) = \min_{x_{1},x_{2}} w_{1}x_{1} + w_{2}x_{2} \quad \ni \quad f(x_{1},x_{2}) = y
$$

oder unter Bezugnahme auf die [[#^d9b34a|langfristigen Faktornachfragen]] (siehe unten):

$$
c(y) = w_{1}x_{1}(w_{1},w_{2},y) + w_{2}x_{2}(w_{1},w_{2},y)
$$

Hierbei können beide Faktoren verändert werden. Langfristige Kosten hängen nur vom Outputniveau, welches die Unternehmung erzeugen will, und den Faktorpreisen ab.

***
#### Faktornachfragen

> [!definition|*] Kurzfristige Faktornachfragen
> Die **kurzfristige Nachfragefunktion** nach Faktor 1 ist jene Menge des Faktors 1, welche die Kosten minimiert. Sie wird im Allgemeinen sowohl von den Faktorpreisen als auch den Niveaus der fixen Faktoren abhängen; wir schreiben die kurzfristigen Faktornachfragefunktionen daher als
> 
> $$
> x_{1} = x_{1}^{s}(w_{1},w_{2},\bar{x}_{2},y) \quad \ni \quad x_{2} = \bar{x}_{2}
> $$

^eebf49

- Diese Gleichungen besagen zum Beispiel einfach, dass bei einer kurzfristig fixen Gebäudegröße die Zahl der Arbeiter, die ein Unternehmen zu bestimmten Preisen und bei gewähltem Output einstellen will, typischerweise von der Größe der Gebäude abhängen wird

> [!definition|*] Langfristige Faktornachfragen
> Die **langfristige Faktornachfragefunktion** wird somit als
> 
> $$
> x_{1} = x_{1}(w_{1},w_{2},y)
> $$
> 
> bzw.
> 
> $$
> x_{2} = x_{2}(w_{1},w_{2},y)
> $$
> 
> geschrieben.

^d9b34a

