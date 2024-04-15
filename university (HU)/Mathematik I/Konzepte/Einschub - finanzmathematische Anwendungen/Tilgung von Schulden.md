---
tags:
  - finanzmathematik
week: 2023-11-21
flashcard: false
publish: true
---
***

In diesem Modell beginnt das Darlehen mit einer Anfangsschuld von $K_0$. Jährlich fallen Zinsen in Höhe von $p \%$ an, die auf die Schulden addiert werden. Zusätzlich werden jährliche Zahlungen (sogenannte Annuitäten) in Höhe von $a$ geleistet, um die Schulden abzutragen. Nach $n$ Jahren (wobei $n$ die Laufzeit ist), soll die Restschuld $K_n=0$ betragen. 

![[Pasted image 20231128162757.png|center|450]]

Gegeben einer Restschuld $K_{i-1}$ im Vorjahr, ergeben sich die neuen Schulden am Ende des Jahres $i$ als
$$
K_i=K_{i-1}+K_{i-1} p-a=K_{i-1} q-a,
$$

denn die Schulden am Ende von Jahr $i$ sind Schulden von Jahr $i-1$ plus Zinsen minus Annuität. Für die Restschuld $K_i$ ergibt sich daraus im Allgemeinen nach $i$ Jahren
$$
\begin{aligned}
K_i & =K_0 q^i-a q^{i-1}-\ldots-a q-a \\
& =K_0 q^i-a\left(q^{i-1}-\ldots-q-1\right) \\
& =K_0 q^i-a \frac{1-q^i}{1-q} .
\end{aligned}
$$

Da nach der Laufzeit von $n$ Jahren das Darlehen zurückgezahlt sein soll, muss also gelten $K_n=$ $K_0 q^n-a \frac{1-q^n}{1-q}=0$. Dies ergibt umgestellt die Gleichung
$$
K_0 q^n=a \frac{1-q^n}{1-q} .
$$

***

Anhand dieser Gleichung kann die Formel für alle Parameter, wie im folgenden beschrieben, hergeleitet werden:

##### Berechnung der Annuität:
$$
a=K_0 \underbrace{q^n \frac{1-q}{1-q^n}}_{\text {Annuitätenfaktor }}
$$

##### Berechnung der Tilgungszeit:
$$
n=\frac{\ln \left(\frac{a}{K_0(1-q)+a}\right)}{\ln (q)}
$$

##### Berechnung der Anfangsschuld:
$$
K_0=\frac{a}{q^n} \frac{1-q^n}{1-q}
$$

##### Berechnung des Zinssatzes:
$$
q^{n+1}-\frac{K_0+a}{K_0} q^n+\frac{a}{K_0}=0
$$

Diese Formel ist nur eine implizite Formel für den Zinssatz. Im Allgemeinen ist die linke Seite der Gleichung ein Polynom vom Grad $n+1$, dessen Nullstellen genau der gesuchte Aufzinsfaktor $q$ sind. Aus diesem lässt sich dann mit $p=100 \cdot(q-1)$ der Zinsfuß berechnen. Da es für allgemeine Polynome keine geschlossene Formel für die Nullstellen gibt, muss die Gleichung ggf. mit numerischen Verfahren gelöst werden.