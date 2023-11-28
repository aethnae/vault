---
tags:
  - finanzmathematik
week: 2023-11-21
flashcard: false
publish: true
---
***

Wir stellen uns nun die Frage, was passiert, wenn die Zinsen **nicht jährlich ausgezahlt** werden, sondern in kürzeren Abständen und dafür nur in Teilen. Zum Beispiel könnten die Zinsen statt einmal in Jahr vollständig, zu 12 gleich großen Teilen jeden Monat gezahlt werden, oder zu 52 gleich großen Teilen jede Woche. Der Unterschied zur jährlichen Verzinsung ergibt sich dadurch, dass **durch die häufigere Zahlung auch mehr Zinseszinsen** gezahlt werden.

Formal fragen wir uns: Was passiert, wenn ein Jahr in $m$ Teilperioden zerlegt wird, und am Ende jeder Teilperiode $\frac{p}{m} \%$ Zinsen auf das aktuelle Kapital gezahlt werden? Und was passiert, wenn $m \rightarrow \infty$, die Auszahlungszeiträume also beliebig klein werden?

Wird $\frac{p}{m} \%$ Zinsen in $m$ Intervallen ausgezahlt, so ergibt sich am Ende des vollen Jahres das Kapital
$$
\begin{aligned}
K_1 & =K_0 \cdot \underbrace{\left(1+\frac{\frac{p}{m}}{100}\right) \cdot\left(1+\frac{\frac{p}{m}}{100}\right) \cdot \ldots \cdot\left(1+\frac{\frac{p}{m}}{100}\right)}_{m-\mathrm{mal}} \\
& =K_0 \cdot\left(1+\frac{\frac{p}{100}}{m}\right)^m
\end{aligned}
$$

Wir sprechen von stetiger Verzinsung, wenn beliebig kleine Bruchteile vom Gesamtzins in beliebig kurzen Intervallen ausgezahlt werden. Formal heißt dies, das Kapital $K_1$ nach einem Jahr bei stetiger Verzinsung beträgt:
$$
K_1=\lim _{m \rightarrow \infty} K_0 \cdot\left(1+\frac{\frac{p}{100}}{m}\right)^m \stackrel{\text { Satz }}{=}{ }^{1.9} K_0 \cdot e^{\frac{p}{100}} .
$$

Daraus erhalten wir, dass das Kapital nach der Zeit $t$ in Jahren
$$
K_t=K_0 \cdot e^{\frac{p}{100} \cdot t}
$$
beträgt.

***
##### Stetige vs. jährliche Verzinsung
Aufgrund der Zinseszinseffekte liefert stetige Verzinsung höhere Kapitalwerte als die einfache jährliche Verzinsung. Wird zum Beispiel ein Kapital von $K_0=$ 12.000 zu einem Zinssatz von $p=5 \%$ für $t=7$ Jahre angelegt, so ergibt sich bei jährlicher Verzinsung ein Endkapital von
$$
K_7=12.000 \cdot(1,07)^7 \approx 16.885,21,
$$
während stetige Verzinsung mit gleichem Zinsfuß $p=5$ ein Endkapital von
$$
\bar{K}_7=12.000 \cdot e^{0,05 \cdot 7} \approx 17.028,81
$$
ergibt.

Möchte man jährliche Verzinsung mit einem Zinsfuß $p$ mit stetiger Verzinsung abbilden, so muss man einen äquivalenten, stetigen Zinsfuß $\bar{p}$ berechnen. Dieser ergibt sich aus der Gleichung $K_0 \cdot\left(1+\frac{p}{100}\right)^t=K_0 \cdot e^{\frac{\bar{p}}{100} t}$ als
$$
\bar{p}=100 \cdot \ln \left(1+\frac{p}{100}\right)
$$

Im Beispiel von oben wäre der zu $p=5$ äquivalente, stetige Zinsfuß $\bar{p}=100 \cdot \ln (1,05) \approx 4,879$.
