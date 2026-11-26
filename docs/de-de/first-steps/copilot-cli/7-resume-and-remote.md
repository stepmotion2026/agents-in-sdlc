---
title: "Lektion 7 - Fortsetzen und aus der Ferne arbeiten"
description: "Verlasse eine Copilot-CLI-Sitzung und kehre später mit copilot --resume oder /resume zu ihr zurück. Optional kannst du sie mit /remote von einem anderen Gerät aus verfolgen."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-05
---

Sitzungen lassen sich pausieren, ohne dass ihre Unterhaltung oder ihr Arbeitskontext verloren geht. Verlasse eine Sitzung, kehre später zu ihr zurück und mache sie optional von einem anderen Gerät aus verfügbar.

In dieser Lektion wirst du:

- eine Sitzung beenden und vom Terminal aus fortsetzen.
- zwischen Sitzungen wechseln, ohne die CLI zu verlassen.
- optional eine Sitzung aus der Ferne verfügbar machen.

## Eine Sitzung verlassen und später zurückkehren

1. Beende die aktuelle Copilot-CLI-Sitzung, wenn du bereit bist, die Aufgabe zu wechseln.
2. Führe in einem Terminal `copilot --resume` aus, um eine frühere Sitzung auszuwählen.
3. Verwende in Copilot CLI `/resume`, um zwischen Sitzungen zu wechseln, ohne die CLI zu verlassen.
4. Bestätige, dass die wiederhergestellte Sitzung noch die erwarteten Dateien, den Issue-Kontext und das Modell enthält.

## Optional: Eine Sitzung aus der Ferne fortsetzen

Führe `/remote` aus, damit *genau diese Sitzung* weiterhin lokal läuft und zugleich im Web und in der mobilen GitHub-Copilot-App verfügbar ist. Dein Computer muss dafür eingeschaltet bleiben. Öffne den zurückgegebenen Link in deinem Browser oder greife in der mobilen GitHub-Copilot-App auf die Sitzung zu.

> [!NOTE]
> `/remote` ist keine Delegation und verlagert die Ausführung nicht in die Cloud. Für diesen Workshop ist der Befehl nicht erforderlich. Probiere ihn aus, sobald sich der lokale Ablauf vertraut anfühlt.

## Zusammenfassung und nächste Schritte

Du kannst Sitzungen pausieren und fortsetzen und eine lokale Sitzung von einem anderen Gerät aus verfolgen. Weiter geht es mit [Lektion 8: Aus der CLI erstellen, prüfen und mergen][next-lesson].

[next-lesson]: ../8-pull-request/
