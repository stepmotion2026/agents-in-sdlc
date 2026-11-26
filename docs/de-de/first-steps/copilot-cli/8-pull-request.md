---
title: "Lektion 8 - Aus der CLI erstellen, prüfen und mergen"
description: "Prüfe den endgültigen Diff, erstelle mit /pr create einen Pull Request, arbeite Feedback ein und merge mit /pr agentmerge."
authors:
  - jamesmontemagno
lastUpdated: 2026-09-28
---

Schließe den Entwicklungszyklus ab, ohne zu einer grafischen Desktop-Oberfläche zu wechseln.

In dieser Lektion wirst du:

- die geänderten Dateien ein letztes Mal prüfen.
- aus dem aktuellen Branch einen Pull Request erstellen.
- den Pull Request prüfen und Feedback einarbeiten.
- den Pull Request mit `/pr agentmerge` validieren und mergen.

## Erstellen, prüfen und mergen

1. Führe `/diff` aus, um die geänderten Dateien ein letztes Mal zu prüfen.
2. Bitte Copilot, aus dem aktuellen Branch einen Pull Request zu erstellen, oder führe `/pr create` aus.
3. Öffne in der Seitenleiste den Reiter **Pull requests** und prüfe Titel, Beschreibung, Dateien und Statusprüfungen.
4. Behebe umsetzbares Feedback, prüfe das Ergebnis im Browser und antworte mit dem, was sich geändert hat.
5. Wenn der Pull Request bereit ist, führe `/pr agentmerge` aus. Der Befehl validiert ihn und mergt ihn, nachdem die erforderlichen Bestätigungen und Prüfungen bestanden sind.

## Zusammenfassung und nächste Schritte

Du hast einen Pull Request erstellt, geprüft und gemergt, ohne das Terminal zu verlassen. Weiter geht es mit [Lektion 9: Arbeit delegieren, sobald du dem Ablauf vertraust][next-lesson].

[next-lesson]: ../9-delegate/
