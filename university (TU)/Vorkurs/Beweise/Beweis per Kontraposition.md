---
tags:
- Beweise
- Logik
flashcard: false
source: "Skript p. 21"
date created: 2024-04-11
types: 
examples: 
constructions: 
generalizations: 
justifications:
---
***
#### Definition

Manchmal ist es leichter, statt der Implikation "$A \implies B$" eine dazu äquivalente Aussage zu Beweisen. Wir beweisen "$A \implies B$" also nicht direkt, sondern *indirekt*.

> [!definition] Beweis per Kontraposition (Umkehrschluss)
> Beim Umkehrschluss beweisen wir statt der Aussage "$A \implies B$" die Aussage "$\neg B \implies \neg A$". Letztere bezeichnen wir als **Kontraposition** von "$A \implies B$".

***
#### Eigenschaften

> [!remark] Fehler beim Beweisen per Kontraposition
> Ein häufiger Fehler beim Beweis per Kontraposition besteht im Bilden der Kontraposition. Insbesondere ist die Kontraposition der Implikation "$A \implies B$" **nicht** "$B \implies A$" (Dies nennen wir *Umkehrung*), und auch nicht "$\neg A \implies \neg B$" (Das ist die Umkehrung der Kontraposition).


***
#### Beispiele

> [!exm|*] Beispiel für einen Beweis per Kontraposition 
> Für alle $n \in \mathbb{N}$ gilt: $n^{2}$ ist gerade $\implies$ $n$ ist gerade.
> 
> `\begin{proof}`
> Wir beweisen den Satz per Kontraposition, d.h. statt der ursprünglichen Aussage zeigen wir ihre Kontraposition: "$n$ ist ungerade $\implies$ $n^{2}$ ist ungerade."
> Sei also $n \in \mathbb{N}$ ungerade, d.h. es existiert ein $k \in \mathbb{N}$ mit $n = 2k + 1$. Dann folgt
> $$
> n^{2} = (2k + 1)^{2} = 4k^{2} + 4k + 1 = 2(2k^{2} + 2k) + 1
> $$
> 
> d.h. auch $n^{2}$ ist ungerade, da $(2k^{2} + 2k) \in \mathbb{N}$ gilt.
> `\end{proof}`

^707a66


***
