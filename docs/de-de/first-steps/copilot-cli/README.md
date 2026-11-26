---
title: "Erste Schritte mit GitHub Copilot CLI"
description: "Mach eine geführte Tour durch GitHub Copilot CLI im Terminal, indem du ein Weltraum-Quiz erstellst und auslieferst."
slug: de-de/first-steps/copilot-cli
authors:
  - jamesmontemagno
lastUpdated: 2026-10-05
---

Mach eine praxisnahe, einsteigerfreundliche Tour durch GitHub Copilot CLI. Du erstellst aus einem leeren Ordner ein farbenfrohes Weltraum-Quiz und lernst den terminalbasierten Ablauf kennen: bauen und Diffs prüfen, bevor Git etwas schreibt, Sitzungen nebeneinander ausführen, vor dem Bearbeiten planen und dann den Pull Request erstellen und mergen, ohne die Shell zu verlassen.

Der Workshop dauert etwa 60 bis 90 Minuten. Dein Projekt besteht aus einer einzelnen HTML-Datei ohne Laufzeitabhängigkeiten, sodass du dich ganz auf die CLI und ihre agentischen Abläufe konzentrieren kannst.

> [!NOTE]
> Dieser Workshop wurde von [James Montemagno][james] erstellt und aus [First Steps with GitHub Copilot][source-lab] übernommen. Der ursprüngliche Inhalt ist unter der [MIT-Lizenz][source-license] verfügbar.

## Lektionen

| Lektion | Thema | Was du tun wirst |
| ------- | ----- | ---------------- |
| [0. Voraussetzungen und Einrichtung][lesson-0] | Einrichtung | Voraussetzungen prüfen, Copilot CLI installieren, anmelden und ein Modell auswählen |
| [1. Das Quiz erstellen][lesson-1] | Erstellen | Das Quiz im Terminal erstellen und eine gezielte Änderung vornehmen |
| [2. Projektanweisungen festhalten][lesson-2] | Anweisungen | Agent-Anweisungen mit `/init` erzeugen und anpassen |
| [3. Das Projekt veröffentlichen][lesson-3] | Veröffentlichen | Initialisieren, committen und veröffentlichen, per Prompt oder von Hand |
| [4. Issues parallel bearbeiten][lesson-4] | Umsetzen | Ein Backlog erstellen, ein Issue zum Chat hinzufügen, mit `/diff` prüfen und eine zweite Sitzung in einem Worktree starten |
| [5. Erst planen, dann bearbeiten][lesson-5] | Planen | Mit `/plan` einen Ansatz für das zweite Issue vereinbaren |
| [6. Wissen, was der Agent sehen kann][lesson-6] | Kontext | Den Kontext mit `/context` und `/clear` untersuchen und zurücksetzen |
| [7. Fortsetzen und aus der Ferne arbeiten][lesson-7] | Fortsetzen | Sitzungen mit `/resume` verlassen und wieder aufnehmen und optional mit `/remote` eine lokale Sitzung von einem anderen Gerät aus verfolgen |
| [8. Erstellen, prüfen und mergen][lesson-8] | Prüfen | Einen Pull Request mit `/pr create` und `/pr agentmerge` erstellen und mergen |
| [9. Arbeit delegieren][lesson-9] | Delegieren | Ein neues Feature mit `/delegate` übergeben und eine Cloud-Sitzung verfolgen |
| [10. Rückblick und nächste Schritte][lesson-10] | Prüfen | Den Ablauf zusammenfassen und weiterlernen |

## Loslegen

[Beginne mit Lektion 0: Voraussetzungen und Einrichtung][lesson-0].

[james]: https://github.com/jamesmontemagno
[source-lab]: https://github.com/jamesmontemagno/first-steps-with-github-copilot
[source-license]: https://github.com/jamesmontemagno/first-steps-with-github-copilot/blob/main/LICENSE
[lesson-0]: 0-prerequisites/
[lesson-1]: 1-build/
[lesson-2]: 2-project-instructions/
[lesson-3]: 3-publish/
[lesson-4]: 4-issues-and-sessions/
[lesson-5]: 5-plan-mode/
[lesson-6]: 6-context/
[lesson-7]: 7-resume-and-remote/
[lesson-8]: 8-pull-request/
[lesson-9]: 9-delegate/
[lesson-10]: 10-review/
