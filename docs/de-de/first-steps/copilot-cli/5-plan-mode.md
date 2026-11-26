---
title: "Lektion 5 - Erst planen, dann bearbeiten"
description: "Schalte die zweite Sitzung mit /plan in den Plan-Modus, damit der Agent einen Ansatz vorschlägt, bevor er Dateien bearbeitet."
authors:
  - jamesmontemagno
lastUpdated: 2026-09-28
---

Du hast bereits eine zweite Sitzung in einem eigenen Worktree laufen. Beginne dort nicht mit Code. Der Plan-Modus untersucht das Projekt und schlägt einen Ansatz vor, ohne deine Dateien anzufassen.

In dieser Lektion wirst du:

- die zweite Sitzung in den Plan-Modus schalten.
- den vorgeschlagenen Plan des Agenten prüfen und verfeinern.
- den Plan genehmigen und die Sitzung ihn umsetzen lassen.

## Sich vor jeder Bearbeitung auf den Ansatz einigen

1. Wechsle zu der **zweiten Sitzung**, die du in der vorherigen Lektion geöffnet hast.
2. Führe `/plan` aus, um diese Sitzung in den Plan-Modus zu schalten.
3. Sende den folgenden Prompt und lass den Agenten recherchieren, ohne etwas zu bearbeiten:

   ```plaintext
   Plan how to implement this issue. Investigate the existing quiz, list the files you would change, call out risks to accessibility and the single-file constraint, and stop before making any edits.
   ```

4. Lies den Plan, hake bei allem nach, was fehlt, und genehmige ihn dann.
5. Die Sitzung geht mit dem genehmigten Plan als Auftrag in die Umsetzung über.

> [!TIP]
> **Wann sich der Plan-Modus lohnt**
>
> Nutze den Plan-Modus bei allem, was mehrdeutig ist, mehrere Bereiche betrifft oder sich nur schwer rückgängig machen lässt. Ein schlechter Ansatz lässt sich am günstigsten vor der ersten Bearbeitung korrigieren.

## Zusammenfassung und nächste Schritte

Du hast dich mit dem Agenten auf einen Ansatz geeinigt, bevor er Code geschrieben hat. Weiter geht es mit [Lektion 6: Wissen, was der Agent sehen kann][next-lesson].

[next-lesson]: ../6-context/
