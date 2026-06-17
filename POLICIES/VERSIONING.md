---
title: "Versionierungs- und Release-Policy"
version: "0.1.0"
last_reviewed: "2026-06-17"
status: "initial"
language: "de-DE"
type: "policy"
license: "CC-BY-4.0"
repository_area: "POLICIES"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
topics:
  - "Versionierung"
  - "Semantic Versioning"
  - "Git-Tags"
  - "GitHub Releases"
  - "Changelog"
  - "Conventional Commits"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# Versionierungs- und Release-Policy

## 1. Zweck und Geltungsbereich

Diese Policy schafft eine schlanke Grundlage für transparente und reproduzierbare Stände der VergabeLab Community. Sie trennt Repository-Versionen, Dateiversionen und mögliche spätere Modulversionen. Eine Versionsnummer dokumentiert einen Stand, verspricht aber keine rechtliche oder fachliche Fehlerfreiheit.

## 2. Repository-Version

Repository-Releases folgen dem Schema `vMAJOR.MINOR.PATCH`. Ein Git-Tag und der zugehörige GitHub Release markieren denselben Repository-Stand. Der erste vorgesehene Repository-Release ist `v0.1.0`.

Releases werden ausschließlich auf einem geprüften Commit des Hauptbranches markiert. Veröffentlichte Tags werden nicht verschoben, überschrieben oder erneut verwendet.

## 3. Dateiversion

Das YAML-Feld `version` bezeichnet ausschließlich die Version der konkreten Datei. Es wird nur erhöht, wenn diese Datei geändert wird. Bei einem Repository-Release werden Dateiversionen nicht automatisch repositoryweit hochgezählt.

Regelmäßig gilt:

- redaktionelle Änderung: PATCH;
- kompatible substantielle Erweiterung: MINOR;
- grundlegende inkompatible Umgestaltung: MAJOR.

Das Feld `last_reviewed` dokumentiert eine Prüfung oder Aktualisierung, ersetzt aber keine Dateiversion.

## 4. Modulversion

Derzeit wird keine verbindliche gesonderte Modulversion geführt. `module_id` bezeichnet die fachliche Zuordnung, nicht die Version. Modulversionen werden erst eingeführt, wenn Modulmanifeste, Paketbildung oder verbindliche Modulverträge dies erfordern. In der gegenwärtigen Phase gibt es keine Modul-Tags.

## 5. Commit-SHA

Der Commit-SHA ist die exakte technische Referenz. Bei Testläufen und Eval-Berichten soll er möglichst dokumentiert werden. Ein Release-Tag erleichtert die menschliche Zuordnung; der SHA gewährleistet die eindeutige technische Referenz.

## 6. SemVer-Regeln für Repository-Releases

### PATCH

PATCH-Releases enthalten insbesondere:

- Fehlerkorrekturen;
- defekte Links;
- Metadatenkorrekturen;
- redaktionelle Klarstellungen ohne substantielle Erweiterung;
- kleinere kompatible Reparaturen.

### MINOR

MINOR-Releases enthalten insbesondere:

- ein neues Modul;
- einen neuen Prompt, Wissensbaustein oder ein neues Template mit eigenständigem Nutzen;
- eine neue Testakte;
- ein substantiell geändertes Testdesign;
- eine neue Policy;
- größere kompatible fachliche Erweiterungen.

### MAJOR

MAJOR-Releases enthalten insbesondere:

- einen grundlegenden inkompatiblen Strukturbruch;
- die Entfernung oder inkompatible Änderung zentraler öffentlicher Bausteine;
- den Bruch später verbindlich definierter Modul- oder Skill-Verträge;
- eine grundlegende Neuausrichtung von Lizenz- oder Governance-Modell.

Vor `1.0.0` kann ein MINOR-Release auch wesentliche oder potenziell inkompatible Änderungen enthalten. Solche Änderungen müssen im Changelog ausdrücklich als `Breaking` gekennzeichnet werden. MAJOR bleibt einer grundlegenden Neuausrichtung vorbehalten.

## 7. Changelog

`CHANGELOG.md` ist die maßgebliche menschenlesbare Release-Historie. Es nutzt die Struktur `Unreleased`, `Added`, `Changed`, `Fixed`, `Deprecated`, `Removed` und `Security`.

Nicht jede interne Commit-Nachricht muss in das Changelog übernommen werden. GitHub Release Notes werden aus dem Changelog abgeleitet oder ergänzen es. Widersprüche sind zugunsten des Changelogs zu bereinigen.

## 8. Commit-Konventionen

Empfohlen ist das Format:

```text
<type>(<scope>): <kurze Beschreibung>
```

Zulässige Typen sind mindestens:

- `feat`
- `fix`
- `docs`
- `test`
- `refactor`
- `chore`
- `ci`

Sinnvolle Scopes sind mindestens:

- `evals`
- `prompts`
- `wissen`
- `templates`
- `guides`
- `policies`
- `tooling`
- `ci`

Conventional Commits ersetzen den DCO-Trailer nicht. Jeder Commit im Pull Request muss weiterhin den erforderlichen `Signed-off-by`-Trailer tragen. Derzeit gibt es keine technische Commitlint-Zwangsprüfung.

## 9. Manueller Release-Prozess

Der manuelle Release-Prozess läuft in dieser Reihenfolge:

1. sauberer und geprüfter Hauptbranch;
2. Release-Inhalt festlegen;
3. `CHANGELOG.md` aktualisieren;
4. Release-Änderungen per Pull Request mergen;
5. annotierten Tag erstellen;
6. GitHub Release zu diesem Tag anlegen;
7. Release Notes anhand des Changelogs erstellen;
8. nachträgliche Korrekturen als neuer PATCH-Release;
9. veröffentlichte Tags niemals umschreiben.

## 10. Release-Reife

Ein Repository-Release bedeutet:

- einen dokumentierten gemeinsamen Stand;
- ein bestandenes vorhandenes Prüfverfahren;
- transparente Kennzeichnung experimenteller oder noch nicht vollständig getesteter Bestandteile.

Ein Repository-Release bedeutet nicht:

- rechtliche Beratung;
- Fehlerfreiheit;
- Eignung für jeden Einzelfall;
- vollständige Produktreife.

## 11. Automatisierung

Releases erfolgen zunächst manuell. Metadaten- und Linkprüfung sind eine mögliche nächste Stufe. Release-PR- und Changelog-Automatisierung kommen erst nach stabiler manueller Praxis in Betracht. Fachliche Dateiversionen werden nicht automatisch geändert.
