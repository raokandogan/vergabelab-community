---
title: "Testakte LB-IT-01 – Übergabevermerk Markterkundung"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "handoff-context"
eval_role: "input"
eval_case_id: "LB-IT-01"
predecessor_eval_case_id: "M-IT-01"
relative_date: "T+12 Wochen"
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

# Aktenstück 01 – Übergabevermerk Markterkundung

## 1. Status des Dokuments

Dieser Übergabevermerk ist ein neu erstelltes Inputdokument der Fortsetzungsakte `LB-IT-01`. Er fasst den fiktiven internen Arbeitsstand nach Sichtung der Marktrückläufe aus `M-IT-01` zusammen.

Der Vermerk ist kein authentischer Output eines früher dokumentierten Assistentenlaufs, kein Bestandteil der ursprünglichen Testakte `M-IT-01` und keine Anbieter- oder Beschaffungsentscheidung.

## 2. Ausgangspunkt

Gegenstand bleibt das Vorhaben `SchulServicePortal` des fiktiven Kommunalen Dienstleistungsverbunds Nordtal AöR. Die Markterkundung umfasste vier fiktive Marktteilnehmer, die unterschiedliche Lösungsansätze repräsentieren:

| Lösungsansatz                 | Fiktiver Marktteilnehmer    |
| ----------------------------- | --------------------------- |
| Standardnahes Fachportal      | NordPortal Solutions GmbH   |
| Low-Code-/Workflow-Plattform  | CivicFlow Technologies GmbH |
| Open-Source-nahe Integration  | OpenGov Werkstatt eG        |
| Erweiterung des Altverfahrens | SchulFach Digital GmbH      |

Die Rückmeldung der SchulFach Digital GmbH stammt vom Anbieter des bestehenden Altverfahrens. Bei ihrer Auswertung sind daher mögliche Vorbefassungs-, Abhängigkeits- und Lock-in-Effekte gesondert zu berücksichtigen. Unabhängig davon bleiben alle Marktrückläufe unverbindliche Marktinformationen. Sie sind keine Angebote, technischen Nachweise, Produktfreigaben oder Festlegungen des Auftraggebers.

## 3. Dokumentierter fachlicher Bedarf und bestätigte Zielsetzungen

Die Aktenstücke 01 bis 03 von `M-IT-01` dokumentieren den folgenden fachlichen Bedarf und die damit verbundenen Zielsetzungen:

* digitale Antragstellung für schulbezogene Verwaltungsleistungen;
* Upload und Nachforderung von Nachweisen;
* Statusinformationen für Antragstellende;
* Unterstützung der Sachbearbeitung durch Aufgaben-, Fristen- und Vorgangssteuerung;
* Bescheidvorbereitung auf Basis geprüfter Daten, ohne vollautomatisierte ablehnende Entscheidungen;
* Mehrmandantenfähigkeit für mehrere Trägerkommunen;
* rollen- und rechtebasierte Bearbeitung;
* Auswertungen für Steuerung und Controlling;
* Datenexporte und geeignete Übergabemöglichkeiten;
* nachvollziehbare Erweiterbarkeit und Vermeidung unnötiger Anbieterabhängigkeiten.

Betroffene Leistungen sind insbesondere Schülerbeförderung und Fahrtkostenerstattung, Lernmittelfreiheit beziehungsweise Lernmittelunterstützung, Zuschüsse zur Mittagsverpflegung, Leihgeräteverwaltung, Härtefall- und Einzelfallprüfungen sowie Rückfragen und Nachforderungen. Die endgültige Abgrenzung der ersten Ausbaustufe ist noch offen.

## 4. Nutzergruppen und Mengengerüst

In `M-IT-01` sind folgende Nutzergruppen dokumentiert:

| Nutzergruppe | Angabe aus `M-IT-01` | Datenstand |
|---|---:|---|
| potenzielle Antragstellende | ca. 38.000 | vorläufige Angabe |
| Schulen | 52 | vorläufige Angabe |
| Sachbearbeitung | ca. 90 Mitarbeitende | vorläufige Angabe |
| Teamleitungen | 9 Personen | vorläufige Angabe |
| IT-Administration | 8 Personen | vorläufige Angabe |
| externe Dienstleister | 6 Busunternehmen, 3 Caterer und 1 IT-Dienstleister | vorläufige Angabe; konkrete Einbindung und Rollen offen |

Die Angaben stammen aus `M-IT-01` und sind nicht abschließend validiert.

### Jährliches Fallmengengerüst

`M-IT-01` enthält folgende vorläufige Schätzungen:

| Vorgangsart | Geschätzter Umfang pro Jahr |
|---|---:|
| Schülerbeförderung / Fahrtkostenerstattung | ca. 12.000 Anträge |
| Lernmittelfreiheit | ca. 8.500 Anträge |
| Mittagsverpflegung / Zuschüsse | ca. 6.000 Anträge |
| Leihgeräteverwaltung | ca. 3.500 Vorgänge |
| Härtefall- und Einzelfallprüfungen | ca. 900 Vorgänge |
| Rückfragen / Nachforderungen | ca. 18.000 Kommunikationsvorgänge |

Auch diese Angaben sind Schätzungen und noch nicht abschließend validiert.

## 5. In der Gesamtschau der Marktrückläufe gestützte Erkenntnisse

Aus der Gesamtschau mehrerer Rückmeldungen lassen sich folgende vorläufige Erkenntnisse ableiten:

* Es bestehen mehrere marktgängige Lösungsansätze; kein Ansatz ist allein durch die Markterkundung festgelegt.
* Digitale Antragstellung, Nachweisupload, Statusanzeige, Workflowfunktionen, Rollenmodelle und Auswertungen sind grundsätzlich marktüblich oder realisierbar.
* Schnittstellen, Datenaustausch, Migration und Auftraggebermitwirkung sind zentrale Kosten- und Risikotreiber.
* Unterschiedliche Betriebsmodelle sind verfügbar, darunter SaaS, Private Cloud, kommunales oder öffentliches Rechenzentrum, Managed Hosting, Auftraggeberumgebung und On-Premises.
* Datenportabilität, Exportfähigkeit und Exit-Unterstützung sind wegen Lock-in-Risiken relevant.
* Die Marktrückläufe enthalten zur Barrierefreiheit überwiegend allgemeine Zusicherungen; konkrete Standards und Prüfverfahren lassen sich daraus nicht ableiten.
* KI-Funktionen werden am Markt als Assistenzfunktionen beschrieben, sind aber nicht als zwingender Kern der ersten Ausbaustufe bestätigt.

Diese Erkenntnisse ersetzen keine interne Bedarfsentscheidung und keine spätere technische Spezifikation.

## 6. Aussagen aus einzelnen Marktrückläufen

Die folgenden Aussagen beruhen jeweils auf einzelnen Marktrückläufen. Sie wurden nicht als interne Anforderungen oder Entscheidungen übernommen:

* die Einschätzung, ein bestimmtes Standardprodukt decke 60 bis 75 Prozent der Anforderungen ab;
* die Empfehlung, eine Low-Code-Plattform nicht zu stark fachportalbezogen auszuschreiben;
* die Empfehlung, mit zwei oder drei priorisierten Leistungen zu starten;
* die Aussage des Altanbieters, die Erweiterung von `SchulFach 9` sei der schnellste und risikoärmste Weg;
* anbieterspezifische Kostenkorridore, Einführungszeiten und Lizenzlogiken;
* Empfehlungen einzelner Marktteilnehmer für oder gegen eine Gesamtvergabe;
* proprietäre Schnittstellen oder plattformeigene Exportformate;
* Anbieterangaben zu Zertifizierungen, Referenzen und Standardabdeckungen.

## 7. Interner Entscheidungsstand der Fortsetzungsakte

Bei `T+12 Wochen` wurden für die Fortsetzungsakte folgende interne Arbeitsstände festgehalten:

* Die Leistungsbeschreibung soll zunächst funktional und produktneutral aufgebaut werden.
* Eine Festlegung auf ein bestimmtes Produkt, einen Hersteller, eine Technologie oder ein Betriebsmodell wurde nicht getroffen.
* Über die spätere Einordnung einzelner Anforderungen als Mindestanforderung, bewertbare Anforderung oder optionaler Leistungsbestandteil wurde noch nicht abschließend entschieden.
* Aussagen aus den Marktrückläufen wurden bislang nicht als Auftraggeberanforderungen übernommen.

Diese Arbeitsstände wurden erstmals für `LB-IT-01` dokumentiert und sind keine bereits in `M-IT-01` enthaltenen Entscheidungen.

Die bereits in `M-IT-01` dokumentierte zeitliche Rahmenannahme, wonach ein Vergabeverfahren frühestens bei `T+20 Wochen` beginnen kann, wird unverändert fortgeführt.

## 8. Schnittstellen und Datenaustausch

Für `SchulFach 9` wird ein geeigneter, möglichst medienbrucharmer Datenaustausch benötigt. Ob dieser über eine direkte Schnittstelle, standardisierte Exporte und Importe oder eine andere Integrationsform erfolgt, ist noch festzulegen.

Für `DMS-Nord` beziehungsweise eine spätere E-Akte wird eine geeignete Übergabe und Ablage relevanter Dokumente und Metadaten benötigt. Die konkrete Architektur und der erforderliche Automatisierungsgrad sind offen.

Der Formularserver des Landesportals ist zu berücksichtigen; seine produktive technische Einbindung ist nicht abschließend geklärt. Der kommunale Identity Provider unterstützt SAML/OIDC, die Authentisierungsarchitektur ist aber noch festzulegen. BundID ist perspektivisch geplant, zum Aktenstand aber nicht als zwingende Startanforderung bestätigt. E-Payment befindet sich im Pilot- beziehungsweise Klärungsstatus.

Anbieterangaben zu REST, SOAP, CSV, XML, JSON, OIDC, SAML, proprietären APIs oder Adapterentwicklungen sind Marktinformationen und keine festgelegten technischen Anforderungen.

## 9. Offene fachliche, technische und organisatorische Punkte

Offen bleiben insbesondere:

* verbindliches Betriebsmodell;
* konkrete Schnittstellenspezifikationen;
* konkrete Daten- und Migrationsmengen;
* Einordnung der Leihgeräteverwaltung in die Ausbaustufen;
* konkrete Rollen und Rechte für Schulen und externe Dienstleister;
* anzuwendender Barrierefreiheitsstandard und Prüfverfahren;
* Verfügbarkeits-, Performance-, Support- und Wiederherstellungswerte;
* Lösch- und Aufbewahrungsfristen;
* Umfang der Protokollierung;
* Umfang der ersten Pilotstufe;
* Losbildung und Integrationsverantwortung;
* konkrete Vertrags- und EVB-IT-Ausgestaltung.

## 10. Noch auszuarbeitende fachliche und technische Themen

Für die weitere Vorbereitung sind insbesondere noch zu konkretisieren:

* fachlicher Umfang der ersten Ausbaustufe;
* funktionaler Umfang von Antragstellung, Nachweisbearbeitung, Vorgangssteuerung, Fristen, Statusinformationen und Bescheidvorbereitung;
* Anforderungen an Mehrmandantenfähigkeit sowie an Rollen und Rechte;
* erforderliche Datenschutz- und Sicherheitsfunktionen;
* Datenexport, Datenportabilität und Exit-Unterstützung;
* Umfang, Datenarten und Mitwirkungsleistungen für die Migration laufender Vorgänge und relevanter Stammdaten;
* Umfang und Abgrenzung von Schulung, Einführung, Betrieb, Wartung, Updates und Support.

## 11. Nicht getroffene Festlegungen

Zum Aktenstand wurden insbesondere folgende Festlegungen nicht getroffen:

* Auswahl oder Bevorzugung eines Marktteilnehmers;
* Erweiterung von `SchulFach 9` als Zielarchitektur;
* Low-Code, Open Source, Standardfachportal, SaaS oder On-Premises als alleiniger Lösungsweg;
* proprietäre Schnittstellen als zwingende Vorgabe;
* vollständige historische Migration;
* KI-Dokumentenklassifikation oder Chatbot als zwingende Grundleistung;
* BundID, E-Payment oder Mehrsprachigkeit als zwingende Startanforderung;
* abschließende Losbildungs-, Betriebsmodell- oder Verfahrensentscheidung.
