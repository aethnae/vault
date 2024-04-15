---
page: 
tags:
  - ableitungen
  - produktion
  - angebot
week: 2023-12-13
flashcard: false
publish: true
aliases:
  - MRTS
date created: Thursday, December 14th 2023, 8:08:24 pm
date modified: Wednesday, January 3rd 2024, 2:26:22 pm
---
***

*Angenommen man produziert in einem Punkt $x_{1},x_{2}$ und überlegt, vom Faktor 1 ein wenig aufzugeben und gerade ausreichend mehr vom Faktor 2 zu verwenden, um dieselbe Outputmenge $y$ zu erzeugen.
Wie viel mehr vom Faktor 2, $\Delta x_{2}$ benötigt man, wenn wir ein wenig vom Faktor 1, $\Delta x_{1}$, aufgeben?*

> [!abstract] Definition 
> Die Antwort für diese Frage gibt die (negative) Steigung der [[university (HU)/Mikroökonomie I/Konzepte/Kapitel 19 - Technologie/Produktionsfunktion|Isoquante]] für Outputmenge $y$ im Punkt $(x_{1},x_{2})$. Diese wird auch **Grenzrate der technischen Substitution (MRTS)** genannt, und berechnet sich durch
>
> $$
> MRTS_{1}(x_{1},x_{2}) = \frac{\frac{ \partial f(x_{1},x_{2}) }{ \partial x_{1} } }{\frac{ \partial f(x_{1},x_{2}) }{ \partial x_{2} } } = \frac{MP_{1}(x_{1},x_{2})}{MP_{2}(x_{1},x_{2})}
> $$

- Die MRTS misst das Austauschverhältnis zwischen zwei Inputs - Sie misst das Verhältnis, zu welchem die Unternehmung einen Input durch den anderen wird ersetzen müssen, um den Output konstant zu halten

#### Beispiel

Beispielsweise wird der Fall einer [[university (HU)/Mikroökonomie I/Konzepte/Kapitel 19 - Technologie/Produktionsfunktion#Cobb-Douglas|Cobb-Douglas-Produktionsfunktion]] betrachtet, welche durch $f(x_{1},x_{2}) = x_{1}^{a}x_{2}^{b}$ dargestellt wird.

Laut Definition gilt also

$$
\frac{\mathrm{MP}_{1}}{\mathrm{MP}_{2}} = \frac{\frac{ \partial f(x_{1},x_{2}) }{ \partial x_{1} } }{\frac{ \partial f(x_{1},x_{2}) }{ \partial x_{2} } } = \frac{ax_{1}^{a-1}x_{2}^{b}}{bx_{1}^{a}x_{2}^{b-1}} = \frac{a}{b} \cdot \frac{x_{2}}{x_{1}}
$$

