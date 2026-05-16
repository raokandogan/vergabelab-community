---
title: "README – Markterkundung IT-Beschaffung"
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "module-readme"
license: "CC-BY-4.0"
repository_area: "prompts/markterkundung/it-beschaffung"
module: "markterkundung"
procurement_area: "it-beschaffung"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
target_audience:
  - "Community-Mitwirkende"
  - "Vergabestellen"
  - "öffentliche Auftraggeber"
  - "Vergabepraktiker"
topics:
  - "Markterkundung"
  - "IT-Beschaffung"
  - "Readme"
  - "Hinweise"
  
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->
*VergabeLab Community – Wissensbaustein (Stand: Mai 2026) • © Okan Doğan • Lizenz: CC BY 4.0*

# Markterkundung IT-Beschaffung

Dieser Ordner enthält Hinweis- und Systemprompt-Bausteine für KI-Expertensysteme, die öffentliche Auftraggeber und Vergabestellen bei der **Vorbereitung, Durchführung und Auswertung von Markterkundungen** unterstützen.

Der Schwerpunkt liegt auf vergaberechtlichen Markterkundungen nach **§ 28 VgV** sowie – unterhalb der EU-Schwellenwerte – **§ 20 UVgO**. Die Bausteine sind besonders auf IT-Beschaffungen ausgerichtet, etwa Software, Hardware, Cloud-/SaaS-Leistungen, Schnittstellen, Datenschutz, IT-Sicherheit, Betrieb, Migration, SLAs und Lizenzmodelle.

Die Bausteine dienen der Strukturierung und Qualitätssicherung. Sie ersetzen keine Rechtsberatung im Einzelfall und automatisieren keine Vergabeentscheidung.

---

## Dateien in diesem Ordner

| Datei | Zweck | Einsatz |
|---|---|---|
| `01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md` | Hinweistext/Systemprompt für einen Markterkundungs-GPT | ChatGPT Custom GPT |

Weitere Varianten, etwa für Claude Projects oder andere KI-Systeme, können später ergänzt werden.

---

## Schnellstart

1. Öffne die Datei `01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md`.
2. Kopiere nur den Abschnitt zwischen **„KOPIERBEREICH START“** und **„KOPIERBEREICH ENDE“**.
3. Füge den kopierten Text in das Feld **„Hinweise“** bzw. **„Instructions“** deines Custom GPT ein.
4. Ergänze bei Bedarf projektspezifische Rahmenbedingungen, etwa Bundesland, interne Vorgaben, Verwaltungsvorschriften oder besondere IT-/Sicherheitsanforderungen.
5. Teste den Assistenten mit einem einfachen Einstieg, zum Beispiel:

```text
Wir planen die Beschaffung einer Softwarelösung und möchten vorab eine Markterkundung durchführen. Bitte stelle mir die erforderlichen Rückfragen.
```

---

## Erwartete Arbeitsweise des Assistenten

Der Assistent arbeitet nach dem Prinzip:

> **Ask first, then draft.**

Das bedeutet: Bei unvollständigen Angaben soll der Assistent zunächst strukturierte Rückfragen stellen und nicht sofort vollständige Entwürfe erzeugen. Vollentwürfe, etwa Anschreiben, Fragenkataloge oder Auswertungsmatrizen, sollen erst erstellt werden, wenn der Sachverhalt hinreichend geklärt ist oder der Nutzer ausdrücklich einen Schnellstart wünscht.

Der Prompt enthält hierfür einen Gatekeeper mit zehn Pflichtangaben, unter anderem:

- Auftraggeber und Organisationseinheit,
- Leistungsbild,
- Schwellenwert-/Auftragswertkontext,
- Zeitplan,
- Stakeholder,
- Datenschutz- und Sicherheitsanforderungen,
- Schnittstellen,
- Betriebsmodell,
- Bestandssysteme und Migrationsbedarf,
- Budget- und Lizenzmodellannahmen.

---

## Typische Outputs

Der Markterkundungs-Assistent kann insbesondere folgende Arbeitsprodukte vorbereiten:

- strukturierte Rückfragen an den Auftraggeber,
- Zweck- und Dokumentationsvermerke zur Markterkundung,
- Musteranschreiben an Anbieter,
- Anbieter-Fragenkataloge,
- E-Mail-Entwürfe,
- Auswertungsmatrizen,
- Variantenvergleiche, etwa SaaS vs. On-Prem,
- Risikolisten für Leistungsbeschreibung, Auftragswert, Losbildung und Verfahrenswahl,
- Hinweise zur Neutralisierung von Vorbefassung.

---

## Vergaberechtliche Leitplanken

Bei der Nutzung ist insbesondere zu beachten:

- Markterkundungen dürfen nicht als Scheinausschreibungen oder verdeckte Preisabfragen ohne Beschaffungsabsicht genutzt werden.
- Gleichbehandlung, Transparenz und Wettbewerbsgrundsätze sind zu beachten.
- Anbieter sollten grundsätzlich identische Informationen erhalten, soweit dies für einen fairen Erkenntnisgewinn erforderlich ist.
- Vorbefasste Unternehmen sind nicht pauschal auszuschließen; ein möglicher Wissensvorsprung ist sachgerecht zu neutralisieren.
- Zweck, Auswahl der angesprochenen Unternehmen, Kommunikation, Unterlagen und Auswertung sollten dokumentiert werden.

Die Verantwortung für rechtliche Bewertung, Verfahrensgestaltung und Vergabeentscheidung bleibt immer beim Menschen.

---

## Datenschutz und Vertraulichkeit

Bitte keine personenbezogenen Daten, Betriebs- und Geschäftsgeheimnisse oder Details laufender Vergaben in öffentliche Systeme oder öffentliche Beiträge einfügen.

Für Tests und Community-Beiträge sollten Beispiele abstrahiert und anonymisiert werden, etwa mit Platzhaltern wie `[Auftraggeber]`, `[Projekt]`, `[Fachverfahren]`, `[Anbieter A]`.

---

## Hinweise für Beiträge

Verbesserungen sind willkommen, insbesondere:

- präzisere Rückfragen,
- bessere Struktur für IT-Markterkundungen,
- zusätzliche typische Schnittstellen oder Sicherheitsanforderungen,
- praxistaugliche Auswertungslogiken,
- Hinweise auf vergaberechtliche Risiken,
- bessere Formulierungen für Anschreiben oder Fragenkataloge.

Bitte beachte bei Beiträgen die allgemeinen Regeln in `CONTRIBUTING.md`, insbesondere:

- keine personenbezogenen Daten,
- keine vertraulichen Vergabeinformationen,
- keine fremden Texte ohne entsprechende Rechte,
- DCO-Sign-off für Pull Requests.

---

## Lizenz

Die Dateien in diesem Ordner stehen – soweit in der jeweiligen Datei nicht anders gekennzeichnet – unter **CC BY 4.0**.

Bitte beachte die jeweiligen SPDX- und Lizenzhinweise in den Dateien. Maßgeblich ist immer der konkrete Lizenzhinweis der jeweiligen Datei.
