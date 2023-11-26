***
#### Grundlegende Rechengesetze
***

- **Kommutativgesetz**

$$
a + b = b + a \quad \quad a \cdot b = b \cdot a
$$

- **Assoziativgesetz**

$$
(a + b) + c = a + (b + c) \quad \quad a \cdot (b \cdot c) = (a \cdot b) \cdot c
$$

- **Distributivgesetz**

$$
(a + b) \cdot c = a \cdot c + b \cdot c \quad \quad a \cdot (b + c) = a \cdot b + a \cdot c
$$
***

#### Binomische Formeln
*Spezialfall der Distributivgesetze*
***

**Erste binomische Formel:**

$$
(a + b)^2 = a^2 + 2ab + b^2
$$

**Zweite binomische Formel:**

$$
(a - b)^2 = a^2 - 2ab + b^2
$$

**Dritte binomische Formel:**

$$
(a + b) \cdot (a - b) = a^2 - b^2
$$
***

#### Potenzgesetze
***
**1. Potenzgesetz:**

$$
a^r \cdot a^s = a^{r+s} \quad \quad a^r : a^s = a^{r - s}
$$

**2. Potenzgesetz:**

$$
(a^r)^s = a^{r \cdot s}
$$

**3. Potenzgesetz:**

$$
a^r \cdot b^r = (a \cdot b)^r
$$

**Spezialfälle:**

$$
a^0 = 1 \quad \quad a^1 = a \quad \quad a^{-b} = \frac{1}{a^b} \quad \text{(für $a, b \neq 0$)}
$$

***

#### Wurzelgesetze
***
**1. Wurzelgesetz:**

$$
\sqrt[n]{a^m} = a^{\frac{m}{n}}
$$

**2. Wurzelgesetz:**

$$
\sqrt[c]{ \sqrt[b]{ a } } = \sqrt[c \cdot b]{ a }
$$

**3. Wurzelgesetz**

$$
\sqrt[c]{ a } \cdot \sqrt[c]{ b } = \sqrt[c]{ a \cdot b }
$$

***

#### Logarithmen
*siehe [[Logarithmen]]*
***
**1. Logarithmengesetz:**

$$
\log_{a}(b \cdot c) = \log_{a}(b) + \log_{a}(c)
$$

**2. Logarithmengesetz:**

$$
\log_{a}\left( \frac{b}{c} \right) = \log_{a}(b) - \log_{a}(c)
$$

**3. Logarithmengesetz:**

$$
\log_{a}(b^{c}) = c \cdot \log_{a}(b)
$$

**4. Logarithmengesetz:**

$$
\log_{a}(b) = \frac{\log_{c}(b)}{\log_{c}(a)}
$$

**5. Logarithmengesetz:**

$$
\log_{a}(a^{x}) = x
$$

$e^x = b \leftrightarrow x = \ln(b)$

$e^{\ln(b)} = b$

$\ln(e^c) = c$

***

#### Ableitungen
***
**Faktorregel**

$$
(c \cdot u(x))' = c \cdot u'(x)
$$

**Summenregel:**

$$
(u(x) + v(x))' = u'(x) + v'(x)
$$

 **Produktregel:**

$$
(u(x) \cdot v(x))' = u'(x) \cdot v(x) + u(x) \cdot v'(x)
$$

**Kettenregel:**

$$
(u(v(x)))' = u'(v(x)) \cdot v'(x)
$$

**Quotientenregel:**

$$
\left( \frac{u(x)}{v(x} \right)' = \frac{u'(x) \cdot v(x) - u(x) \cdot {v'(x)}}{(v(x))^2}
$$

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
***

> [!summary] Grenzwertrechenregeln
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
