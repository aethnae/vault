---
tags:
  - funktionen
week: 2023-12-05
flashcard: false
publish: true
---
***

> [!def] Logistische Funktionen 
> Eine Funktion $f$ mit
> 
> $$
> f(x) = \frac{k}{1 + e^{ a - bx }}
> $$
> 
> mit Parametern $a, b, k > 0$ heißt **logistische Funktion**

**Eigenschaften:**
- Es gilt $0 < f(x) < k$ sowie ${} \displaystyle \lim_{ x \to - \infty } f(x) = 0 {}$ und $\displaystyle \lim_{ x \to \infty } f(x) = k$
- $f$ ist streng monton wachsend, d.h. $f'(x) > 0 \text{ für alle } x > 0$
- $f$ hat genau einen Wendepunkt $P = \left( \frac{a}{b}, \frac{k}{2} \right)$

![[Pasted image 20231210011805.png|300]]
