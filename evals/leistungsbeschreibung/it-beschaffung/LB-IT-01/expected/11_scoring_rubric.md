---
title: "Testakte LB-IT-01 – Scoring Rubric"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "scoring-rubric"
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

# Aktenstück 11 – Scoring Rubric

## 1. Rubric A – Neuentwurf einer Leistungsbeschreibung

Maximalpunktzahl: **100 Punkte**.

| Bereich | Punkte |
|---|---:|
| Übergang und Nachvollziehbarkeit aus der Markterkundung | 15 |
| Nutzung des Templates und sinnvolle Strukturierung | 10 |
| Neutralisierung von Anbieter- und Technologiepositionen | 15 |
| Abgrenzung von Grundleistung, Optionen und offenen Punkten | 15 |
| Qualität der MUSS-/KANN-/Kandidaten-Systematik | 15 |
| Betriebsmodell, Datenaustausch, Migration und Exit | 10 |
| Datenschutz, Informationssicherheit und Barrierefreiheit mit Leistungsbezug | 10 |
| Trennung zu Wertung, Eignung, Vertrag und gesonderten Anlagen | 5 |
| Transparenz zu Annahmen, Risiken und Prüfbedarf | 5 |
| **Gesamt** | **100** |

### Übergang und Nachvollziehbarkeit aus der Markterkundung – 15 Punkte

Bewertet wird, ob der Assistent den Fortsetzungscharakter von `LB-IT-01`, den Bezug zu `M-IT-01` und den Status des Übergabevermerks korrekt versteht.

### Nutzung des Templates und sinnvolle Strukturierung – 10 Punkte

Bewertet wird, ob das Template als hilfreiche Strukturreferenz genutzt wird, ohne den Sachverhalt schematisch oder mit unpassenden Abschnitten zu überfrachten.

### Neutralisierung von Anbieter- und Technologiepositionen – 15 Punkte

Bewertet wird, ob Anbieterpositionen, Technologiepräferenzen und Marktbehauptungen neutralisiert und nicht als Auftraggeberentscheidung übernommen werden.

### Abgrenzung von Grundleistung, Optionen und offenen Punkten – 15 Punkte

Bewertet wird, ob dokumentierter Bedarf, neue interne Entscheidungen, mögliche Optionen, spätere Ausbaustufen und offene Punkte sauber getrennt werden.

### Qualität der MUSS-/KANN-/Kandidaten-Systematik – 15 Punkte

Bewertet wird:

* ob `MUSS`-Anforderungen erforderlich und prüfbar sind;
* ob `KANN` nur bei erkennbarer Bewertbarkeit verwendet wird;
* ob sonst Kandidaten oder offene Bewertungsfragen ausgewiesen werden;
* ob keine Punkte, Gewichtungen oder Bewertungsmaßstäbe erfunden werden.

### Betriebsmodell, Datenaustausch, Migration und Exit – 10 Punkte

Bewertet wird, ob Betriebsmodell, Datenaustausch, Schnittstellen, Migration, Datenportabilität und Exit differenziert und offen beschrieben werden.

### Datenschutz, Informationssicherheit und Barrierefreiheit mit Leistungsbezug – 10 Punkte

Bewertet wird, ob leistungsbezogene Funktionen beschrieben und vollständige Datenschutz-, Sicherheits- oder Barrierefreiheitskonzepte nicht ungefragt ausgearbeitet werden.

### Trennung zu Wertung, Eignung, Vertrag und gesonderten Anlagen – 5 Punkte

Bewertet wird, ob die Leistungsbeschreibung nicht mit Kriterienmatrix, Eignungsanforderungen, Referenzen, Haftung, Vertragsstrafen, Kündigung oder EVB-IT-Anlagen vermischt wird.

### Transparenz zu Annahmen, Risiken und Prüfbedarf – 5 Punkte

Bewertet wird, ob offene Annahmen, Risiken und Prüfbedarfe klar sichtbar bleiben.

## 2. Rubric B – Prüfung einer internen Arbeitsfassung

Maximalpunktzahl: **100 Punkte**.

| Bereich | Punkte |
|---|---:|
| Erkennung des Fortsetzungs- und Markterkundungskontexts | 10 |
| Erkennung von Anbieter-, Produkt- und Technologievorfestlegungen | 20 |
| Erkennung widersprüchlicher und unbestimmter Leistungsanforderungen | 15 |
| Prüfung von Grundleistung, MUSS, KANN, Kandidaten, Optionen und offenen Punkten | 15 |
| Prüfung von Betriebsmodell, Schnittstellen, Migration, Portabilität und Exit | 10 |
| Prüfung von Datenschutz, Informationssicherheit, Barrierefreiheit und Rollenrechten | 10 |
| Trennung zu Wertung, Eignung, Vertrag und gesonderten Unterlagen | 10 |
| Qualität der konkreten Änderungs- und Neutralisierungsvorschläge | 10 |
| **Gesamt** | **100** |

Testmodus B bewertet keine vollständige Neufassung. Entscheidend sind Risikoerkennung, korrekte Dokumentzuordnung und brauchbare Änderungsvorschläge. Hohe Punktzahlen setzen voraus, dass der Assistent tragfähige Bestandteile erkennt und erhält, zwischen Beibehalten, Konkretisieren, Verschieben und Streichen beziehungsweise Neutralisieren unterscheidet, Probleme priorisiert und nicht pauschal neu formuliert. Das Template dient als Struktur- und Abgrenzungsreferenz, nicht als starre Musterlösung.

### Erkennung des Fortsetzungs- und Markterkundungskontexts – 10 Punkte

Bewertet wird, ob der Assistent `LB-IT-01` als Fortsetzung von `M-IT-01` versteht und Marktrückläufe nicht als Angebote oder Auftraggeberentscheidungen behandelt.

### Erkennung von Anbieter-, Produkt- und Technologievorfestlegungen – 20 Punkte

Bewertet wird, ob verdeckte Vorprägungen durch Weiterverwendung von `SchulFach 9`, Hersteller- oder Standardschnittstellen, Produktarchitekturen, bestimmte Betriebsmodelle oder eine unklare Gesamtverantwortung erkannt werden. Erwartet wird keine pauschale Ablehnung vorhandener Systeme, sondern eine leistungsbezogene Neutralisierung von Lock-in- und Wettbewerbsrisiken.

### Erkennung widersprüchlicher und unbestimmter Leistungsanforderungen – 15 Punkte

Bewertet wird, ob widersprüchliche Vorgaben, unbestimmte Qualitätsbegriffe, nicht aktenbelegte Performance-, SLA-, Lösch- und Protokollierungswerte sowie unprüfbare Abnahme- oder Erfolgskriterien erkannt werden.

### Prüfung von Grundleistung, MUSS, KANN, Kandidaten, Optionen und offenen Punkten – 15 Punkte

Bewertet wird, ob der Assistent tragfähige Anforderungen von bloßen Kandidaten, Optionen und offenen Punkten unterscheidet, die Standardmodulabhängigkeit der Leihgeräteverwaltung einordnet, `KANN`-Funktionen wie KI, Chatbot und Mehrsprachigkeit nicht pauschal streicht, die undefinierte `SOLL`-Kategorie klärt und qualitative Wünsche nicht vorschnell als bewertungsreif behandelt.

### Prüfung von Betriebsmodell, Schnittstellen, Migration, Portabilität und Exit – 10 Punkte

Bewertet wird, ob der Assistent die Risiken aus SaaS-Präferenz, fehlender Betriebsmodellentscheidung oder fehlender Vergleichssystematik, zu spät festgelegten Schnittstellen- und Architekturfragen, historischer Migration, Datenbereinigung, Mitwirkungsleistungen sowie vorhandenen, aber noch zu konkretisierenden Portabilitäts- und Exit-Regelungen erkennt.

### Prüfung von Datenschutz, Informationssicherheit, Barrierefreiheit und Rollenrechten – 10 Punkte

Bewertet wird, ob der Assistent Systemfunktionen, Nachweise, TOM, Sicherheits- und Betriebskonzept, AVV, DSFA-Unterstützung sowie Vertrags- und Anlagenregelungen trennt. Außerdem wird bewertet, ob unklare Barrierefreiheit, nicht belegte Lösch- und Protokollierungsfristen sowie ungeklärte Detailrechte für Schulen und Dienstleister erkannt werden.

### Trennung zu Wertung, Eignung, Vertrag und gesonderten Unterlagen – 10 Punkte

Bewertet wird, ob der Assistent Wertungsmethodik, Referenzen wie F-15, Angebotspräsentationen, Nachweise, Vergütungsregelungen, Abnahmefiktion und gesonderte Datenschutz- oder Sicherheitsunterlagen aus der Leistungsbeschreibung herauslöst.

### Qualität der konkreten Änderungs- und Neutralisierungsvorschläge – 10 Punkte

Bewertet wird, ob die Vorschläge praktisch nutzbar, produktneutral, dokumentengerecht, priorisiert und nicht übermäßig pauschal sind. Positiv zu bewerten ist, wenn tragfähige Passagen bewusst beibehalten und nur bei Bedarf konkretisiert oder in ein passenderes Dokument verschoben werden.

Dieselbe Schwäche darf nicht mehrfach voll bepunktet oder mehrfach vollständig abgewertet werden. Vorfestlegung und Lock-in, Schnittstellen und Architektur, Betriebsmodell und Vergleichbarkeit sowie Datenschutzfunktionen und gesonderte Datenschutz- oder Sicherheitsunterlagen sind bei Überschneidungen nachvollziehbar einem Schwerpunkt zuzuordnen.

## 3. Gemeinsame Bewertungsstufen

| Punkte | Einordnung |
|---:|---|
| 90–100 | sehr gut |
| 75–89 | gut |
| 60–74 | mit Überarbeitungsbedarf |
| unter 60 | nicht ausreichend |

## 4. Gemeinsame KO-Fehler

Ein KO-Fehler begrenzt die Bewertung des jeweiligen Testmodus auf höchstens 59 Punkte. KO-Fehler sind insbesondere:

* Empfehlung oder Bevorzugung eines Marktteilnehmers;
* Festlegung auf `SchulFach 9`, Low-Code, Open Source oder eine andere Technologie allein aufgrund einer Marktantwort oder einer verdeckten Produktvorprägung;
* Darstellung des Übergabevermerks als tatsächlich dokumentierter früherer Assistenten-Output;
* ungeprüfte Übernahme anbieterspezifischer Aussagen als Mindestanforderung;
* vollständige Kriterienmatrix trotz gegenteiliger Anweisung;
* erfundene Punkte oder Gewichtungen;
* KI-Funktionen, Chatbot oder Mehrsprachigkeit werden ohne Grundlage als zwingende Startanforderung behandelt;
* historische Migration wird ohne Zweckabgrenzung als vollständige Zwangsmigration behandelt oder ohne Prüfung pauschal verworfen;
* direkte oder herstellergebundene Schnittstellen werden allein aufgrund von Anbieterangaben zwingend;
* Leihgeräteverwaltung wird allein wegen Produkt- oder Standardmodulgrenzen ohne interne Entscheidung zur Option erklärt;
* BundID oder E-Payment werden ohne Grundlage zwingende Startanforderungen oder verbindliche Umsetzungsleistungen ohne geklärten Zeitpunkt und Abrufmechanismus;
* pauschale Datenschutz- oder Sicherheitskonzepte werden ungefragt erzeugt;
* Vertragsklauseln werden ungefragt erzeugt;
* Exit-, Lock-in-, Schnittstellen- oder Migrationsrisiken werden vollständig ignoriert oder vorhandene tragfähige Exit-Ansätze pauschal als fehlend behandelt;
* Marktrückläufe werden als verbindliche Angebote oder technische Nachweise behandelt;
* eine abschließende Losbildungs-, Betriebsmodell- oder Verfahrensentscheidung wird erfunden.

Bei Testmodus B ist kein KO-Fehler allein deshalb anzunehmen, weil der Assistent vorhandene Exit-Regelungen zu Recht nicht als fehlend beanstandet, KI, Chatbot oder Mehrsprachigkeit als `KANN` beziehungsweise Bewertungskandidaten behandelt, historische Migration differenziert statt pauschal ablehnt oder tragfähige Teile der Arbeitsfassung bewusst beibehält. Eine bloß unvollständige Detailprüfung ist grundsätzlich über die Punktwertung zu berücksichtigen.
