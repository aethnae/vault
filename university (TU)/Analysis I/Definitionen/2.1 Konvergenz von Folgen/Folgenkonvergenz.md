---
tags:
- Folgen
flashcard: false
source: 
date created: 2024-10-31
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

> [!definition] Konvergenz von Folgen
> Sei $\left(a_n\right)_{n \in \mathbb{N}}$ eine Folge reeller Zahlen.
> 1. ( $a_n$ ) heißt konvergent gegen $a \in \mathbb{R}$, falls zu jedem $\varepsilon>0$ ein $N_{\varepsilon} \in \mathbb{N}$ existiert, so dass für alle $n \in \mathbb{N}$ mit $n \geq N_{\varepsilon}$ gilt, dass $\left|a_n-a\right|<\varepsilon$.
>    In diesem Fall heißt a Grenzwert (auch Limes) der Folge ( $a_n$ ). Schreibweise:
>    
>    $$
>    \lim _{n \rightarrow \infty} a_n=a \text { oder } \quad a_n \rightarrow a \text { für } n \rightarrow \infty
>    $$
> 2. ( $a_n$ ) heift konvergent, falls ein $a \in \mathbb{R}$ existiert, so dass $\left(a_n\right)$ konvergent gegen $a$ ist. Andernfalls heißt ( $a_n$ ) divergent.
> 3. $\left(a_n\right)$ heißt Nullfolge, falls $\left(a_n\right)$ gegen den Grenzwert $a=0$ konvergiert.

> [!definition] $\epsilon$-Umgebung
> Seien $\varepsilon>0$ und $a \in \mathbb{R}$. Dann heißt
> 
> $$
> U_{\varepsilon}(a):=\{x \in \mathbb{R}| | x-a \mid<\varepsilon\}=\mid a-\varepsilon, a+\varepsilon[
> $$
> 
> die $\varepsilon$-Umgebung von $a$.

***

#### Eigenschaften

> [!remark] Bemerkung zu $\epsilon$-Umgebungen
> Ist $\left(a_n\right)_{n \in \mathbb{N}}$ eine gegen $a \in \mathbb{R}$ konvergente Folge, so gibt es zu jedem $\varepsilon>0$ ein $N_{\varepsilon} \in \mathbb{N}$, so dass $a_n \in U_{\varepsilon}(a)$ für alle $n \geq N_{\varepsilon}$ gilt, d.h. in $U_{\varepsilon}(a)$ liegen bis auf endlich viele Ausnahmen alle Folgenglieder $a_n$. Da dies für jedes $\varepsilon>0$ gilt, können wir diese Erkenntnis mit der Abkürzung "fast alle" für "alle bis auf endlich viele" wie folgt zusammenfassen:
> 
> *"In jeder noch so kleinen $\varepsilon$-Umgebung um a liegen fast alle Folgenglieder $a_n$."*

***

#### Beispiele für Folgenkonvergenz

> [!exm] Folgenkonvergenz
> 1. Konstante Folgen sind konvergent, d.h. Folgen $\left(a_n\right)_{n \in \mathbb{N}}$ mit $a_n=a \in \mathbb{R}$ für alle $n \in \mathbb{N}$. Es folgt $\lim _{n \rightarrow \infty} a_n=a$, denn offenbar gilt
>    
>    $$
>    \left|a_n-a\right|=0<\varepsilon
>    $$
>    
>    für alle $n \in \mathbb{N}$ und alle $\varepsilon>0$. Wir können also $N_{\varepsilon}=0$ wählen.
> 2. Das klassische Beispiel für eine nicht konstante, konvergente Folge ist die Folge $\left(a_n\right)_{n \geq 1}$ mit $a_n=\frac{1}{n}$. Es gilt
>    
>    $$
>    \lim _{n \rightarrow \infty} \frac{1}{n}=0 .
>    $$
>    
>    Beweis: Sei $\varepsilon>0$ beliebig. (Dies ist der typische Beginn für den Konvergenzbeweis einer Folge.) Nach dem [[Vollständigkeitsaxiom#^f03eaa]]  existiert eine natürliche Zahl $N_{\varepsilon} \in \mathbb{N}$, so dass $\varepsilon N_{\varepsilon}>1$. Daher gilt für alle $n \geq N_{\varepsilon}$, dass
>    
>    $$
>    \left|\frac{1}{n}-0\right|=\frac{1}{n} \leq \frac{1}{N_{\varepsilon}}<\varepsilon
>    $$
>    
>    Da $\varepsilon>0$ beliebig war, folgt, dass $0$ der Grenzwert der Folge $\left(\frac{1}{n}\right)_{n \geq 1}$ ist. Für ein gegebenes $\varepsilon>0$ können wir leicht ein explizites $N_{\varepsilon}$ angeben, z.B. können wir für $\varepsilon=0.1$ die natürliche Zahl $N_{\varepsilon}=11$ wählen, da $11 \cdot 0.1=1.1>1$ gilt.
> 3. Ein Standardbeispiel für eine nicht konvergente Folge ist $\left(a_n\right)_{n \in \mathbb{N}}$ mit $a_n=(-1)^n$, also
>    
>    $$
>    \left(a_n\right)_{n \in \mathbb{N}}=(1,-1,1,-1,1,-1, \ldots) .
>    $$
>    
>    Wir weisen die Divergenz dieser Folge nach. Angenommen, es gibt ein $a \in \mathbb{R}$ mit $\lim _{n \rightarrow \infty} a_n=a$. Dann gibt es speziell zu $\varepsilon=1>0$ ein $N_1 \in \mathbb{N}$ mit $\left|a_n-a\right|<1$ für alle $n \geq N_1$. Für alle $n \in \mathbb{N}$ mit $n \geq N_1$ erhalten wir dann den Widerspruch
>    
>    $$
>    2=\left|a_{n+1}-a_n\right|=\left|a_{n+1}-a+a-a_n\right| \leq\left|a_{n+1}-a\right|+\left|a-a_n\right|<1+1=2,
>    $$
>    
>    also $2<2$. Folglich ist $\left(a_n\right)$ gegen kein $a \in \mathbb{R}$ konvergent.