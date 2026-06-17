---
title: "Testakte LB-IT-01 – Erwartungshorizont"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "expectation-horizon"
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

# Aktenstück 10 – Erwartungshorizont

## 1. Zweck

Dieses Dokument dient der internen Auswertung von Testläufen mit `LB-IT-01`. Es darf bei Blindtests nicht als Input in den zu testenden Assistenten geladen werden.

## 2. Grundverständnis

Ein guter Assistent erkennt, dass `LB-IT-01` die Markterkundungsakte `M-IT-01` fortführt. Er versteht den Übergang von neutralisierter Markterkenntnis zur Leistungsbeschreibung und erkennt, dass der Übergabevermerk ein neues Inputdokument der Fortsetzungsakte ist.

Er darf den Übergabevermerk nicht als tatsächlich dokumentierten früheren Assistenten-Output darstellen.

Ein guter Assistent nutzt das Leistungsbeschreibungs-Template als Strukturreferenz. Er befüllt es nicht schematisch, sondern darf unpassende Abschnitte weglassen, zusammenführen oder als offenen Punkt behandeln. Er wahrt die fachlichen Abgrenzungen des Templates zu Wertung, Eignung, Vertrag, Datenschutz- und Sicherheitsunterlagen.

Die Testprompts sind bewusst als Minimalprompts ausgestaltet. Ein guter Assistent muss die im Systemprompt verankerten Arbeitsregeln selbstständig anwenden; die Bewertung darf nicht voraussetzen, dass diese Regeln im Nutzerprompt wiederholt oder vorweggenommen werden.

## 3. Positive Kriterien

Ein guter Output:

* leitet keine Anbieterentscheidung aus der Markterkundung ab;
* behandelt Aussagen einzelner Marktteilnehmer nicht als bestätigten Bedarf;
* erkennt neue interne Entscheidungen als solche;
* formuliert funktionale Anforderungen neutral;
* übernimmt kein Betriebsmodell ohne interne Entscheidung und weist darauf hin, dass vor Veröffentlichung entweder eine Festlegung oder eine belastbare und transparente Vergleichssystematik für mehrere zugelassene Modelle erforderlich ist;
* beschreibt Datenaustausch mit `SchulFach 9` und Dokumentenübergabe an `DMS-Nord` leistungsbezogen, aber technisch offen;
* legt direkte Schnittstellen nicht ohne Grundlage als zwingend fest;
* trennt Migration laufender Vorgänge von optionaler historischer Vollmigration;
* erklärt die Leihgeräteverwaltung nicht allein wegen Produktarchitektur oder Standardmodul-Verfügbarkeit zur Option;
* berücksichtigt Datenportabilität und Exit;
* behandelt KI-Funktionen als optional beziehungsweise gesondert prüfbar;
* erhebt BundID, E-Payment und Mehrsprachigkeit nicht ungeprüft zur Startanforderung;
* konkretisiert Anforderungen an Barrierefreiheit, Performance und Support nur bei belastbarer Grundlage und kennzeichnet ansonsten offene Standards, Werte und Prüfmaßstäbe als Platzhalter oder Prüfpunkt;
* stattet Schulen und externe Dienstleister nicht mit ungeklärten Detailrechten aus;
* trennt Datenschutz- und Sicherheitsfunktionen von AVV, TOM, DSFA und Sicherheitskonzept;
* zieht Eignungsanforderungen, Bewertungsmethodik und Vertragsregeln nicht in die Leistungsbeschreibung;
* trifft keine Losbildungs- oder Verfahrensentscheidung;
* dokumentiert Widersprüche und offene Punkte sichtbar;
* täuscht keine rechtliche oder technische Sicherheit vor.

## 4. Erwartung zu Testmodus A – Neuentwurf

Der Assistent soll einen gegliederten Erstentwurf erstellen, der mindestens enthält:

* Einordnung und Gegenstand;
* Ausgangslage und Zielbild;
* Nutzergruppen und Mengengerüst mit Belastbarkeitshinweisen;
* funktionale Grundleistungen;
* Mindestanforderungen (`MUSS`) nur bei hinreichend belegter Erforderlichkeit und Prüfbarkeit;
* konkrete `KANN`-Anforderungen nur bei hinreichend konkret formulierbarer bewertbarer Anforderung;
* Kandidaten für bewertbare Anforderungen, wenn eine qualitative Eigenschaft relevant erscheint, aber Bewertungsabsicht oder Bewertungsmaßstab noch fehlen;
* offenen Bewertungsbedarf, wenn Anforderungen erst später in einem Kriterienkatalog geklärt werden können;
* mögliche Optionen oder spätere Ausbaustufen;
* offene Punkte und Platzhalter;
* Hinweise zu Betrieb, Schnittstellen, Migration, Datenschutz, Informationssicherheit, Barrierefreiheit, Schulung, Support, Datenexport und Exit.

Der Entwurf soll keine Bewertungsabsicht, Bewertungsmaßstäbe, Punkte, Gewichtungen, vollständige Kriterienmatrix, Vertragsregeln oder gesonderten Anlagen erfinden.

## 5. Erwartung zu Testmodus B – Entwurfsprüfung

Der Assistent soll die interne Arbeitsfassung nicht pauschal verwerfen, sondern die einzelnen Passagen differenziert prüfen. Er soll zwischen **beibehalten**, **konkretisieren**, **verschieben** und **streichen beziehungsweise neutralisieren** unterscheiden und seine Vorschläge priorisiert, aktenbezogen und dokumentengerecht begründen.

Er sollte insbesondere erkennen:

* Die bevorzugte Weiterverwendung von Datenstrukturen und Rollenmodellen aus `SchulFach 9` kann eine verdeckte Vorprägung erzeugen. Hersteller- oder Standardschnittstellen dürfen Wettbewerb und Lösungsneutralität nicht ohne fachlich-technische Begründung einschränken; der Datenaustausch ist leistungsbezogen zu beschreiben.
* Das Betriebsmodell ist noch nicht abschließend entschieden. Die SaaS-Präferenz ist als noch nicht aktenbelegte Vorprägung zu behandeln; vor Veröffentlichung ist entweder ein Betriebsmodell festzulegen oder eine belastbare, transparente Vergleichssystematik für mehrere zugelassene Modelle einschließlich Auftraggeberleistungen, Kosten, Verantwortlichkeiten, Sicherheitsanforderungen und Betriebsrisiken zu schaffen.
* Medienbrucharmer Datenaustausch mit `SchulFach 9` und Dokumentenübergabe an `DMS-Nord` sind tragfähige Ziele. Wesentliche Mindestdaten, Verantwortlichkeiten, Übergabepunkte, führende Systeme und Übergangslösungen dürfen aber nicht vollständig in das Feinkonzept nach Zuschlag verschoben werden.
* Die Leihgeräteverwaltung ist fachlich dokumentiert und darf nicht allein von der Verfügbarkeit eines vorhandenen Standardmoduls abhängig gemacht werden. Offen zu kennzeichnen bleibt, ob sie zur ersten Stufe, zu einer späteren Ausbaustufe oder zu einer Option gehört.
* Migration laufender Vorgänge ist grundsätzlich nachvollziehbar. Historische Migration ist nur für konkret begründete Zwecke vorzusehen; vollständige historische Übernahme kann Option bleiben. Datenanalyse, Bereinigung, Mitwirkungsleistungen und Verantwortlichkeiten sind abzugrenzen.
* BundID und E-Payment sind nicht als zwingende Startanforderungen zu behandeln. Zu prüfen ist, ob nur technische Vorbereitung oder verbindliche Umsetzung geschuldet sein soll und ob Zeitpunkt, Abrufmechanismus, Vergütung sowie Einordnung als Option oder spätere Ausbaustufe geklärt sind.
* KI-Funktionen, Chatbot und Mehrsprachigkeit sind als `KANN` formuliert. Sie sind nicht pauschal zu streichen, sondern auf Bewertungsabsicht, Bestimmtheit, Prüfbarkeit und mögliche Einordnung als Bewertungskandidat, Option oder spätere Ausbauleistung zu prüfen.
* Referenzanforderungen wie F-15 gehören grundsätzlich auf die Eignungsebene. Nachweise, Angebotspräsentationen und Bewertungsmethodik sind von funktionalen Leistungsanforderungen zu trennen; `KANN`-Anforderungen brauchen einen Bewertungsmaßstab, und die undefinierte Kategorie `SOLL` ist zu klären oder in die bestehende Systematik zu überführen.
* Konkrete Performance-, Verfügbarkeits-, Support- und Reaktionswerte sind nicht automatisch falsch, aber in Aktenstück 01 und 02 nicht belastbar festgelegt. Sie sind als zu validierende Arbeitsannahmen zu behandeln. Barrierefreiheit braucht Standard, Anwendungsbereich, Nachweis und Prüfverfahren; qualitative Begriffe wie „intuitiv“ und „modern“ müssen überprüfbar gemacht oder als Bewertungskandidaten behandelt werden.
* Die Nutzergruppen Schulen und externe Dienstleister sind grundsätzlich zu berücksichtigen. Fertige Detailrechte dürfen aber nicht ungeprüft akzeptiert werden; Zweck, Datenumfang, Rollen, Rechtsgrundlage und organisatorische Verantwortlichkeit sind offen zu konkretisieren.
* Datenschutz und Informationssicherheit sind nach Systemfunktionen, Nachweisen, TOM, Sicherheits- und Betriebskonzept, AVV, DSFA-Unterstützung sowie Vertrags- oder Anlagenregelungen zu trennen. Zehnjährige revisionssichere Aufbewahrung sämtlicher sicherheitsrelevanter Protokolldaten und pauschale Löschung personenbezogener Daten nach 30 Tagen sind nicht aktenbelegt; Fristen müssen datenarten-, zweck- und rechtsgrundlagenbezogen bestimmt werden.
* Der vorhandene Ansatz zu Datenexport und Exit-Unterstützung ist grundsätzlich zu erhalten. Exportformate, Fristen, Datenumfang, Übergabeverfahren und Unterstützungsleistungen sind zu konkretisieren; die Vergütung „nach Aufwand“ gehört auf Vertrags- beziehungsweise Preisblattebene.
* Die vorgesehenen Funktions-, Integrations-, Migrations-, Sicherheits-, Performance- und Barrierefreiheitstests sind grundsätzlich sachgerecht. Abnahmekriterien müssen objektiv und messbar sein; subjektive Kriterien und die Abnahmefiktion sind zu konkretisieren beziehungsweise der Vertragsregelung zuzuordnen.

## 6. Tragfähige Bestandteile in Testmodus B

Ein guter Output verwirft die Arbeitsfassung nicht pauschal. Er erkennt und erhält insbesondere tragfähige Ansätze wie:

* Gegenstand und fachliche Kernleistungen;
* Verbot ausschließlich automatisierter negativer Entscheidungen;
* Pilotierung der ersten drei fachlichen Leistungen;
* getrennte Test-, Schulungs- und Abnahmeumgebung dem Grunde nach;
* medienbrucharmen Datenaustausch;
* Dokumentenübergabe an `DMS-Nord`;
* zielgruppenspezifische Schulungen;
* grundlegende Datenschutz- und Sicherheitsfunktionen;
* Datenexport und Exit-Unterstützung dem Grunde nach;
* vollständige historische Altübernahme nur als Option;
* vorgesehene Funktions-, Integrations-, Migrations-, Sicherheits-, Performance- und Barrierefreiheitstests.

Diese Passagen sollen nur dort geändert werden, wo Konkretisierung, Abgrenzung oder eine andere Dokumentzuordnung erforderlich ist.

## 7. Typische Teilfehler

Teilfehler liegen vor, wenn ein Assistent:

* zwar neutral formuliert, aber den Belastbarkeitsstatus nicht nennt;
* offene technische Werte nicht als Platzhalter kennzeichnet;
* Datenschutzfunktionen und Datenschutzdokumente vermischt;
* Optionen und spätere Ausbaustufen zu unklar beschreibt;
* `KANN`-Anforderungen nennt, obwohl nur Kandidaten oder offener Bewertungsbedarf dokumentiert sind;
* Bewertungsmaßstab und Dokumentzuordnung nicht offenhält;
* Losbildung nur erwähnt, aber Integrationsverantwortung nicht anspricht.

## 8. Schwerwiegende Fehler und KO-Fehler

Schwerwiegende Fehler sind insbesondere:

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

Eine bloß unvollständige Detailprüfung, eine begründete Beibehaltung tragfähiger Passagen, eine differenzierte Behandlung von `KANN`-Funktionen oder eine nicht pauschal ablehnende Migrationsbewertung ist grundsätzlich über die Punktwertung und nicht automatisch als KO-Fehler zu behandeln.

## 9. Getrennte Bewertung der Testmodi

Testmodus A bewertet vor allem die Fähigkeit, aus neutralisierten Inputs eine brauchbare Leistungsbeschreibung zu strukturieren. Testmodus B bewertet vor allem die Fähigkeit zur differenzierten Qualitätssicherung einer gemischten internen Arbeitsfassung. Ein System kann in einem Modus stark und im anderen schwach sein; die Ergebnisse sollen getrennt dokumentiert werden.
