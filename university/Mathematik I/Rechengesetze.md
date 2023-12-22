***
#### Grundlegende Rechengesetze

> [!definition] Kommutativgesetz
> $$
> a + b = b + a \quad \quad a \cdot b = b \cdot a
> $$

> [!definition] Assoziativgesetz
> $$
> (a + b) + c = a + (b + c) \quad \quad a \cdot (b \cdot c) = (a \cdot b) \cdot c
> $$

> [!definition] Distributivgesetz
> $$
> (a + b) \cdot c = a \cdot c + b \cdot c \quad \quad a \cdot (b + c) = a \cdot b + a \cdot c
> $$

***
#### Binomische Formeln
*Spezialfall der Distributivgesetze*

> [!definition] Erste binomische Formel
> $$
> (a + b)^2 = a^2 + 2ab + b^2
> $$

> [!definition] Zweite binomische Formel
> $$
> (a - b)^2 = a^2 - 2ab + b^2
> $$

> [!definition] Dritte binomische Formel
> $$
> (a + b) \cdot (a - b) = a^2 - b^2
> $$

***
#### Potenzgesetze

> [!definition] Erstes Potenzgesetz
> $$
> a^r \cdot a^s = a^{r+s} \quad \quad a^r : a^s = a^{r - s}
> $$

> [!definition] Zweites Potenzgesetz
> $$
> (a^r)^s = a^{r \cdot s}
> $$

> [!definition] Drittes Potenzgesetz
> $$
> a^r \cdot b^r = (a \cdot b)^r
> $$

^096095

> [!lemma] Spezialfälle
> $$
> a^0 = 1 \quad \quad a^1 = a \quad \quad a^{-b} = \frac{1}{a^b} \quad \text{(für $a, b \neq 0$)}
> $$

***
#### Wurzelgesetze

> [!definition] Erstes Wurzelgesetz
> $$
> \sqrt[n]{a^m} = a^{\frac{m}{n}}
> $$

> [!definition] Zweites Wurzelgesetz
> $$
> \sqrt[c]{ \sqrt[b]{ a } } = \sqrt[c \cdot b]{ a }
> $$

> [!definition] Drittes Wurzelgesetz
> $$
> \sqrt[c]{ a } \cdot \sqrt[c]{ b } = \sqrt[c]{ a \cdot b }
> $$

***
#### Logarithmen
*siehe [[Logarithmen#^3362bc]]*

> [!definition] Erstes Logarithmengesetz
> $$
> \log_{a}(b \cdot c) = \log_{a}(b) + \log_{a}(c)
> $$

> [!definition] Zweites Logarithmengesetz
> $$
> \log_{a}\left( \frac{b}{c} \right) = \log_{a}(b) - \log_{a}(c)
> $$

> [!definition] Drittes Logarithmengesetz
> $$
> \log_{a}(b^{c}) = c \cdot \log_{a}(b)
> $$

> [!definition] Viertes Logarithmengesetz
> $$
> \log_{a}(b) = \frac{\log_{c}(b)}{\log_{c}(a)}
> $$

> [!definition] Fünftes Logarithmengesetz
> $$
> \log_{a}(a^{x}) = x
> $$

- $e^x = b \leftrightarrow x = \ln(b)$
- $e^{\ln(b)} = b$
- $\ln(e^c) = c$

***
#### Ableitungen

> [!definition] Faktorregel
> $$
> (c \cdot u(x))' = c \cdot u'(x)
> $$

> [!definition] Summenregel
> $$
> (u(x) + v(x))' = u'(x) + v'(x)
> $$

> [!definition] Produktregel
> $$
> (u(x) \cdot v(x))' = u'(x) \cdot v(x) + u(x) \cdot v'(x)
> $$

> [!definition] Kettenregel
> $$
> (u(v(x)))' = u'(v(x)) \cdot v'(x)
> $$

> [!definition] Quotientenregel
> $$
> \left( \frac{u(x)}{v(x} \right)' = \frac{u'(x) \cdot v(x) - u(x) \cdot {v'(x)}}{(v(x))^2}
> $$

Die Quotientenregel folgt direkt aus Produkt- und Kettenregel, denn

![[Pasted image 20231105184313.png|400]]

**Besondere Ableitungen:**

| Funktion            | Ableitung                       |
| ------------------- | ------------------------------- |
| $f(x) = \sqrt{ x }$ | $f'(x) = \frac{1}{2\sqrt{ x }}$ |
| $f(x) = \cos(x)$    | $f'(x) = -\sin(x)$|  
| $f(x) = \sin(x)$    | $f'(x) = \cos(x)$|   
| $f(x) = \tan(x)$    | $f'(x) = \frac{1}{\cos^{2}(x)}$ |  
| $f(x) = e^x$        | $f'(x) = e^x$|   
| $f(x) = \ln(x)$     | $f'(x) = \frac{1}{x}$|    

***
#### Grenzwerte

> [!thm] Grenzwertrechenregeln
> Es sei
> $$
> \lim _{n \rightarrow \infty} a_n=a \in \mathbb{R} \quad \text { und } \quad \lim _{n \rightarrow \infty} b_n=b \in \mathbb{R} \quad \text { sowie } \quad c \in \mathbb{R} .
> $$
> Dann gelten folgende Rechenregeln.
> $$
> \begin{aligned}
> \lim_{n \rightarrow \infty}\left(a_n+c\right) & =\lim _{n \rightarrow \infty} a_n+c & & = a+c \\
> \lim _{n \rightarrow \infty}\left(c \cdot a_n\right) & =c \cdot \lim _{n \rightarrow \infty} a_n & & = c \cdot a \\
> \lim _{n \rightarrow \infty}\left(a_n+b_n\right) & =\lim _{n \rightarrow \infty} a_n+\lim _{n \rightarrow \infty} b_n & & = a+b \\
> \lim _{n \rightarrow \infty}\left(a_n \cdot b_n\right) & =\lim _{n \rightarrow \infty} a_n \cdot \lim _{n \rightarrow \infty} b_n & & = a \cdot b \\
> \lim _{n \rightarrow \infty} \frac{a_n}{b_n} & =\frac{\lim _{n \rightarrow \infty} a_n}{\lim _{n \rightarrow \infty} b_n} & & = \frac{a}{b}
> \end{aligned}
> $$
