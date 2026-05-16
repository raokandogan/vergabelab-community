---
title: "README – VergabeLab Wissensbasis"
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "folder-readme"
license: "CC-BY-4.0"
repository_area: "wissen"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
target_audience:
  - "Community-Mitwirkende"
  - "Vergabestellen"
  - "öffentliche Auftraggeber"
  - "Vergabepraktiker"
topics:
  - "Wissensbasis"
  - "Wissensbausteine"
  - "Vergaberecht"
  - "KI"
  - "Systemprompts"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# wissen/ die VergabeLab Community Wissensbasis

Dieser Ordner enthält Hintergrundwissen und Referenzmaterial („Wissensbausteine“) zu VergabeLab-Themen. Die Inhalte sind dafür gedacht, Systemprompts fachlich zu unterfüttern und als Wissens-Upload (z. B. für ChatGPT Custom GPTs oder Claude Projects) verwendet zu werden.

**Wichtig:** In `wissen/` liegen keine ausfüllbaren Mustertexte und keine Systemprompts.

---

## Was gehört hier hinein?

Typische Inhalte:
- Leitfäden, Grundlagen, Überblicksdarstellungen (z. B. Markterkundung, Losbildung, Wertung)
- Begriffsklärungen/Abgrenzungen (z. B. „Eignung vs. Zuschlag“, „Muss- vs. Kann-Kriterien“)
- Praxis-Checklisten als Erläuterung (nicht als „Copy/Paste-Muster“)
- Kuratierte FAQs / typische Fallstricke („Do/Don’t“)
- Auszüge/Notizen zu Rechtsprechung oder Literatur als Zusammenfassung (keine Volltexte)
- Definierte Output-Standards für Modelle („wenn du X antwortest, nutze Struktur Y“)

---

## Was gehört nicht hier hinein?

Bitte nicht in `wissen/` ablegen:
- Systemprompts/Hinweistexte → gehören nach `prompts/`
- Ausfüllbare Muster (Musteranschreiben, Muster-LB, Matrizen, Formulare) → gehören nach `templates/`
- Integrations-/How-to-Anleitungen (z. B. Einrichtung Custom GPT) → gehören nach `guides/`
- Personenbezogene Daten, Vergabeinterna oder vertrauliche Inhalte

---

## Ordnerstruktur & Benennung

**Empfohlenes Schema:**
```text
wissen/
  <modul>/
    01_<kurztitel>_de.md
    02_<kurztitel>_de.md
    README.md
```

**Beispiele:**
- wissen/markterkundung/01_leitfaden_markterkundung_de.md
- wissen/leistungsbeschreibung/01_grundlagen_losbildung_de.md

**Hinweise:**
- Nummerierung (01_, 02_ …) ermöglicht stabile Referenzen und Wachstum.
- Sprache im Dateinamen markieren (_de, später ggf. _en).

---

## Lizenz & Header

`wissen/` enthält in der Regel Textwerke → Standardlizenz: CC BY 4.0.

Jede Datei soll am Anfang ein YAML-Frontmatter mit Metadaten und anschließend einen SPDX-Kommentar tragen. Zum Beispiel:

```text
---
title: "..."
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "knowledge"
license: "CC-BY-4.0"
repository_area: "wissen/..."
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->
```

Wenn Inhalte auf externen Quellen beruhen, sind die Quellen am Ende der Datei in einem sichtbaren Abschnitt ``` ## Quellen ``` anzugeben. Das gilt insbesondere für Rechtsprechung, Behördenleitfäden, Blogbeiträge, Fachaufsätze oder sonstige externe Materialien. Beispiel:

```text
## Quellen

- [Titel der Quelle], [Autor/Herausgeber], [URL], abgerufen am [Datum]. Nutzung: fachliche Auswertung/Zusammenfassung/Zitat, keine Übernahme fremder Textpassagen.
```
Fremde Inhalte dürfen nur übernommen, bearbeitet oder übersetzt werden, wenn die hierfür erforderlichen Nutzungsrechte vorliegen. In diesem Fall sind Quelle, Rechte-/Lizenzstatus und Änderungen transparent anzugeben.

---

## Nutzung als Wissens-Upload (Custom GPT / Claude)

Die Dateien in `wissen/` sind so strukturiert, dass sie sich gut als kontextgebende Wissensbasis eignen.

Empfehlung für die Praxis:
- Pro Modul (z. B. Markterkundung) ein eigenes „Wissens-Paket“ aus 1–3 MD-Dateien.
- Klare Überschriftenhierarchie (#, ##, ###).
- Kurze, dichte Absätze (keine Textwüsten).
- Eindeutige Begriffe und Definitionen.
- Optional: Abschnitt „Output-Struktur“, wenn das Modell Antworten standardisiert ausgeben soll.

---

## Verhältnis zu prompts/ und templates/

- **`prompts/`** = Steuerung (Wie soll das Modell arbeiten?)
- **`wissen/`** = Wissen (Welche fachliche Grundlage gilt?)
- **`templates/`** = Output (Welche Muster/Artefakte sollen entstehen?)

*Diese Trennung ist absichtlich: Sie macht das Repo wartbar, auditierbar und in Custom-GPT-Setups gut kombinierbar.*
