---
title: "Lektion 3 - Das Projekt veröffentlichen"
description: "Initialisiere das Weltraum-Quiz, committe es und veröffentliche es auf GitHub, entweder per Prompt oder indem du die Befehle selbst ausführst."
authors:
  - jamesmontemagno
lastUpdated: 2026-09-28
---

Mach aus dem Experiment ein öffentliches GitHub-Repository. Du kannst das mit einem einzigen Prompt anfordern oder die Befehle selbst ausführen. Probiere beide Wege einmal aus, dann weißt du genau, was der Agent in deinem Auftrag tut.

In dieser Lektion wirst du:

- ein Git-Repository initialisieren und den ersten Commit erstellen.
- ein öffentliches GitHub-Repository erstellen und dorthin pushen.
- bestätigen, dass der Commit und die Datei angekommen sind.

## Option A: Den Agenten darum bitten

Sende den folgenden Prompt:

```plaintext
Initialize this folder as a Git repository, create an initial commit, and create a new public GitHub repository named space-quiz in my account. Push the current branch and set it as the default branch.
```

Genehmige jede Git- und GitHub-Aktion, sobald der Agent sie anfordert.

## Option B: Selbst ausführen

Setze jedem Befehl ein `!` voran, um ihn innerhalb der Sitzung auszuführen, oder führe die Befehle ohne Präfix in deinem eigenen Terminal aus:

```plaintext
!git init -b main
!git add .
!git commit -m "Add space quiz"
!gh repo create space-quiz --public --source=. --push
```

Der letzte Befehl verwendet die [GitHub CLI][gh-cli]. Falls du sie nicht hast, erstelle das Repository auf GitHub und führe dann `!git remote add origin <url>` und `!git push -u origin main` aus.

## Das Ergebnis bestätigen

1. Führe `!git log --oneline` aus, um zu bestätigen, dass der Commit angekommen ist.
2. Öffne das Repository auf GitHub und bestätige, dass `index.html` vorhanden ist.

## Zusammenfassung und nächste Schritte

Dein Projekt ist jetzt ein GitHub-Repository mit einer bewährten Version, mit der du vergleichen kannst. Weiter geht es mit [Lektion 4: Issues parallel bearbeiten][next-lesson].

[gh-cli]: https://cli.github.com/
[next-lesson]: ../4-issues-and-sessions/
