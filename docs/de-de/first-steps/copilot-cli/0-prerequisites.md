---
title: "Lektion 0 - Voraussetzungen und Einrichtung"
description: "Prüfe die Voraussetzungen für den Workshop, installiere GitHub Copilot CLI, melde dich an und wähle in einem leeren Projektordner ein Modell aus."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-05
---

Hol dir einen Agenten ins Terminal. Stelle sicher, dass du alles Nötige hast, installiere GitHub Copilot CLI, melde dich an und bereite dich darauf vor, in einem leeren Ordner deine erste Anfrage zu stellen.

In dieser Lektion wirst du:

- die Voraussetzungen für den Workshop prüfen.
- GitHub Copilot CLI installieren und dich anmelden.
- den Projektordner erstellen und als vertrauenswürdig einstufen.
- ein Modell für deine Sitzung auswählen.

## Voraussetzungen

Du benötigst:

- ein GitHub-Konto. [Erstelle ein GitHub-Konto][github-signup] oder verwende dein bestehendes Konto.
- einen aktiven Copilot-Plan. [Aktiviere Copilot Free oder einen kostenpflichtigen Copilot-Plan][copilot-plans]. Wenn deine Organisation bereits Copilot-Zugriff bereitstellt, verwende dieses Konto.
- eine Installation von [Git][git]. Führe `git --version` aus, um das zu prüfen.
- einen Computer mit macOS, Windows oder Linux.

Die [GitHub CLI][gh-cli] (`gh`) ist optional, wird aber empfohlen, weil der Agent damit Repositories und Pull Requests für dich erstellen kann.

> [!NOTE]
> Wenn du Copilot Business oder Copilot Enterprise verwendest, muss dein Administrator die Richtlinie **Copilot CLI** aktivieren, damit Agent-Sitzungen funktionieren.

## Die CLI einrichten

1. Installiere [GitHub Copilot CLI][install-cli] für deine Plattform.
2. Erstelle den Projektordner und wechsle hinein:

   ```bash
   mkdir space-quiz && cd space-quiz
   ```

3. Führe `copilot` aus, melde dich an und bestätige bei der Abfrage, dass du dem Ordner vertraust.
4. Führe `/model` aus und wähle ein Modell anhand der Reihenfolge im nächsten Abschnitt.
5. Installiere optional die [GitHub CLI][gh-cli], falls du sie noch nicht hast.

![Illustration von Copilot CLI in einem Terminalfenster mit dem Titel space-quiz. Es fragt, ob den Dateien in diesem Ordner vertraut wird, wobei Yes, proceed ausgewählt ist, und verweist auf den Befehl /model zur Auswahl des Modells für diese Sitzung sowie auf /help, um alle Slash-Befehle aufzulisten. Die Eingabezeile lautet Create a space exploration quiz.](../../../_images/first-steps-cli-welcome.svg)

Die CLI startet mit einer Vertrauensabfrage und einigen Startbefehlen, darunter `/model`.

> [!TIP]
> Gib jederzeit `/` ein, um alle verfügbaren Befehle zu durchsuchen, oder führe `/help` für die vollständige Referenz aus.

## Ein Modell auswählen

Gehe beim Ausführen von `/model` in der folgenden Reihenfolge vor und wähle die erste Option, die dir zur Verfügung steht:

1. **GPT-6-Luna** (empfohlen).
2. **Auto** als ausgewogene Ausweichoption.
3. Ein beliebiges Modell aus der [Liste der aktiven Modelle][active-models].

Welche Modelle verfügbar sind, hängt von deinem Plan, den Richtlinien deiner Organisation und der Produktversion ab.

## Zusammenfassung und nächste Schritte

Copilot CLI ist installiert, du bist angemeldet, und die CLI läuft in einem leeren Ordner `space-quiz`. Weiter geht es mit [Lektion 1: Das Quiz im Terminal erstellen][next-lesson].

[github-signup]: https://github.com/signup
[copilot-plans]: https://github.com/features/copilot/plans
[git]: https://git-scm.com/downloads
[gh-cli]: https://cli.github.com/
[install-cli]: https://docs.github.com/copilot/how-tos/set-up/install-copilot-cli
[active-models]: https://docs.github.com/copilot/reference/copilot-billing/models-and-pricing
[next-lesson]: ../1-build/
