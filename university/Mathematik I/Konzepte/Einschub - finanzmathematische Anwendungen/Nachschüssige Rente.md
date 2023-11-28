---
tags:
  - finanzmathematik
week: 2023-10-21
flashcard: false
publish: true
---
***

In diesem Abschnitt schauen wir uns nun das umgekehrte Modell zum [[Bausparkonto mit nachschüssiger Verzinsung|Bausparkonto]] an; das Modell einer nachschüssigen Rente. Dabei wird nun ein Anfangskapital $R_0$ jedes Jahr mit einem Zinsfuß von $p$ verzinst. Außerdem wird in jedem Jahr eine Rente $r$ ausgezahlt (also das Kapital um $r$ verringert), sodass nach $n$ Jahren (die Laufzeit der Rente) das Endkapital $K_n=0$ ist.

![[Pasted image 20231128161351.png|center|600]]

Wir interessieren uns nun für den Barwert $R_0$ (also das Anfangskapital) bei fester Auszahlungsdauer $n$ und festem Zinsfuß $p$. Es gilt
$$
\begin{aligned}
R_0 & =r v+r v^2+\cdots+r v^{n-1}+r v^n \\
& =r v\left(1+v+\cdots+v^{n-1}\right)=r v \frac{1-v^n}{1-v} .
\end{aligned}
$$

Dabei ist $v=\frac{1}{q}=\frac{1}{1+\frac{p}{100}}$ der Abzinsfaktor.

##### Berechnung der Rente:
Sind Barwert $R_0$, Zinsfuß $p$ und Laufzeit $n$ gegeben, so kann entsprechende Rente berechnet werden als
$$
r=\frac{R_0(1-v)}{v\left(1-v^n\right)}
$$

##### Berechnung der Laufzeit:
Sind Barwert $R_0$, Zinsfuß $p$ und Rente $r$ gegeben, so kann die Laufzeit berechnet werden als
$$
n=\frac{\ln \left(1-\frac{R_0(1-v)}{r v}\right)}{\ln (v)} .
$$
