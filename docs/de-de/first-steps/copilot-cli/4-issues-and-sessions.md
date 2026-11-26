---
title: "Lektion 4 - Issues parallel bearbeiten"
description: "Erstelle ein Backlog, füge ein Issue über die Seitenleiste zum Chat hinzu, prüfe Änderungen mit /diff und starte eine zweite Sitzung in einem eigenen Worktree."
authors:
  - jamesmontemagno
lastUpdated: 2026-09-28
---

Behalte das Backlog und den Umsetzungszyklus im Terminal und öffne separate Sitzungen für voneinander unabhängige Aufgaben.

In dieser Lektion wirst du:

- drei klar umrissene GitHub-Issues erstellen.
- ein Issue über die Seitenleiste zum Chat hinzufügen und umsetzen.
- die Änderung mit `/diff` prüfen.
- eine zweite Sitzung in einem isolierten Worktree starten.

## Ein Backlog erstellen

Sende den folgenden Prompt:

```plaintext
Review the space quiz and create three focused GitHub issues with clear titles, user-focused descriptions, and acceptance criteria. Do not implement them yet.
```

## Das erste Issue in dieser Sitzung bearbeiten

1. Drücke die <kbd>Pfeil-links</kbd>-Taste, um die Seitenleiste zu öffnen, und drücke dann <kbd>Tab</kbd>, um zum Reiter **Issues** zu wechseln.
2. Markiere das erste Issue und drücke <kbd>c</kbd>, um es als Kontext zum Chat hinzuzufügen. Wenn du das Issue zuerst vollständig lesen möchtest, drücke stattdessen <kbd>Enter</kbd>.
3. Bitte den Agenten, das Issue umzusetzen.

![Illustration der Copilot-CLI-Seitenleiste in einem Terminal. Unter den Reitern Current, Sessions, Issues, Pull requests und Gists ist Issues ausgewählt. Ein Suchfilter für offene Issues im Repository space-quiz zeigt ein Issue, Add a score screen at the end of the quiz. Hinweise erklären, dass die Pfeil-links-Taste die Seitenleiste öffnet und Tab zwischen den Reitern wechselt. Die untere Zeile listet die Tasten: Schrägstrich zum Suchen, Enter für Details, o zum Öffnen, w für Worktree, c für Chat und a für alle.](../../../_images/first-steps-cli-side-panel.svg)

Die Seitenleiste zeigt oben alle Reiter. Die Hinweise am unteren Rand nennen die Tasten, die auf den jeweils markierten Eintrag wirken.

## Die Änderung mit `/diff` prüfen

Das Projekt ist veröffentlicht, daher gibt es eine bewährte Version zum Vergleichen. `/diff` zeigt genau, was dieses Issue darauf aufbauend geändert hat. Genau das würdest du auch jemandem zur Prüfung vorlegen.

1. Führe `/diff` aus und lies jede geänderte Datei.
2. Bitte um eine Korrektur für alles, was falsch aussieht, und führe dann `/diff` erneut aus.
3. Führe `!git status` oder `!git diff` aus, wenn du Git direkt untersuchen möchtest.

## Das zweite Issue parallel bearbeiten

1. Öffne die Seitenleiste erneut und wechsle zum Reiter **Sessions**.
2. Starte für das zweite Issue eine weitere Sitzung, ohne die erste zu verlieren.
3. Führe in der neuen Sitzung `/worktree` aus, damit sie einen isolierten Worktree erhält, statt am selben Ort zu verzweigen. Beide Sitzungen können jetzt gleichzeitig laufen, ohne sich zu stören.
4. Füge das zweite Issue mit <kbd>c</kbd> zu dieser Sitzung hinzu.
5. Lass die Sitzung vorerst dort stehen. Die nächste Lektion plant dieses Issue, bevor Code geschrieben wird.

![Illustration der Copilot-CLI-Ausgabe nach dem Ausführen von /worktree. Sie meldet, dass der Worktree ../space-quiz-13 auf dem Branch issue-13-review-screen erstellt wurde und dass diese Sitzung nun dort arbeitet, während main unberührt bleibt.](../../../_images/first-steps-cli-worktree.svg)

`/worktree` verschiebt die Sitzung in einen eigenen Checkout auf einem eigenen Branch, sodass die erste Sitzung ungestört weiterarbeitet.

## Zusammenfassung und nächste Schritte

Du hast das erste Issue umgesetzt, mit `/diff` geprüft und eine zweite Sitzung in einem eigenen Worktree gestartet. Weiter geht es mit [Lektion 5: Erst planen, dann bearbeiten][next-lesson].

[next-lesson]: ../5-plan-mode/
