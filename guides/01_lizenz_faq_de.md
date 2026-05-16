---
title: "Lizenz-FAQ"
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "guide"
license: "CC-BY-4.0"
repository_area: "guides"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
target_audience:
  - "Community-Mitwirkende"
  - "Vergabestellen"
  - "öffentliche Auftraggeber"
  - "Plattformanbieter"
topics:
  - "Lizenzierung"
  - "CC BY 4.0"
  - "EUPL 1.2"
  - "Attribution"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# Lizenz-FAQ (VergabeLab Community)

Diese FAQ ist eine praxisnahe Orientierung für Nutzer der VergabeLab-Community-Artefakte. Maßgeblich sind die Lizenztexte sowie die Lizenzangaben in den jeweiligen Dateien (SPDX-Header/README).

---

## 1) Welche Lizenz gilt für welche Inhalte?

**Grundsatz:** Textartefakte (Prompts/Hinweistexte, Templates, Guides, Muster, Wissensbausteine) stehen – sofern in der Datei nicht anders angegeben – unter **CC BY 4.0**.

**Ausnahme:** Echte Software-/Tooling-Bestandteile (Code, Plugins, Skripte) werden – sofern vorhanden – separat lizenziert (vorgesehen: **EUPL 1.2**) und in einem eigenen Ordner (z. B. `tooling/`) geführt.

**Wichtig:** Hat eine Datei einen SPDX-Header oder einen eindeutigen Lizenzhinweis, **geht dieser vor**.

---

## 2) Darf ich die Inhalte in Behördenprojekten und in KI-Setups nutzen (Custom GPT, Azure OpenAI, Self-hosted)?

Ja. **CC BY 4.0** erlaubt die Nutzung auch in professionellen und proprietären Umgebungen.  

Dabei gilt zusätzlich: Du musst natürlich **die Nutzungsbedingungen** deines jeweiligen KI-Anbieters/Setups einhalten (z. B. Datenverarbeitung, Zugriffskontrollen, Logging).

**Hinweis aus der Praxis:** Systemprompts/Hinweistexte sind nur ein Baustein. Achte bei realen Vergaben auf eine **belastbare Datenbasis**, **Vertraulichkeit**, **Datenminimierung** und darauf, keine Betriebs- und Geschäftsgeheimnisse oder personenbezogene Daten unkontrolliert einzuspeisen.

---

## 3) Muss ich bei rein interner Nutzung etwas „offenlegen“ oder veröffentlichen?

Bei **rein interner Nutzung** (keine Weitergabe an Dritte) entstehen typischerweise **keine praktischen Veröffentlichungspflichten** aus CC BY 4.0.

Sobald du Inhalte **weitergibst** (z. B. an IT-Dienstleister, Plattformanbieter, andere Behörden) oder **veröffentlichst**, gelten die **Attributionspflichten** (siehe unten).

**Empfehlung:** Auch intern ist ein kurzer Quellenvermerk sinnvoll (z.B. zwecks Nachvollziehbarkeit/Revision) und zeigt gleichzeitig Wertschätzung für dieses Projekt.

---

## 4) Was genau muss ich bei CC BY 4.0 angeben (Attribution)?

Wenn du Inhalte weitergibst oder veröffentlichst, solltest du mindestens angeben:
- Projekt/Quelle (VergabeLab Community + Repo-Link) + Urheber (Okan Doğan)
- Lizenz (CC BY 4.0) + Lizenzlink
- Hinweis, ob Änderungen vorgenommen wurden (kurz)

**Beispiel:**
> Basierend auf VergabeLab Community (c) 2026 Okan Doğan – CC BY 4.0.  
> Quelle: https://github.com/VergabeLab/vergabelab-community – Änderungen: angepasst für [Organisation], [Datum].

**Wo platzieren?**  
Geeignet sind z. B. Projektdokumentation, „Über dieses System“-Seite, Admin-Doku, Anlage/Quellenblatt in der Vergabeakte oder (bei Dokumentvorlagen) ein Quellenhinweis im Dokumentfuß.

---

## 5) Was gilt, wenn ich Prompts/Muster anpasse?

Anpassen ist erlaubt. Bei Weitergabe/Veröffentlichung gilt:
- **Attribution** wie oben
- **Änderungshinweis** (kurz, sachlich)
- keine Share-Alike-Pflicht (anders als BY-SA)

**Praxis-Tipp:** Pflege intern eine kurze Änderungsnotiz („Changelog“), damit du später erklären kannst, was gegenüber der Ausgangsversion geändert wurde.

---

## 6) Was gilt, wenn es (später) echte Software/Tools im Ordner `tooling/` gibt?

Für `tooling/` ist – sofern dort ausgewiesen – **EUPL 1.2** vorgesehen.  
Dann gelten die dortigen Regeln für Weitergabe/Änderungen gemäß EUPL (Lizenz- und Urheberhinweise beibehalten, Lizenztext beachten).

Solange `tooling/` nicht existiert oder keine EUPL-Dateien enthalten sind, betrifft dich das nicht.
