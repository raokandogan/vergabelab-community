---
title: "SPDX- und Metadaten-Policy"
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "policy"
license: "CC-BY-4.0"
repository_area: "POLICIES"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
topics:
  - "SPDX"
  - "Lizenzierung"
  - "YAML-Frontmatter"
  - "Rechtekette"
  - "Quellenangaben"
  - "VergabeLab Community"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# SPDX- und Metadaten-Policy

## 1. Zweck

VergabeLab nutzt pro Datei einheitliche Metadaten und SPDX-Hinweise, damit Lizenz, Rechteinhaberschaft, Quellenstatus und Einordnung der Datei nachvollziehbar bleiben.

Der Standard lautet:

1. YAML-Frontmatter am Anfang der Datei,
2. danach ein SPDX-Kommentar,
3. anschließend der eigentliche Inhalt.

Dadurch bleibt die Datei sowohl für Menschen als auch für spätere Katalogisierung, Website-Sync, Suche oder Automatisierung gut auswertbar.

---

## 2. Grundstruktur je Markdown-Datei

Jede neue oder wesentlich geänderte Markdown-Datei soll am Anfang dieses Muster verwenden:

```md
---
title: "..."
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "..."
license: "CC-BY-4.0"
repository_area: "..."
spdx_file_copyright_text: "2026 Vorname Nachname"
spdx_license_identifier: "CC-BY-4.0"
---

<!--
SPDX-FileCopyrightText: 2026 Vorname Nachname
SPDX-License-Identifier: CC-BY-4.0
-->
```

Für Software-/Tooling-Dateien gilt entsprechend die ausgewiesene Softwarelizenz, z. B.:
```md
---
title: "..."
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "tooling"
license: "EUPL-1.2"
repository_area: "tooling/..."
spdx_file_copyright_text: "2026 Vorname Nachname"
spdx_license_identifier: "EUPL-1.2"
---

<!--
SPDX-FileCopyrightText: 2026 Vorname Nachname
SPDX-License-Identifier: EUPL-1.2
-->
```
---

## 3. Verhältnis von YAML und SPDX-Kommentar

Die YAML-Felder dienen der strukturierten Metadatenpflege, Katalogisierung und späteren technischen Auswertung.

Der SPDX-Kommentar dient als klarer, dateibezogener Lizenz- und Rechtehinweis.

Wenn YAML-Metadaten und SPDX-Kommentar ausnahmsweise voneinander abweichen, ist die Abweichung vor dem Merge zu klären. Die Datei soll erst übernommen werden, wenn Lizenz und Rechteinhaberschaft eindeutig sind.

---
## 4. Pflichtangaben

Jede Markdown-Datei soll mindestens folgende YAML-Felder enthalten:

```md
title: "..."
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "..."
license: "..."
repository_area: "..."
spdx_file_copyright_text: "..."
spdx_license_identifier: "..."
```

Zusätzlich soll unmittelbar darunter ein SPDX-Kommentar stehen:

```md
<!--
SPDX-FileCopyrightText: <Jahr(e)> <Name des Rechteinhabers>
SPDX-License-Identifier: <Lizenz-ID>
-->
```
Zulässige Lizenz-IDs im Projekt sind insbesondere:

```md
CC-BY-4.0
EUPL-1.2
```
---
## 5. Typische Dateitypen

Für ```type``` sollen nach Möglichkeit einheitliche Werte verwendet werden:

```md
type: "root-readme"
type: "folder-readme"
type: "module-readme"
type: "guide"
type: "template"
type: "knowledge"
type: "systemprompt"
type: "policy"
type: "tooling"
```
Beispiele:
```md
type: "guide"
repository_area: "guides"
```

```md
type: "template"
repository_area: "templates/markterkundung/it-beschaffung"
```

```md
type: "knowledge"
repository_area: "wissen/markterkundung"
```

```md
type: "systemprompt"
repository_area: "prompts/markterkundung/it-beschaffung"
```
---

## 6. Wer steht im Copyright?

In den SPDX-Hinweis gehört der tatsächliche Rechteinhaber bzw. die Person oder Organisation, die berechtigt ist, den Beitrag unter der angegebenen Lizenz bereitzustellen.

Beispiele:

```md
<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->
```
Bei mehreren Rechteinhabern oder substantiellen Beiträgen mehrerer Personen sind mehrere Zeilen zulässig:

```md
<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-FileCopyrightText: 2026 Vorname Nachname
SPDX-License-Identifier: CC-BY-4.0
-->
```
Bestehende Copyright-Zeilen dürfen nicht ohne Klärung entfernt werden.

---
## 7. Bearbeitungen

Bei bloßen redaktionellen Korrekturen muss nicht zwingend eine neue Copyright-Zeile ergänzt werden.

Bei substantiellen inhaltlichen Bearbeitungen kann eine zusätzliche Copyright-Zeile ergänzt werden. Bestehende Angaben bleiben erhalten.

Beispiel:

```md
<!--
SPDX-FileCopyrightText: 2025 Okan Doğan
SPDX-FileCopyrightText: 2026 Vorname Nachname
SPDX-License-Identifier: CC-BY-4.0
-->
```

---
## 8. Keine exklusive Rechteübertragung

Durch das Einreichen eines Beitrags werden keine exklusiven Rechte an den Projektträger übertragen. Beiträge folgen dem Prinzip „Inbound = Outbound“: Ein Beitrag wird unter der Lizenz des betroffenen Ordners bzw. der betroffenen Datei veröffentlicht.

---
## 9. Zusicherung der Beitragenden

Mit jedem Beitrag bestätigen Beitragende, dass sie:

- die erforderlichen Rechte am eingereichten Inhalt besitzen oder zur Lizenzierung berechtigt sind,
- keine vertraulichen Informationen, personenbezogenen Daten oder Vergabeinterna einstellen,
- keine Betriebs- und Geschäftsgeheimnisse einstellen,
- keine urheberrechtlich geschützten Volltexte Dritter ohne ausreichende Berechtigung einstellen,
- fremde Inhalte, soweit sie verwendet werden, transparent kennzeichnen.

Pull Requests müssen per DCO signiert werden.

---
##10. Quellenhinweise

Wenn Inhalte auf externen Quellen beruhen, sind diese Quellen transparent anzugeben.

Bei bloßer fachlicher Auswertung, Zusammenfassung oder Einordnung genügt regelmäßig ein sichtbarer Abschnitt am Ende der Datei:

```md
## Quellen

- [Titel der Quelle], [Autor/Herausgeber], [URL], abgerufen am [Datum]. Nutzung: fachliche Auswertung/Zusammenfassung/Zitat, keine Übernahme fremder Textpassagen.
```
Bei Übernahme, Bearbeitung oder Übersetzung fremder Inhalte müssen zusätzlich Rechte- und Lizenzstatus geprüft und angegeben werden.

Beispiel:

## Quellen- und Rechtehinweise

```md
- [Titel], [Autor/Herausgeber], [URL], abgerufen am [Datum]. Lizenz/Rechtestatus: [z. B. CC BY 4.0 / Nutzung mit Zustimmung / amtliches Werk / Zitat]. Änderungen: [gekürzt / zusammengefasst / übersetzt / sprachlich angepasst].
```
Fremde Inhalte dürfen nicht ohne passende Nutzungsrechte unter die VergabeLab-Lizenz gestellt werden.

---
## 11. Quellenangaben in YAML

Zusätzlich zum sichtbaren Quellenabschnitt können Quellen auch im YAML-Frontmatter erfasst werden:

```md
sources:
  - title: "Titel der Quelle"
    url: "https://..."
    author_or_publisher: "..."
    accessed: "2026-05-16"
    usage: "fachliche Auswertung/Zusammenfassung/Zitat, keine Textübernahme"
```
Die sichtbare Quellenangabe im Dokument bleibt bei Wissensbausteinen empfohlen, weil sie für Nutzerinnen und Nutzer unmittelbar nachvollziehbar ist.

---
## 12. Konfliktfall / Korrektur

Wenn Metadaten, SPDX-Kommentar, Lizenzangaben oder Quellenhinweise erkennbar fehlerhaft oder unklar sind, wird der Beitrag vor dem Merge korrigiert oder zurückgestellt, bis die Rechte- und Lizenzlage geklärt ist.

Typische Klärungsfälle:

- falscher Rechteinhaber,
- falsche Lizenz-ID,
- unklare Quelle,
- möglicher Fremdtext ohne Lizenzhinweis,
- personenbezogene Daten,
- Vergabeinterna,
- widersprüchliche YAML- und SPDX-Angaben.
