---
title: "Lektion 6 - Wissen, was der Agent sehen kann"
description: "Nutze /context, um zu prüfen, was das Kontextfenster füllt, und /clear, um neu zu beginnen, wenn eine Unterhaltung abdriftet."
authors:
  - jamesmontemagno
lastUpdated: 2026-09-28
---

Terminalbefehle machen den Kontext sichtbar und steuerbar. Wenn du weißt, was der Agent sehen kann, verstehst du seine Ergebnisse besser und kannst entscheiden, wann ein Neustart sinnvoll ist.

In dieser Lektion wirst du:

- das Kontextfenster mit `/context` untersuchen.
- sehen, wie viel Platz jeder Teil des Fensters belegt.
- eine abdriftende Unterhaltung mit `/clear` zurücksetzen.

## Den Kontext untersuchen

1. Führe `/context` aus, um Dateien, Anweisungen und den Gesprächsverlauf zu untersuchen.
2. Prüfe, wie viel Platz jeder Teil des Fensters belegt.
3. Führe `/clear` aus, um neu zu beginnen, wenn die Unterhaltung abgedriftet ist.
4. Füge die richtige Datei wieder hinzu, bevor du die nächste Änderung anforderst.

![Illustration der Copilot-CLI-Ausgabe nach dem Ausführen von /context. Eine Anzeige des Kontextfensters zeigt eine Auslastung von 61 Prozent, aufgeteilt auf Unterhaltung, gelesene Dateien und Anweisungen. Ein Hinweis empfiehlt, mit /compact zusammenzufassen oder eine neue Sitzung zu starten, wenn der Platz knapp wird.](../../../_images/first-steps-cli-context.svg)

`/context` zeigt genau, was das Kontextfenster füllt und wie viel Platz noch frei ist. Wenn der Platz knapp wird, fasse die Unterhaltung mit `/compact` zusammen oder starte eine neue Sitzung.

## Zusammenfassung und nächste Schritte

Du kannst jetzt sehen und steuern, was der Agent weiß. Weiter geht es mit [Lektion 7: Fortsetzen und aus der Ferne arbeiten][next-lesson].

[next-lesson]: ../7-resume-and-remote/
