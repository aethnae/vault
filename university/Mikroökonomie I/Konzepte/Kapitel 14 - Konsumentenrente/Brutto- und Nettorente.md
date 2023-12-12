---
tags:
  - nutzen
  - nachfrage
  - rente
week: 2023-12-06
flashcard: false
publish: true
---
***
#### Bruttorente

> [!abstract] Definition
> Oftmals auch als **Bruttorente des Konsumenten** bezeichnet, misst diese Kennzahl den Nutzen aus dem Konsum des x-Gutes bei [[Quasilineare Präferenzen|quasilinearen Präferenzen]].
> Dieser wird graphisch beim Konsum von $n$ Einheiten als Fläche unter der Nachfragefunktion bis $n$ dargestellt, und mathematisch als $\mathrm{W}(q)$, also die **Zahlungsbereitschaft** für die Menge $q$.

***
#### Nettorente

> [!abstract] Definition
> Da der **Bruttonutzen** nur den Nutzen in Assoziation mit dem Konsum des x-Gutes misst, wird der Nutzen nach Abzug der Verringerung der Konsumausgaben für das andere Gut als **Nettorente**, bzw. einfach **Rente des Konsumenten** bezeichnet.
> Graphisch ist dies die Fläche unter Nachfragefunktion bis $n$, unter Abzug der Fläche unterhalb der Gerade, die den Preis $p$ darstellt.
> 
> Mathematisch gilt hier $\mathrm{CS}(q, T)=\mathrm{W}(q)-T$, also die Differenz aus ihrer Zahlungsbereitschaft und dem tatsächlich gezahlten Preis.

***
#### Veränderung der Rente

> [!abstract] Definition
> Die Veränderung der Rente einer Konsumentin als Folge einer Preisänderung wird mit $T + R$ angegeben. $R$ misst hierbei den Verlust der Rente, der daraus entsteht, dass die Konsumentin die Güter nun anstatt des Preises $p'$ zum höheren Preis $p''$ konsumieren muss. $T$ misst den Wert des *entgangenen* Konsums des x-Gutes, der entstanden ist, da die Konsumentin aufgrund der höheren Preise weniger konsumiert.

***
#### Berechnung der Rente mit Differentialrechnung
Die Rente des Konsumenten kann als Maximierungsproblem unter Nebenbedingung aufgefasst werden:

$$
\max_{x, y} v(x) + y \quad \text{ unter der Nebenbedingung } \quad px + y = m
$$

Nach Einsetzen der Budgetbeschränkung erhält man

$$
\max_{x, y} v(x) + m - px
$$

Aufgrund der Bedingung erster Ordnung ($v'(x) = p$) ist die [[Inverse Nachfragefunktionen|inverse Nachfragekurve]] durch 

$$
p(x) = v'(x)
$$

definiert.
Da die inverse Nachfragekurve die Ableitung der Nutzenfunktion misst, können wir die inverse Nachfragekurve integrieren, um die [[Nutzenfunktionen|Nutzenfunktion]] zu finden

$$
v(x) = v(x) - v(0) = \int_{0}^{x} v'(t) \, dt = \int_{0}^{x} p(t) \, dt
$$

Der mit dem Konsum des $x$-Gutes assoziierte Nutzen ist daher einfach die Fläche unter der [[Nachfragekurven|Nachfragekurve]].