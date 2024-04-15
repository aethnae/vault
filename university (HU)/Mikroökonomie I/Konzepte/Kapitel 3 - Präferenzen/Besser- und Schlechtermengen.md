---
source: 
publish: true
page: 
tags:
  - präferenzen
week: 2023-10-25
flashcard: true
date created: Wednesday, November 8th 2023, 4:48:11 pm
date modified: Wednesday, January 3rd 2024, 2:24:34 pm
---
***

> [!important] Definition
> Definiere für $x \in X$ "Bessermenge" $A(x)=\{y \in X \mid y \succeq x\}$ und "Schlechtermenge"
> $D(x)=\{y \in X \mid x \succeq y\}$.
> $(\mathrm{NB}: I(x)=A(x) \cap D(x)$.

![[Pasted image 20231108165101.png|center|400]]

**Eigenschaften:**
- Stetigkeit von $\succeq$ : Für jedes $x \in X$ sind $A(x)$ und $D(x)$ abgeschlossene Mengen; d.h., sie enthalten ihre Grenzen.
- Monotonie von $\succeq$ : Aus $x \geq y$ folgt $x \succeq y$, und falls außerdem noch $x \neq y$ dann $x \succ y$. $(x \geq y$ heißt: Ungleichung komponentenweise erfüllt; z.B. $(3,5) \geq(2,5)$.)
- Kurz gesagt: "Mehr ist besser."

![[Pasted image 20231108165410.png|center|450]]

- Konvexität von $\succeq$ : Für jedes $x \in X$ ist $A(x)$ eine konvexe Menge; d.h., für alle $\alpha \in[0,1]$ folgt aus $y \in A(x)$ und $z \in A(x)$, dass $\alpha y+(1-\alpha) z \in A(x) .(\alpha y+(1-\alpha) z$ ist das Bündel, das sich aus der komponentenweisen Mischung ergibt; z.B. $0.5 \cdot(3,5)+0.5 \cdot(2,5)=(2.5,5))$
- Kurz gesagt: "Mischungen sind mindestens genauso gut."

![[Pasted image 20231108165509.png|center|450]]

- Jedes Bündel liegt auf (mindestens) einer Indifferenzkurve. (Vollständigkeit)
- Dasselbe Bündel kann nicht auf zwei verschiedenen Indifferenzkurven liegen; d.h., Indifferenzkurven kreuzen einander nicht. (Transitivität)
- Indifferenzkurve $I(x)$ ist die Grenze sowohl von $A(x)$ als auch $D(x)$, und stetig. (Stetigkeit)
- Indifferenzkurven, keine "dicken" Indifferenzmengen. (Monotonie)
- Höhere Indifferenzkurven sind besser. (Monotonie)
- Indifferenzkurven fallen. (Monotonie)
- Indifferenzkurven sind konvex. (Konvexität)