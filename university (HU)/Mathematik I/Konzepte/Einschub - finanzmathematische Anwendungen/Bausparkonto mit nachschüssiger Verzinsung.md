---
tags:
  - finanzmathematik
week: 2023-11-21
flashcard: false
publish: true
---
***

Wir betrachten nun ein leicht verändertes Modell, welches zum Beispiel zur Modellierung eines Bausparkontos genutzt werden kann. Im Gegensatz zu unserem ersten Modell gibt es nun kein **Anfangskapital** $K_0$ mehr, welches verzinst wird. Stattdessen werden **jährliche Einzahlungen** in Höhe von $b$ getätigt, die jeweils am Ende eines Jahres mit Zinsfuß $p$ verzinst werden (**nachschüssige Verzinsung**).

![[Pasted image 20231128161040.png|center|600]]

Als Formel für das Endkapital nach $n$ Jahren mit jährlicher Einzahlung $b$ und festem Zinssatz $p \%$ ergibt sich
$$
K_n=b q\left(1+q+\ldots q^{n-2}+q^{n-1}\right)=b q \frac{1-q^n}{1-q}
$$
