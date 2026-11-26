---
title: "Lektion 1 - Das Quiz im Terminal erstellen"
description: "Bitte Copilot CLI in einer einzigen ausführlichen Anfrage um das gesamte Weltraum-Quiz und nimm dann eine gezielte Verfeinerung vor."
authors:
  - jamesmontemagno
lastUpdated: 2026-09-28
---

Bitte in einer ausführlichen Anfrage um das ganze Projekt, prüfe den Vorschlag des Agenten, bevor du ihn genehmigst, und nimm dann eine kleine, klar abgegrenzte Änderung vor.

In dieser Lektion wirst du:

- ein Quiz ohne Abhängigkeiten in `index.html` erstellen.
- das Quiz aus der Sitzung heraus in einem Browser öffnen.
- eine gezielte Änderung vornehmen und überprüfen.

## Das Quiz erstellen

Sende den folgenden Prompt in deiner Copilot-CLI-Sitzung:

```plaintext
Create a space exploration quiz with 10 questions, a progress bar, score counter, and colorful animated feedback (green for correct, red shake for wrong). Show a results screen with an emoji reaction at the end. Single index.html, no server or dependencies. Accessible, keyboard-navigable, and respects prefers-color-scheme.
```

1. Lies den vorgeschlagenen Plan und genehmige die Dateiänderungen.
2. Öffne `index.html` in einem Browser und spiele ein paar Fragen durch. Um die Datei aus der Sitzung zu starten, führe `!open index.html` unter macOS, `!start index.html` unter Windows oder `!xdg-open index.html` unter Linux aus.

## Eine kleine Änderung vornehmen und prüfen

Bitte um eine gezielte Verfeinerung, damit du siehst, wie sich eine eng gefasste Anfrage verhält:

```plaintext
The results screen feels flat. Give it a stronger sense of arrival: animate the score counting up and make the emoji reaction larger. Change nothing else.
```

1. Lade die Seite im Browser neu und spiele das Quiz bis zum Ende durch.
2. Beachte, dass sich noch nichts in Git befindet und es deshalb nichts gibt, womit du vergleichen könntest. Das ändert sich, sobald du das Projekt veröffentlichst.

## Zusammenfassung und nächste Schritte

Du hast das Quiz erstellt und mit einer eng gefassten Anfrage verfeinert. Weiter geht es mit [Lektion 2: Projektanweisungen festhalten][next-lesson].

[next-lesson]: ../2-project-instructions/
