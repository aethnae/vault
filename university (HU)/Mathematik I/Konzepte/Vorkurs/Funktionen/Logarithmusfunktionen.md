---
tags:
  - funktionen
week: 
flashcard: true
---
***

> [!def] Natürliche Logarithmusfunktionen
> Die reellwertige Funktion $f:(0, \infty) \rightarrow \mathbb{R}$ definiert durch
> $$
> x \mapsto \ln (x)=\log _e(x)
> $$
> mit $a>0$ heißt natürliche Logarithmusfunktion.

**Eigenschaften:**
- $\ln (1)=0$
- $\ln (x)<0$ für $x<1, \ln (x)>0$ für $x>1$
- $\lim _{x \rightarrow 0} \ln (x)=-\infty$
- $\ln (x)$ ist nicht definiert für $x \leq 0$ !
- Für a $>0$ gilt $\log _a(x)=\frac{1}{\ln (a)} \cdot \ln (x)$
$\Rightarrow \log _a(x)$ ist vertikal gestreckte/gestauchte Variante von $\ln (x)$

#### Logarithmus und Wurzel als Umkehrfunktion

- Die Wurzelfunktion $\sqrt[a]{\cdot}:[0, \infty] \rightarrow \mathbb{R}$ ist die Umkehrfunktion des Polynoms

$$
f:[0, \infty] \rightarrow \mathbb{R}, f(x)=x^a
$$

- Es gilt für $a>0$ und $x \geq 0$, dass

$$
\sqrt[a]{x^a}=x=(\sqrt[a]{x})^a
$$

- Die natürliche Logarithmusfunktion $\ln: (0, \infty) \rightarrow \mathbb{R}$ ist die Umkehrfunktion der [[university (HU)/Mathematik I/Konzepte/Vorkurs/Funktionen/Exponentialfunktionen|Exponentialfunktion]] $\exp : \mathbb{R} \rightarrow(0, \infty)$
- Es gilt

$$
\exp (\ln (x))=x=\ln (\exp (x))
$$
