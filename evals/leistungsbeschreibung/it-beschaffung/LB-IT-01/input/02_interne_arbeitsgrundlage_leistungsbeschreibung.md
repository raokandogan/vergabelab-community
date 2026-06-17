---
title: "Testakte LB-IT-01 – Interne Arbeitsgrundlage Leistungsbeschreibung"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "working-basis"
eval_role: "input"
eval_case_id: "LB-IT-01"
predecessor_eval_case_id: "M-IT-01"
relative_date: "T+14 Wochen"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/leistungsbeschreibung/it-beschaffung/LB-IT-01/input"
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

# Aktenstück 02 – Interne Arbeitsgrundlage Leistungsbeschreibung

## 1. Zweck

Diese Arbeitsgrundlage hält den internen Stand bei `T+14 Wochen` fest. Sie dient ausschließlich als Input für die Erstellung oder Prüfung einer Leistungsbeschreibung. Sie ist keine Beschaffungsstrategie, keine Losbildungsentscheidung, keine Wertungsmatrix und keine Vertragsanlage.

## 2. Neue interne Arbeitsentscheidungen der Fortsetzungsakte

Als neue, ausdrücklich gekennzeichnete interne Arbeitsentscheidungen von `LB-IT-01` gelten:

* Die Leistungsbeschreibung soll funktional und produktneutral aufgebaut werden.
* Antragstellung, Nachweis-Upload, Statusinformationen, Sachbearbeitungsworkflow, Rollen- und Rechtefunktionen, Mehrmandantenfähigkeit, Fristensteuerung, Auswertungen und Datenexport sollen grundsätzlich Gegenstand der Beschaffung sein.
* Ein geeigneter Datenaustausch mit `SchulFach 9` soll ermöglicht werden.
* Relevante Dokumente und Metadaten sollen geeignet an `DMS-Nord` beziehungsweise eine spätere E-Akte übergeben werden können.
* Migration laufender Vorgänge und relevanter Stammdaten soll berücksichtigt werden.
* Schulung der Sachbearbeitung, Teamleitungen und Administration soll berücksichtigt werden.
* Betrieb, Wartung, Updates und Support sollen Bestandteil des Leistungsbildes sein.
* Vollautomatisierte ablehnende Entscheidungen sind nicht Gegenstand der ersten Leistungsbeschreibung.

Diese Entscheidungen sind neue Prämissen von `LB-IT-01` und nicht bereits dokumentierte Festlegungen aus `M-IT-01`.

Die bereits in `M-IT-01` dokumentierte Zeitplanung, wonach der Produktivstart zunächst in einer Pilotkommune frühestens ab `T+12 Monaten` und der Rollout auf alle Trägerkommunen frühestens ab `T+18 Monaten` vorgesehen ist, wird unverändert fortgeführt. Offen bleiben der fachliche Umfang der Pilotstufe sowie die Voraussetzungen und Kriterien für den anschließenden Rollout.

## 3. Qualitative Interessen

Die folgenden qualitativen Aspekte werden intern als relevant angesehen:

* Qualität der Konfigurierbarkeit;
* Qualität des Bedien- und Nutzungskonzepts;
* Qualität des Migrations- und Einführungskonzepts;
* Qualität der Datenportabilität und Exit-Unterstützung;
* Qualität der Auswertungsfunktionen;
* Unterstützungs- und Schulungskonzept;
* Qualität der fachlichen Erweiterbarkeit.

Eine weitere Priorisierung und Konkretisierung dieser Aspekte liegt zum Aktenstand nicht vor.

## 4. Weitere Ausbauüberlegungen

Für spätere Ausbaustufen oder zusätzliche Leistungsumfänge werden derzeit folgende Themen diskutiert:

* KI-gestützte Dokumentenklassifikation;
* Textvorschläge für Rückfragen;
* interne Wissensassistenz;
* Bürger-Chatbot;
* vollständige historische Datenmigration;
* BundID-Anbindung;
* E-Payment;
* weitergehende Mehrsprachigkeit;
* Erweiterung auf weitere kommunale Leistungen;
* zusätzliche Fachmodule.

Eine Entscheidung über Aufnahme, Zeitpunkt, Umfang und Beauftragungsform liegt zum Aktenstand nicht vor.

## 5. Weiterhin offene Punkte

* verbindliches Betriebsmodell;
* konkrete Schnittstellenspezifikationen;
* konkrete Daten- und Migrationsmengen;
* Einordnung der Leihgeräteverwaltung in die Ausbaustufen;
* konkrete Rollen und Rechte für Schulen und externe Dienstleister;
* anzuwendender Barrierefreiheitsstandard;
* Prüfverfahren für Barrierefreiheit;
* konkrete Verfügbarkeitswerte;
* konkrete Performancewerte;
* Support- und Reaktionszeiten;
* Wiederherstellungszeiten;
* Lösch- und Aufbewahrungsfristen;
* Umfang der Protokollierung;
* Authentisierungsarchitektur;
* Umfang der ersten Pilotstufe;
* Abgrenzung zwischen Grundleistung und späteren Ausbaustufen;
* Losbildung und Integrationsverantwortung;
* konkrete Vertrags- und EVB-IT-Ausgestaltung.

## 6. Weitere Sachverhaltsklarstellungen

* Für technische Ausgestaltungen, Betriebsmodelle und konkrete Standards liegt keine abschließende interne Entscheidung vor.
* Die in Abschnitt 5 aufgeführten Werte, Spezifikationen und Abgrenzungsfragen sind weiterhin offen.
* Die Leihgeräteverwaltung bleibt Teil des dokumentierten fachlichen Bedarfs. Offen ist nur, ob sie zur ersten Ausbaustufe, zu einer späteren Stufe der Grundleistung oder zu einem gesonderten optionalen Leistungsbestandteil gehört.
