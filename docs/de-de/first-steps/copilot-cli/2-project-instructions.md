---
title: "Lektion 2 - Projektanweisungen festhalten"
description: "Führe /init aus, um Agent-Anweisungen zu erzeugen, die das fertige Weltraum-Quiz beschreiben, und passe sie dann an deine Arbeitsweise an."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-05
---

Mit einem funktionierenden Quiz auf der Festplatte kannst du Agent-Anweisungen erzeugen, die das echte Projekt beschreiben. Jede künftige Sitzung liest diese Anweisungen, bevor sie mit der Arbeit beginnt. So musst du nicht in jedem Prompt dieselben Hinweise wiederholen.

In dieser Lektion wirst du:

- Agent-Anweisungen mit `/init` erzeugen.
- die erzeugte Datei prüfen, bevor du sie übernimmst.
- die Anweisungen kürzen und anpassen.

## Regeln mit `/init` festhalten

In Copilot CLI funktioniert `/init` auch allein. Du kannst aber zusätzlich Hinweise mitgeben, die steuern, was erzeugt wird, wie in der [Befehlsreferenz der CLI][cli-init] beschrieben. Dieses Beispiel bittet um einfache Projektregeln.

1. Führe in der Sitzung `/init create simple rules for the project` aus.
2. Prüfe die erzeugte Anweisungsdatei, bevor du sie übernimmst.
3. Behalte nur Hinweise, die zu diesem Projekt passen: eine einzelne Datei, keine Abhängigkeiten, barrierefrei und im Browser getestet.

> [!IMPORTANT]
> **Die Reihenfolge ist wichtig**
>
> `/init` liest das Projekt so, wie es gerade vorliegt. Wenn du den Befehl ausführst, nachdem das Quiz gebaut und verfeinert wurde, entstehen Anweisungen, die auf echtem Code beruhen.

## Mach sie zu deinen eigenen

Die Anweisungsdatei ist nicht nur für Fakten über das Projekt gedacht. Ergänze die Besonderheiten, die du sonst in jedem Prompt wiederholen würdest, etwa wie du Code gern schreibst, Namenskonventionen, welche Bibliotheken du vermeiden möchtest und wie viele Kommentare du dir wünschst. Jede künftige Sitzung liest diese Datei, bevor sie deinen Prompt liest.

## Zusammenfassung und nächste Schritte

Dein Projekt hat jetzt Agent-Anweisungen, die auf echtem Code beruhen. Weiter geht es mit [Lektion 3: Das Projekt veröffentlichen][next-lesson].

[next-lesson]: ../3-publish/
[cli-init]: https://docs.github.com/copilot/reference/copilot-cli-reference/cli-command-reference#project-initialization-for-copilot
