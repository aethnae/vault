---
tags:
  - beweis
week: 2023-11-24
publish: true
---
***
#### Formales Beweisprinzip der vollständigen Induktion

> [!abstract] Ziel
> Zu beweisen ist:
> $$
> \text{ Aussage } A(n) \text{ gilt für alle ganzen Zahlen } n \geq n_{0}
> $$

1. **Induktionsanfang** (IA)
Zeige, dass die Aussage $A(n)$ für $n=n_0$ wahr ist.

2. **Induktionsvoraussetzung** (IV)
Nehme an: Die Aussage $A(n)$ sei für ein beliebiges, aber festes $n \in \mathbb{Z}$ mit $n \geq n_0$ wahr.

3. **Induktionsschluss** (IS)
Zeige, dass, wenn die Induktionsvoraussetzung gilt, auch $A(n+1)$ wahr ist.
Das heißt, zeige
$$
A(n) \Rightarrow A(n+1)
$$