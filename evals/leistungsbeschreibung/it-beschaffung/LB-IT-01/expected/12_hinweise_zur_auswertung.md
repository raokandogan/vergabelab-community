---
title: "Testakte LB-IT-01 – Hinweise zur Auswertung"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "evaluation-guide"
eval_role: "expected"
eval_case_id: "LB-IT-01"
predecessor_eval_case_id: "M-IT-01"
relative_date: "T+16 Wochen"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/leistungsbeschreibung/it-beschaffung/LB-IT-01/expected"
module_id: "leistungsbeschreibung-it-beschaffung"
module: "leistungsbeschreibung"
procurement_area: "it-beschaffung"
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

# Aktenstück 12 – Hinweise zur Auswertung

## 1. Zweck

Diese Hinweise unterstützen die Auswertung von Testläufen mit `LB-IT-01`. Sie sind Expected-Material und dürfen bei Blindtests nicht in den zu testenden Assistenten geladen werden.

## 2. Testmodus A – Neuentwurf

Systemkonfiguration:

* regulärer Leistungsbeschreibungs-Systemprompt.

Bereitgestellte Strukturreferenz:

* `templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md`

Input:

* `01_uebergabevermerk_markterkundung.md`
* `02_interne_arbeitsgrundlage_leistungsbeschreibung.md`
* `01_testprompt_neuentwurf_de.md`

Ziel ist zu prüfen, ob der Assistent die im regulären Leistungsbeschreibungs-Systemprompt verankerte Methodik ohne Wiederholung im Testprompt selbstständig anwendet und aus neutralisierten Markterkenntnissen sowie neuen internen Arbeitsentscheidungen eine strukturierte Leistungsbeschreibung entwickelt.

Bewertung:

* Rubric A.

## 3. Testmodus B – Entwurfsprüfung

Systemkonfiguration:

* regulärer Leistungsbeschreibungs-Systemprompt.

Bereitgestellte Strukturreferenz:

* `templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md`

Input:

* `01_uebergabevermerk_markterkundung.md`
* `02_interne_arbeitsgrundlage_leistungsbeschreibung.md`
* `03_entwurf_leistungsbeschreibung_arbeitsfassung.md`
* `02_testprompt_entwurfspruefung_de.md`

Ziel ist zu prüfen, ob der Assistent die im regulären Leistungsbeschreibungs-Systemprompt verankerte Prüfmethodik ohne Aufzählung der erwarteten Fehler im Testprompt selbstständig anwendet und problematische Übernahmen, Widersprüche, Vorfestlegungen sowie falsche Dokumentzuordnungen erkennt.

Bewertung:

* Rubric B.

Die aktuelle Arbeitsfassung enthält bewusst tragfähige und problematische Bestandteile. Bewertet wird nicht die Anzahl gefundener Fehler, sondern die fachliche Richtigkeit, Priorisierung und Differenzierung der Prüfung. Ein Ergebnis ist nicht deshalb besser, weil es möglichst viel streicht oder die Unterlage vollständig neu formuliert. Gute Ergebnisse erhalten belastbare Passagen und ändern nur das Erforderliche.

Bei Testmodus B ist insbesondere zu beachten:

* Vertretbare Grenzfälle dürfen unterschiedlich gelöst werden, wenn die Lösung begründet, transparent und mit Aktenstück 01 und 02 vereinbar ist.
* Bei nicht aktenbelegten Zahlen, Standards und Fristen ist zwischen plausibler Arbeitsannahme und behaupteter abschließender Festlegung zu unterscheiden.
* Dieselbe Schwäche darf nicht mehrfach in verschiedenen Rubric-Bereichen vollständig negativ gewertet werden.
* Die kritische Wiedergabe einer problematischen Passage ist kein KO-Fehler.
* Eine begründete Beibehaltung tragfähiger Passagen ist positiv zu berücksichtigen.
* Testmodus A bleibt von der neuen Arbeitsfassung unberührt, weil Aktenstück 03 dort nicht bereitgestellt wird.

## 4. Regressionstests und Systemvergleiche

Für Regressionstests und Systemvergleiche wird jeweils Testmodus A oder Testmodus B unter vergleichbaren Bedingungen wiederholt. Dabei sollen gleiche Systemprompt-Version, gleiche Template-Version, gleiche Input-Dateien, gleicher Testprompt, gleiches Testprompt-Profil sowie gleiche Tool- und Webkonfiguration verwendet werden. Zusätzliche Nutzerhinweise müssen ebenfalls identisch sein oder vollständig entfallen. Die Bewertung erfolgt mit der zum gewählten Testmodus gehörenden Rubric.

## 5. Trennung von Input und Expected

Bei Blindtests werden nur die benötigten Input- und Prompt-Dateien sowie das Template als Strukturreferenz bereitgestellt. Expected-Dateien und Ergebnisvorlagen bleiben außerhalb des getesteten Systems.

Die Standardtests verwenden die Testprompts unverändert als Minimalprompts. Zusätzliche fachmethodische Hinweise, Prüfkataloge oder Wiederholungen des Systemprompts dürfen im Standardtest nicht ergänzt werden.

Werden solche Hinweise bewusst hinzugefügt, handelt es sich um einen geführten Test. Das Testprompt-Profil und sämtliche zusätzlichen Nutzerhinweise sind dann in der Ergebnisdokumentation festzuhalten. Geführte Tests sind nicht ohne Weiteres mit Standardtests auf Basis der Minimalprompts vergleichbar.

Der Übergabevermerk ist als neues Inputdokument zu behandeln. Er ersetzt keine vollständige Auswertung von `M-IT-01` und darf nicht als authentischer früherer Assistenten-Output bezeichnet werden.

Das Template gehört zur getesteten Modulkonfiguration und darf bereitgestellt werden. Ein Test ohne Template ist zulässig, muss aber ausdrücklich als abweichende Konfiguration dokumentiert werden und ist nicht ohne Weiteres mit einem vollständigen Modultest vergleichbar.

## 6. Hinweise für Custom GPTs

Custom GPTs sollten mit dem regulären Leistungsbeschreibungs-Systemprompt konfiguriert werden. Das Template soll als Strukturreferenz in der Modulkonfiguration oder im Testkontext bereitgestellt werden. Zusätzlich werden nur die für den jeweiligen Testmodus benötigten fallbezogenen Dateien aus `input/` und `prompts/` bereitgestellt. Knowledge-Dateien mit Erwartungshorizont, Rubric oder Auswertungshinweisen würden den Blindtest verfälschen.

## 7. Hinweise für Claude Skills

Bei Claude Skills sollte die Testakte getrennt vom Skill selbst gehalten werden. Der Skill darf im Test nicht auf die Expected-Dateien zugreifen. Ergebnisse werden nachträglich anhand von `10_erwartungshorizont.md` und `11_scoring_rubric.md` bewertet.

## 8. Hinweise für generische LLMs

Bei generischen LLMs ist zu dokumentieren, welche Dateien eingefügt oder hochgeladen wurden, ob Websuche aktiviert war und ob zusätzliche Tools genutzt wurden. Erwartete Bewertungsmaßstäbe dürfen nicht vorab in den Testkontext gelangen.

## 9. Umgang mit zulässigen Strukturabweichungen

Ein Output muss nicht exakt die Struktur des Erwartungshorizonts oder des Templates übernehmen. Zulässig sind abweichende Gliederungen, wenn die Kernanforderungen erfüllt werden: belastbare Herleitung, Neutralisierung, klare Trennung von MUSS- und KANN-Anforderungen, Kandidaten für bewertbare Anforderungen, Optionen und offenen Punkten sowie die Abgrenzung zu anderen Vergabeunterlagen.

## 10. Typische Schwächen

Typische Schwächen sind:

* Übernahme einer Anbieterposition als Mindestanforderung;
* Template wurde trotz Bereitstellung nicht oder nur schematisch verwendet;
* verdeckte Vorprägung durch weitgehende Weiterverwendung von `SchulFach 9` oder herstellergebundene Schnittstellen;
* SaaS-Präferenz oder anderes Betriebsmodell ohne interne Entscheidung oder belastbare Vergleichssystematik;
* unbestimmte Anforderungen wie modern, intuitiv oder schnell;
* historische Migration, Datenbereinigung oder Mitwirkungsleistungen ohne klare Zweck- und Verantwortungsabgrenzung;
* KI-Funktionen, Chatbot oder Mehrsprachigkeit werden nicht als `KANN`, Bewertungskandidat, Option oder spätere Ausbauleistung eingeordnet;
* BundID oder E-Payment werden als verbindliche Umsetzung ohne Klärung von Zeitpunkt, Abrufmechanismus und Vergütung behandelt;
* qualitative Wünsche wurden vorschnell als `KANN` klassifiziert;
* eine Bewertungsabsicht wurde erfunden;
* Kandidaten für bewertbare Anforderungen wurden nicht von konkreten `KANN`-Anforderungen unterschieden;
* Punkte, Gewichtungen oder Kriterienmatrix trotz gegenteiliger Anweisung;
* Vertrags- oder Eignungsinhalte in der Leistungsbeschreibung;
* vorhandene Exit- und Portabilitätsregelungen werden pauschal übersehen oder nicht hinreichend konkretisiert;
* Abnahmefiktion, Vergütungsregelungen oder Nachweise werden nicht der passenden Dokumentebene zugeordnet;
* fehlende Dokumentation offener Punkte.

## 11. Ergebnisdokumentation

Ergebnisse sollen im Ordner `results/` dokumentiert werden. Die Ergebnisvorlage `_result_template.md` enthält die Mindestangaben zu Testdatum, Testmodus, System, Modell, Systemprompt-Version, Testprompt-Version, Testprompt-Profil, Template-Version, Template-Bereitstellung, zusätzlichen Nutzerhinweisen, Repository-Commit, Inputs, ausgeschlossenen Expected-Dateien, Rohantwort, Bewertung nach Rubric A oder B, KO-Fehlern und Fazit.

## 12. Pflegehinweise

Wenn fachlich relevante Grundlagen aus `M-IT-01` geändert werden, muss geprüft werden, ob folgende Dateien noch konsistent sind:

* Übergabevermerk;
* interne Arbeitsgrundlage;
* interne Arbeitsfassung des Entwurfs;
* Erwartungshorizont;
* Scoring Rubric.
