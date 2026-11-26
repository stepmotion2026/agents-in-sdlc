---
title: "Lektion 10 - Rückblick und nächste Schritte"
description: "Gehe den Ablauf mit Copilot CLI noch einmal durch und finde Ressourcen zum Weiterlernen."
authors:
  - jamesmontemagno
lastUpdated: 2026-09-28
---

Du hast den terminalbasierten Ablauf durchlaufen: Du hast das Quiz erstellt, Diffs geprüft, veröffentlicht, Sitzungen parallel ausgeführt, vor dem Bearbeiten geplant, Sitzungen fortgesetzt, einen Pull Request gemergt und neue Arbeit delegiert, ohne das Terminal zu verlassen.

## Was du abgeschlossen hast

Du hast:

- Copilot CLI installiert und mit `/model` ein Modell ausgewählt.
- aus einem einzigen Prompt ein Quiz erstellt und verfeinert.
- Projektregeln mit `/init` festgehalten.
- das Projekt per Prompt oder von Hand veröffentlicht.
- ein Issue über die Seitenleiste zum Chat hinzugefügt und die Änderung mit `/diff` geprüft.
- mit `/worktree` eine zweite Sitzung in einem eigenen Worktree ausgeführt.
- das zweite Issue mit `/plan` geplant, bevor sich Code geändert hat.
- den Kontext mit `/context` und `/clear` untersucht und verwaltet.
- Sitzungen mit `copilot --resume` und `/resume` fortgesetzt.
- mit `/pr create` und `/pr agentmerge` einen Pull Request erstellt und gemergt.
- mit `/delegate` ein neues Feature delegiert.

## Weiter erkunden

- [Installiere Copilot CLI unter macOS, Windows und Linux][install-cli].
- [Erfahre mehr über Copilot CLI sowie seine Slash-Befehle und Flags][about-cli].
- [Nutze die GitHub CLI für Repositories und Pull Requests][gh-cli].
- [Installiere Git][git].
- [Beachte bewährte Vorgehensweisen für Prompts, die sich bei echtem Code bewähren][best-practices].
- [Vergleiche die Copilot-Pläne][copilot-plans].

Durchlaufe dasselbe Weltraum-Quiz mit einer anderen Arbeitsweise, und zwar im [Workshop „Erste Schritte mit der GitHub-Copilot-App“][first-steps-app] oder im [Workshop „Erste Schritte mit Visual Studio Code“][first-steps-vscode]. Wenn du für ein anspruchsvolleres Szenario mit einer vollständigen Anwendung und einem Team-Backlog bereit bist, mache mit dem [praxisnahen Copilot-CLI-Workshop][real-world-cli] weiter.

[install-cli]: https://docs.github.com/copilot/how-tos/set-up/install-copilot-cli
[about-cli]: https://docs.github.com/copilot/concepts/agents/about-copilot-cli
[gh-cli]: https://cli.github.com/
[git]: https://git-scm.com/downloads
[best-practices]: https://docs.github.com/copilot/get-started/best-practices
[copilot-plans]: https://github.com/features/copilot/plans
[first-steps-app]: ../../copilot-app/
[first-steps-vscode]: ../../vscode/
[real-world-cli]: ../../../real-world-development/cli/
