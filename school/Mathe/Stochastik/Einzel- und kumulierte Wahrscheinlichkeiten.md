***

#### Aufgabe im Heft:
$P(X = 4) = B_{50;0,05}(4) \approx 0,1360$

**Bedeutung:**
Wahrscheinlichkeit für *genau* vier Treffer bei fünfzig Versuchen mit einer Wahrscheinlichkeit von 5%

**GTR-Befehl:**
```binompdf(50,0.05,4)```


#### Aufgabe im Heft:
$P(X \leq 4) = F_{50;0,05}(4) \approx 0,8964$

**Bedeutung:**
Wahrscheinlichkeit für *höchstens* vier Treffer bei fünfzig Versuchen mit einer Wahrscheinlichkeit von 5%

**GTR-Befehl:**
```binomcdf(50,0.05,4)```


#### Aufgabe im Heft:
$P(X \geq 3) = 1 - F_{50;0,05}(2) \approx 0,4595$

**Bedeutung:**
Wahrscheinlichkeit für *mindestens* drei Treffer bei fünfzig Versuchen mit einer Wahrscheinlichkeit von 5%

**GTR-Befehl:**
```binomcdf(50,0.05,3,50)```

oder 

```1 - binomcdf(50,0.05,2)```


#### Aufgabe im Heft:
$P(1 \leq X \leq 5) = F_{50;0,05}(5) - F_{50;0,05}(0) \approx 0,8853$

**Bedeutung:**
Wahrscheinlichkeit für mindestens einen und höchstens fünf Treffer bei fünfzig Versuchen mit einer Wahrscheinlichkeit von 5%

**GTR-Befehl:**
```binomcdf(50,0.05,1,5)```

oder

```binomcdf(50,0.05,5) - binomcdf(50,0.05,0)```


#### Aufgabe im Heft:
$P(X \leq 1 \cup X \geq 5) = F_{50;0,05}(1) + 1 - F_{50;0,05}(4) \approx 0,3830$

**Bedeutung:**
Wahrscheinlichkeit für höchstens einen oder mindestens fünf Treffer bei fünfzig Versuchen mit einer Wahrscheinlichkeit von 5%

**GTR-Befehl:**
```binomcdf(50,0.05,1) + binomcdf(50,0.05,5,50)```

oder

```1 - binomcdf(50,0.05,2,4)```


#### Kumulierte Wahrscheinlichkeiten
Unter kumulierten Wahrscheinlichkeiten versteht man die Summe aller benannten Einzel- (oder Punkt-) Wahrscheinlichkeiten.