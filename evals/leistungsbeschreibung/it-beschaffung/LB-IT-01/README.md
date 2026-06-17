---
title: "Testakte LB-IT-01 – Leistungsbeschreibung SchulServicePortal"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "case-readme"
eval_role: "documentation"
eval_case_id: "LB-IT-01"
predecessor_eval_case_id: "M-IT-01"
relative_date: "T+14 Wochen"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/leistungsbeschreibung/it-beschaffung/LB-IT-01"
module_id: "leistungsbeschreibung-it-beschaffung"
module: "leistungsbeschreibung"
procurement_area: "it-beschaffung"
related_systemprompt: "prompts/leistungsbeschreibung/it-beschaffung/01_hinweistext_systemprompt_leistungsbeschreibung_it_de.md"
related_template: "templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md"
target_systems:
  - "chatgpt-custom-gpt"
  - "claude-skill"
  - "generic-llm"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# Testakte LB-IT-01

`LB-IT-01` prüft, ob ein Leistungsbeschreibungs-Assistent neutralisierte Ergebnisse einer Markterkundung in einen strukturierten Erstentwurf einer Leistungsbeschreibung überführen und einen problematischen Entwurf fachlich prüfen kann.

Die Testakte ist eine fiktive, aktenkonsistente Fortsetzung von [`M-IT-01`](../../../markterkundung/it-beschaffung/M-IT-01/). Gegenstand bleibt das Vorhaben `SchulServicePortal` des fiktiven Auftraggebers Kommunaler Dienstleistungsverbund Nordtal AöR.

## Methodische Einordnung

Der Übergabevermerk in `input/01_uebergabevermerk_markterkundung.md` ist ein neues Inputdokument dieser Fortsetzungsakte. Er ist kein tatsächlich dokumentierter früherer Assistenten-Output, kein Bestandteil der ursprünglichen Testakte `M-IT-01` und kein Nachweis einer real durchgeführten Marktauswertung.

Die Aktenstücke 01 bis 09 aus `M-IT-01` bilden die Sachverhaltsgrundlage. Die dortigen Expected-Dateien dienen nur als fachliche Kontrollgrundlage für die Erstellung und Auswertung dieser Fortsetzungsakte. Der dokumentierte Testlauf in `M-IT-01/results/` betrifft die Vorbereitung der Markterkundung mit Aktenstücken 01 bis 05 und nicht die Auswertung der Marktrückläufe 06 bis 09.

## Zeitliche Einordnung

| Zeitpunkt | Bedeutung |
|---|---|
| `T+10 Wochen` | fiktive Auswertung der Marktrückläufe aus `M-IT-01` |
| `T+12 Wochen` | interne Sichtung und Vorbereitung erster Eckpunkte |
| `T+14 Wochen` | Start der Fortsetzungsakte `LB-IT-01` zur Leistungsbeschreibung |
| `T+15 Wochen` | problematischer interner Entwurf der Leistungsbeschreibung |
| `T+16 Wochen` | interne Expected- und Bewertungsmaterialien |
| `T+20 Wochen` | frühestmöglicher Beginn eines Vergabeverfahrens |
| `T+36 Wochen` | frühestmöglicher Zuschlag nach der in `M-IT-01` dokumentierten Zeitplanung |

## Testziel

Die Testakte untersucht insbesondere, ob ein Assistent:

* Markterkenntnisse nach Belastbarkeit einordnet;
* einzelne Anbieterpositionen nicht zu Auftraggeberanforderungen erhebt;
* funktionale Anforderungen produkt- und herstellerneutral formuliert;
* Grundleistung, belastbar begründbare Mindestanforderungen (`MUSS`), hinreichend konkretisierbare bewertbare Anforderungen (`KANN`), Kandidaten für bewertbare Anforderungen, Optionen und offene Punkte trennt;
* keine Kriterienmatrix, Punkte oder Gewichtungen erfindet;
* keine Entscheidung über Betriebsmodell, Losbildung oder Verfahrensart trifft;
* Leistungsbeschreibung, Wertung, Eignung, Vertrag und gesonderte Anlagen auseinanderhält.

## Verwendete Kategorien

* **MUSS:** zwingend erforderliche und überprüfbare Mindestanforderung.
* **KANN:** nicht zwingende qualitative Anforderung, die später bewertet werden kann.
* **Qualitatives Interesse beziehungsweise Bewertungskandidat:** fachlich relevanter Aspekt, dessen Bewertungsabsicht oder Maßstab noch nicht ausreichend feststeht.
* **Option oder spätere Ausbaustufe:** zusätzlicher Leistungsbestandteil, dessen Aufnahme, Zeitpunkt oder Beauftragung noch nicht abschließend entschieden ist.

## Verzeichnisstruktur

```text
LB-IT-01/
  README.md
  input/
    01_uebergabevermerk_markterkundung.md
    02_interne_arbeitsgrundlage_leistungsbeschreibung.md
    03_entwurf_leistungsbeschreibung_arbeitsfassung.md
  prompts/
    01_testprompt_neuentwurf_de.md
    02_testprompt_entwurfspruefung_de.md
  expected/
    10_erwartungshorizont.md
    11_scoring_rubric.md
    12_hinweise_zur_auswertung.md
  results/
    _result_template.md
```

## Blindtest-Trennung

Für einen Blindtest dürfen nur die jeweils benötigten Dateien aus `input/` und `prompts/` sowie das Leistungsbeschreibung-Template als Strukturreferenz bereitgestellt werden. Die Dateien unter `expected/` und `results/` dürfen während des Testlaufs nicht als Input verwendet werden.

Für den Standardtest werden die Testprompts unverändert verwendet und nicht durch zusätzliche fachmethodische Nutzerhinweise ergänzt.

Die vollständigen Marktteilnehmerantworten aus `M-IT-01` müssen dem Leistungsbeschreibungs-Assistenten nicht zwingend bereitgestellt werden, weil `LB-IT-01` mit einem neu erstellten, neutralisierten Übergabevermerk arbeitet. Wird zusätzlich auf `M-IT-01` zurückgegriffen, ist zu dokumentieren, welche Aktenstücke bereitgestellt wurden.

Das Template darf und soll bei den vorgesehenen Modul-Tests bereitgestellt werden. Seine konkrete Version und die Art der Bereitstellung müssen in der Ergebnisdatei dokumentiert werden. Falls bewusst ein Test ohne Template erfolgt, ist dies als abweichende Testkonfiguration zu kennzeichnen.

## Getestete Modulbestandteile

Die Testakte prüft das Zusammenwirken folgender Modulbestandteile:

* Systemprompt: [`prompts/leistungsbeschreibung/it-beschaffung/01_hinweistext_systemprompt_leistungsbeschreibung_it_de.md`](../../../../prompts/leistungsbeschreibung/it-beschaffung/01_hinweistext_systemprompt_leistungsbeschreibung_it_de.md)
* Template: [`templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md`](../../../../templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md)

Der Systemprompt wird als Systemkonfiguration des getesteten Assistenten verwendet. Das Template wird als Struktur- und Arbeitsreferenz bereitgestellt. Die Dateien aus `input/` liefern den konkreten Sachverhalt; die Dateien aus `prompts/` enthalten den jeweiligen Testauftrag.

Die Testprompts sind bewusst knapp gehalten. Die fachmethodischen Leitplanken für Neutralisierung, Anforderungssystematik, Dokumentabgrenzung und den Umgang mit offenen Punkten sollen aus dem Systemprompt und dem Template stammen. Zusätzliche methodische Hinweise im Testprompt bilden eine geführte Testkonfiguration und müssen als solche dokumentiert werden; ihre Ergebnisse sind nicht ohne Weiteres mit den Standardtests vergleichbar.

Die Expected-Dateien und die Ergebnisvorlage bleiben während eines Blindtests außerhalb des getesteten Systems.

## Referenzen im Repository

* Systemprompt Leistungsbeschreibung: [`prompts/leistungsbeschreibung/it-beschaffung/01_hinweistext_systemprompt_leistungsbeschreibung_it_de.md`](../../../../prompts/leistungsbeschreibung/it-beschaffung/01_hinweistext_systemprompt_leistungsbeschreibung_it_de.md)
* Template Leistungsbeschreibung: [`templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md`](../../../../templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md)
