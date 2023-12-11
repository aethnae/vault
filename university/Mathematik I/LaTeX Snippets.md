***

*Eine Auflistung der wichtigsten $\LaTeX$-Befehle in ==Latex Suite==.*

**Fehlende Snippets:**


***
### Umgebungen

1. Aktiviert Inline-Mathematik

```JSON
{trigger: "mk", replacement: "$$0$", options: "tA"}
```

2. Aktiviert Block-Mathematik

```JSON
{trigger: "dm", replacement: "$$\n$0\n$$", options: "tAw"}
```

3. Erzeugt eine \begin-Struktur

```JSON
{trigger: "beg", replacement: "\\begin{$0}\n$1\n\\end{$0}", options: "mA"}
```

### Griechische Buchstaben

*Griechische Buchstaben werden mit einem **@** vor dem entsprechenden Buchstaben erzeugt. Griechische Großbuchstaben, welche eine Bedeutung in der Mathematik haben, werden mit einem **@** und dem entsprechenden Großbuchstaben erzeugt.*

### Wichtige Symbole einzelner Rechenfunktionen

1. Texte innerhalb einer Gleichung

```JSON
{trigger: "te", replacement: "\\text{$0}", options: "m"}
```

2. Fett gedruckte Mathematik

```JSON
{trigger: "bf", replacement: "\\mathbf{$0}", options: "mA"}
```

3. Quadriere einen Term

```JSON
{trigger: "sr", replacement: "^{2}", options: "mA"}
```

4. Potenziere einen Term

```JSON
{trigger: "rd", replacement: "^{$0}$1", options: "mA"}
```

5. Unterstrich

```JSON
{trigger: "_", replacement: "_{$0}$1", options: "mA"}
```

6. Text im Unterstrich

```JSON
{trigger: "sts", replacement: "_\\text{$0}", options: "rmA"}
```

7. Quadratwurzeln

```JSON
{trigger: "sq", replacement: "\\sqrt{ $0 }$1", options: "mA"}
```

8. Brüche (Werden auch automatisch durch $/$ erzeugt)

```JSON
{trigger: "//", replacement: "\\frac{$0}{$1}$2", options: "mA"}
```

9. Eulersche Zahlen

```JSON
{trigger: "ee", replacement: "e^{ $0 }$1", options: "mA"}
```

