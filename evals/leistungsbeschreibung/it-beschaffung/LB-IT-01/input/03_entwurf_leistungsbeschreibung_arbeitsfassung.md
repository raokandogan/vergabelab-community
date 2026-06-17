---
title: "Testakte LB-IT-01 – Entwurf Leistungsbeschreibung, interne Arbeitsfassung"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "working-draft"
eval_role: "input"
eval_case_id: "LB-IT-01"
predecessor_eval_case_id: "M-IT-01"
relative_date: "T+15 Wochen"
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

# Aktenstück 03 – Entwurf Leistungsbeschreibung, interne Arbeitsfassung

## 1. Gegenstand und Zielsetzung

Der Kommunale Dienstleistungsverbund Nordtal AöR beabsichtigt, für das Vorhaben `SchulServicePortal` eine integrierte Portal- und Vorgangsbearbeitungslösung einzuführen. Die Lösung soll die digitale Antragstellung, die fachliche Bearbeitung, die Kommunikation mit Antragstellenden sowie die Übergabe von Dokumenten und Vorgangsdaten an bestehende Systeme unterstützen.

Gegenstand der Beschaffung sind insbesondere:

* Bereitstellung und Einführung der Portallösung;
* Konfiguration der fachlichen Prozesse;
* Anbindung der vorhandenen Systemlandschaft;
* Migration der für die Bearbeitung benötigten Daten;
* Schulung und Einführungsunterstützung;
* Betrieb, Wartung und Support;
* Unterstützung bei Datenschutz und Informationssicherheit.

Der Auftragnehmer soll die Gesamtverantwortung für die technische Funktionsfähigkeit der Lösung einschließlich der erforderlichen Schnittstellen übernehmen. Leistungen anderer Systemanbieter sind durch den Auftragnehmer zu koordinieren, soweit dies für eine durchgängige Lösung erforderlich ist.

Die vorhandenen Funktionen, Datenstrukturen und Rollenmodelle von `SchulFach 9` sollen möglichst weitgehend weiterverwendet werden. Dadurch sollen Umstellungsaufwand, Migrationsrisiken und zusätzlicher Pflegeaufwand begrenzt werden.

## 2. Fachlicher Leistungsumfang

Die Lösung muss mindestens folgende Leistungen unterstützen:

1. Schülerbeförderung und Fahrtkostenerstattung;
2. Lernmittelfreiheit beziehungsweise Lernmittelunterstützung;
3. Zuschüsse zur Mittagsverpflegung;
4. Härtefall- und Einzelfallprüfungen;
5. Leihgeräteverwaltung, soweit hierfür ein standardmäßig verfügbares Modul eingesetzt werden kann.

Für die erste Produktivstufe sind die Leistungen nach den Nummern 1 bis 3 vorgesehen. Weitere Leistungen sollen ohne grundlegenden Systemwechsel ergänzt werden können.

Die Portallösung muss insbesondere ermöglichen:

* digitale Antragstellung und strukturierte Erfassung der erforderlichen Angaben;
* Upload und Zuordnung von Nachweisen;
* Plausibilitäts- und Vollständigkeitsprüfungen;
* Nachforderung fehlender Unterlagen;
* Statusinformationen für Antragstellende;
* Kommunikation zwischen Antragstellenden und Sachbearbeitung;
* Vorbereitung fachlicher Entscheidungen und Bescheide;
* Weitergabe von Dokumenten an `DMS-Nord`;
* Austausch relevanter Vorgangsdaten mit `SchulFach 9`;
* Protokollierung wesentlicher Bearbeitungs- und Kommunikationsschritte;
* rollenbezogene Auswertungen und Berichte.

Eine automatisierte Ablehnung oder sonstige abschließende negative Entscheidung darf nicht allein durch das System erfolgen.

## 3. Lösungs- und Betriebsmodell

Bevorzugt wird eine vom Auftragnehmer betriebene und regelmäßig aktualisierte Lösung. Ein SaaS-Modell erscheint nach der bisherigen Marktsichtung grundsätzlich geeignet.

Alternativ können andere Betriebsmodelle angeboten werden, sofern sie hinsichtlich Verfügbarkeit, Informationssicherheit, Datenschutz, Skalierbarkeit, Aktualisierbarkeit und Gesamtbetrieb mindestens gleichwertig sind. Der Auftragnehmer hat die Gleichwertigkeit in seinem Lösungskonzept nachvollziehbar darzustellen.

Personenbezogene Daten sind innerhalb der Europäischen Union oder des Europäischen Wirtschaftsraums zu verarbeiten. Administrations- oder Supportzugriffe aus Drittstaaten sind grundsätzlich auszuschließen.

Für Test-, Schulungs- und Abnahmezwecke soll eine vom Produktivsystem getrennte Umgebung bereitgestellt werden. Soweit erforderlich, muss diese Umgebung auch innerhalb der Infrastruktur des Auftraggebers betrieben werden können.

Die Lösung muss für mindestens 38.000 potenzielle Antragstellende und rund 90 Beschäftigte der Sachbearbeitung skalierbar sein. Eine spätere Erweiterung auf weitere kommunale Leistungen darf keinen grundlegenden Austausch der technischen Plattform erfordern.

## 4. Einbindung der bestehenden Systemlandschaft

### 4.1 Fachverfahren `SchulFach 9`

Die Lösung muss einen medienbrucharmen Datenaustausch mit `SchulFach 9` ermöglichen. Hierzu sollen die vom Hersteller des Fachverfahrens vorgesehenen Standardschnittstellen und vorhandenen Rollen- und Datenstrukturen genutzt werden.

Mindestens folgende Informationen müssen ausgetauscht werden können:

* Vorgangs- und Statusdaten;
* Identifikations- und Zuordnungsmerkmale;
* entscheidungsrelevante Fachdaten;
* Bescheid- und Zahlungsinformationen;
* Verweise auf zugehörige Dokumente.

Eine doppelte Pflege fachlich identischer Informationen soll vermieden werden. Welche Daten in welchem System führend gehalten werden, wird im Feinkonzept festgelegt.

Falls einzelne Schnittstellenfunktionen zum Zeitpunkt der Angebotsabgabe noch nicht verfügbar sind, hat der Auftragnehmer eine technisch gleichwertige Übergangslösung anzubieten. Die endgültigen Schnittstellenspezifikationen werden nach Zuschlag gemeinsam mit dem Auftraggeber und den beteiligten Systemanbietern abgestimmt.

### 4.2 Dokumentenmanagementsystem `DMS-Nord`

Antragsunterlagen, Nachforderungen, eingehende Nachweise und erzeugte Bescheide müssen automatisiert an `DMS-Nord` übergeben werden können.

Dokumente sollen aus dem Portal beziehungsweise aus der Vorgangsbearbeitung heraus aufgerufen werden können, ohne dass Nutzerinnen und Nutzer das jeweils führende System wechseln müssen. Die technische Umsetzung kann über direkte Schnittstellen, dokumentierte Übergabedienste oder eine vergleichbare Integration erfolgen.

### 4.3 Weitere Dienste

Die Lösung soll für die Einbindung des vorhandenen Identity Providers, des Formularservers sowie perspektivisch von BundID und E-Payment vorbereitet sein.

BundID und E-Payment müssen spätestens während der Vertragslaufzeit ohne grundlegende Änderung der Systemarchitektur integriert werden können. Über den Zeitpunkt der produktiven Aktivierung entscheidet der Auftraggeber im Projektverlauf.

## 5. Funktionale und qualitative Anforderungen

| ID   | Status | Anforderung                                                                                                            | Nachweis beziehungsweise Hinweis                 |
| ---- | ------ | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ |
| F-01 | MUSS   | Antragstellende können Anträge vollständig digital einreichen und Nachweise hochladen.                                 | Darstellung im Lösungskonzept                    |
| F-02 | MUSS   | Die Sachbearbeitung kann unvollständige Anträge erkennen und Unterlagen strukturiert nachfordern.                      | Test im Pilotbetrieb                             |
| F-03 | MUSS   | Der aktuelle Bearbeitungsstand wird für berechtigte Nutzergruppen transparent dargestellt.                             | Rollenabhängige Darstellung                      |
| F-04 | MUSS   | Die Lösung unterstützt eine medienbrucharme Übergabe relevanter Daten an `SchulFach 9`.                                | Beschreibung der vorgesehenen Schnittstelle      |
| F-05 | MUSS   | Dokumente werden automatisiert an `DMS-Nord` übergeben und dem jeweiligen Vorgang zugeordnet.                          | Schnittstellenkonzept                            |
| F-06 | MUSS   | Das bestehende Rollenmodell von `SchulFach 9` kann übernommen oder ohne zusätzlichen Pflegeaufwand abgebildet werden.  | Beschreibung im Rollen- und Berechtigungskonzept |
| F-07 | KANN   | Eingehende Dokumente können automatisiert erkannt, klassifiziert und dem passenden Vorgang zugeordnet werden.          | Funktionsbeschreibung und Demonstration          |
| F-08 | KANN   | Die Lösung stellt einen digitalen Assistenten zur Beantwortung wiederkehrender Fragen bereit.                          | Beschreibung vorhandener Standardfunktion        |
| F-09 | MUSS   | Standardseiten und Standardvorgänge reagieren unter normalen Betriebsbedingungen innerhalb von zwei Sekunden.          | Messung im Abnahmetest                           |
| F-10 | MUSS   | Die Lösung unterstützt eine vollständig barrierefreie Nutzung durch Antragstellende und Beschäftigte.                  | Eigenerklärung und Prüfbericht                   |
| F-11 | SOLL   | Oberflächen, Texte und Bearbeitungsschritte sind intuitiv, modern und ohne besondere technische Vorkenntnisse nutzbar. | Bewertung anhand der Präsentation                |
| F-12 | KANN   | Die Benutzeroberfläche kann zusätzlich in mehreren Sprachen bereitgestellt werden.                                     | Angabe unterstützter Sprachen                    |
| F-13 | MUSS   | Die Lösung ist für eine spätere Einbindung weiterer kommunaler Leistungen geeignet.                                    | Darstellung von Erweiterungsmöglichkeiten        |
| F-14 | KANN   | Für die Leihgeräteverwaltung steht ein bereits produktiv eingesetztes Standardmodul zur Verfügung.                     | Funktionsbeschreibung und Referenz               |
| F-15 | MUSS   | Der Auftragnehmer verfügt über mindestens drei Referenzen für vergleichbare Portallösungen im kommunalen Umfeld.       | Referenzliste mit Angebotsabgabe                 |

Anforderungen mit dem Status `KANN` können bei der späteren Angebotswertung berücksichtigt werden. Einzelheiten zur Gewichtung werden in der Bewertungsmatrix festgelegt.

## 6. Nutzergruppen und Berechtigungen

Die Lösung muss mindestens folgende Nutzergruppen abbilden:

* Antragstellende und gegebenenfalls Sorgeberechtigte;
* Beschäftigte der Sachbearbeitung;
* Teamleitungen;
* IT-Administration;
* Schulen;
* beteiligte externe Dienstleister.

Antragstellende erhalten ausschließlich Zugriff auf die eigenen Anträge, Nachrichten, Nachweise und Statusinformationen.

Beschäftigte der Sachbearbeitung und Teamleitungen erhalten rollen- und aufgabenbezogene Zugriffe. Teamleitungen benötigen zusätzlich Auswertungs-, Vertretungs- und Steuerungsfunktionen.

Schulen sollen die Anträge und Bearbeitungsstände der ihrer Schule zugeordneten Schülerinnen und Schüler einsehen können, soweit dies zur Bestätigung schulbezogener Angaben, zur Bearbeitung von Rückfragen oder zur Unterstützung der Antragstellenden erforderlich ist.

Externe Dienstleister, insbesondere Busunternehmen und Caterer, sollen auf die für die Leistungserbringung notwendigen Vorgangs-, Kontakt- und Abrechnungsdaten zugreifen können. Der konkrete Datenumfang und die erforderlichen Bearbeitungsrechte werden im Berechtigungskonzept festgelegt.

Das Rollen- und Berechtigungskonzept ist im Feinkonzept gemeinsam mit dem Auftraggeber auszuarbeiten. Standardrollen der angebotenen Lösung sollen möglichst verwendet werden.

## 7. Migration

Für die Produktivsetzung müssen sämtliche laufenden Vorgänge einschließlich der dazugehörigen Stammdaten, Dokumente, Kommunikationsstände und Bearbeitungsinformationen übernommen werden.

Darüber hinaus sind historische Vorgänge zu migrieren, soweit sie für:

* die vollständige Vorgangshistorie;
* Rückfragen und Wiederholungsanträge;
* gesetzliche Aufbewahrungsanforderungen;
* Auswertungen;
* die Bearbeitung möglicher Rechtsbehelfe

benötigt werden.

Der Auftragnehmer hat die vorhandenen Datenbestände zu analysieren und ein Migrationskonzept vorzulegen. Erkannte Dubletten, unvollständige Angaben und strukturelle Abweichungen sind durch den Auftragnehmer soweit technisch möglich zu bereinigen.

Der Auftraggeber stellt vorhandene Datenexporte und fachliche Ansprechpartner zur Verfügung. Weitere Mitwirkungsleistungen werden nach Abschluss der Datenanalyse festgelegt.

Eine vollständige historische Übernahme aller Altbestände kann als gesonderte Option angeboten werden.

## 8. Einführung, Pilot und Schulung

Die Einführung erfolgt zunächst in einer Pilotkommune. Der Pilot umfasst mindestens:

* Schülerbeförderung und Fahrtkostenerstattung;
* Lernmittelfreiheit beziehungsweise Lernmittelunterstützung;
* Zuschüsse zur Mittagsverpflegung.

Die Leihgeräteverwaltung kann in den Pilot einbezogen werden, sofern ein geeignetes Standardmodul verfügbar ist und hierdurch der Zeitplan nicht wesentlich beeinträchtigt wird.

Der Auftragnehmer erstellt auf Grundlage der Vergabeunterlagen ein Feinkonzept und einen verbindlichen Einführungsplan. Das Feinkonzept konkretisiert insbesondere:

* fachliche Prozesse;
* Rollen und Berechtigungen;
* Datenflüsse und Schnittstellen;
* Migration;
* Konfiguration;
* Test und Abnahme;
* Schulungen;
* Pilotierung und Rollout.

Für Sachbearbeitung, Teamleitungen und IT-Administration sind zielgruppenspezifische Schulungen vorzusehen. Für Schulen und externe Dienstleister sind geeignete Einweisungs- oder Selbstlernangebote bereitzustellen.

Nach erfolgreichem Pilotbetrieb erfolgt der schrittweise Rollout auf die weiteren Kommunen.

## 9. Betrieb, Service und Performance

Die produktive Lösung muss eine monatliche Verfügbarkeit von mindestens 99,5 Prozent erreichen. Angekündigte Wartungsfenster werden bei der Berechnung nicht berücksichtigt.

Der Auftragnehmer stellt Support mindestens montags bis freitags von 8:00 bis 18:00 Uhr bereit. Kritische Störungen müssen innerhalb von 30 Minuten bestätigt und unverzüglich bearbeitet werden. Für sonstige Anfragen ist grundsätzlich eine Rückmeldung am selben Arbeitstag vorzusehen.

Die abschließenden Reaktions-, Wiederherstellungs- und Lösungszeiten werden im Servicekonzept festgelegt.

Das System muss Lastspitzen insbesondere vor Ablauf gesetzlicher oder behördlich bekannt gegebener Antragsfristen ohne wesentliche Leistungseinbußen bewältigen. Die Skalierung der technischen Ressourcen erfolgt durch den Auftragnehmer und darf nicht zu zusätzlichen Lizenzkosten führen.

Updates, Sicherheitsaktualisierungen und neue Releases sind regelmäßig bereitzustellen. Wesentliche Änderungen an Bedienung, Schnittstellen oder fachlichen Abläufen sind dem Auftraggeber rechtzeitig anzukündigen.

## 10. Datenschutz und Informationssicherheit

Die Lösung muss die datenschutzrechtlichen und informationssicherheitsbezogenen Anforderungen des Auftraggebers erfüllen.

Insbesondere sind vorzusehen:

* rollenbasierte Zugriffssteuerung nach dem Prinzip der geringsten Berechtigung;
* Mehr-Faktor-Authentisierung für administrative Zugriffe;
* Verschlüsselung bei Übertragung und Speicherung;
* Protokollierung administrativer und sicherheitsrelevanter Vorgänge;
* mandanten- und organisationsbezogene Trennung der Daten;
* Lösch- und Aufbewahrungsfunktionen;
* regelmäßige Datensicherungen;
* Wiederanlauf- und Notfallverfahren;
* Verfahren zum Umgang mit Sicherheitsvorfällen;
* regelmäßige Schwachstellenprüfungen.

Der Auftragnehmer legt mit dem Angebot einen TOM-Katalog sowie eine Beschreibung des Sicherheits- und Betriebskonzepts vor. Die eingesetzte Betriebsumgebung muss nach ISO/IEC 27001 zertifiziert sein oder ein vergleichbares Sicherheitsniveau nachweisen.

Der Auftragnehmer unterstützt den Auftraggeber bei der Erstellung beziehungsweise Fortschreibung der Datenschutz-Folgenabschätzung und stellt die hierfür erforderlichen technischen und organisatorischen Informationen bereit.

Sicherheitsrelevante Protokolldaten sind für mindestens zehn Jahre revisionssicher aufzubewahren. Personenbezogene Daten sind nach Ende des jeweiligen Vorgangs spätestens innerhalb von 30 Tagen zu löschen, soweit keine gesetzlichen Aufbewahrungspflichten entgegenstehen.

## 11. Datenportabilität und Vertragsende

Der Auftraggeber muss seine Daten während der Vertragslaufzeit und bei Vertragsende vollständig exportieren können.

Der Export umfasst mindestens:

* Stamm- und Vorgangsdaten;
* Dokumente;
* Status- und Bearbeitungshistorien;
* Kommunikationsdaten;
* Rollen- und Konfigurationsdaten;
* Protokolldaten.

Die Daten sind in gängigen, maschinenlesbaren Formaten bereitzustellen. Die konkreten Exportformate und Übergabeverfahren werden im Feinkonzept festgelegt.

Der Auftragnehmer unterstützt bei Vertragsende den Übergang auf ein Nachfolgesystem. Hierfür erforderliche Unterstützungsleistungen werden nach Aufwand vergütet.

## 12. Test und Abnahme

Vor dem Pilotbetrieb führt der Auftragnehmer gemeinsam mit dem Auftraggeber Funktions-, Integrations-, Migrations-, Sicherheits-, Performance- und Barrierefreiheitstests durch.

Die Abnahme setzt insbesondere voraus, dass:

* die für den Pilot vorgesehenen Prozesse durchgängig bearbeitet werden können;
* Daten und Dokumente vollständig zwischen den beteiligten Systemen übertragen werden;
* keine wesentlichen Datenschutz- oder Sicherheitsmängel bestehen;
* die vereinbarten Performance- und Verfügbarkeitswerte erreicht werden;
* die Pilotnutzer die Lösung im Wesentlichen ohne zusätzliche Unterstützung bedienen können;
* keine Fehler vorliegen, die den produktiven Einsatz wesentlich beeinträchtigen.

Die Pilotphase gilt als erfolgreich, wenn die vorgesehenen Prozesse über einen Zeitraum von vier Wochen stabil betrieben werden und die Projektgruppe keine wesentlichen Einwände erhebt.

Äußert der Auftraggeber innerhalb von zehn Arbeitstagen nach Bereitstellung zur Abnahme keine wesentlichen Mängel, gilt die jeweilige Leistung als abgenommen.
