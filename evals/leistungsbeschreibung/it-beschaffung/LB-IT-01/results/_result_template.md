---
title: "Testlauf LB-IT-01 – [System] – [Testmodus]"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "draft"
language: "de-DE"
type: "eval-result"
subtype: "result-template"
eval_case_id: "LB-IT-01"
predecessor_eval_case_id: "M-IT-01"
eval_test_id: "[test-id]"
run_id: "[lauf-000]"
test_mode: "[A-neuentwurf / B-entwurfspruefung]"
relative_date: "[T+...]"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
tested_system: "[System]"
tested_model: "[Modell]"
systemprompt_version: "[Version Leistungsbeschreibungs-Systemprompt]"
testprompt_version: "[Version des verwendeten Testprompts]"
testprompt_profile: "[minimal / guided / custom]"
additional_user_instructions: "[keine / Angabe]"
template_version: "[Version Leistungsbeschreibungs-Template]"
template_provided: null
repository_commit: "[Commit-SHA]"
web_search_enabled: null
additional_tools_or_actions: "[Angabe]"
knowledge_files_uploaded: "[Angabe]"
blind_test_status: "[full / limited / no]"
score_total: null
score_maximum: 100
score_classification: "not-evaluated"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/leistungsbeschreibung/it-beschaffung/LB-IT-01/results"
module_id: "leistungsbeschreibung-it-beschaffung"
module: "leistungsbeschreibung"
procurement_area: "it-beschaffung"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

# Testlauf LB-IT-01 – [System] – [Testmodus]

## 1. Testdatum und Einordnung

| Merkmal | Angabe |
|---|---|
| Testdatum | `[YYYY-MM-DD]` |
| Relative Einordnung | `[T+...]` |
| Testmodus | `[A – Neuentwurf / B – Entwurfsprüfung]` |
| Bezug auf `M-IT-01` | Fortsetzungsakte; `LB-IT-01` nutzt einen neu erstellten Übergabevermerk |
| Hinweis Übergabevermerk | Der Übergabevermerk ist kein authentischer früherer Assistenten-Output |

## 2. Testkonfiguration

| Merkmal | Angabe |
|---|---|
| Getestetes System |  |
| Getestetes Modell |  |
| Version Leistungsbeschreibungs-Systemprompt |  |
| Version verwendeter Testprompt |  |
| Testprompt-Profil | minimal / guided / custom |
| Zusätzliche Nutzerhinweise | keine / Angabe |
| Version Leistungsbeschreibungs-Template |  |
| Template bereitgestellt | ja/nein |
| Art der Template-Bereitstellung |  |
| Blindteststatus |  |
| Repository-Commit |  |
| Websuche | ja/nein |
| Zusätzliche Tools oder Actions |  |
| Knowledge-Dateien |  |

## 3. Verwendeter Testprompt

```text
[Prompt unverändert einfügen oder auf Datei verweisen]
```

**Zusätzliche Nutzerhinweise:** `[keine / vollständig und unverändert dokumentieren]`

## 4. Bereitgestellte Input-Dateien und Strukturreferenzen

### Input-Dateien

* `[Datei]`

### Strukturreferenz

* `templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md` – bereitgestellt: ja/nein

## 5. Nicht bereitgestellte Evaluations- und Ergebnisdateien

* `expected/10_erwartungshorizont.md`
* `expected/11_scoring_rubric.md`
* `expected/12_hinweise_zur_auswertung.md`
* `results/_result_template.md`

## 6. Unveränderte Rohantwort

```markdown
[Originalantwort unverändert einfügen oder auf Rohantwort verweisen]
```

## 7. Punktbewertung nach Rubric

**Verwendete Rubric:** `[A – Neuentwurf / B – Entwurfsprüfung]`

Pro Testlauf geht nur eine Rubric in die Gesamtpunktzahl ein. Die nicht verwendete Tabelle vor Speicherung des konkreten Testlaufs entfernen oder unausgefüllt als nicht anwendbar kennzeichnen.

### 7.1 Rubric A – nur für Testmodus A

| Bereich | Maximum | Erreicht | Kurzbegründung |
|---|---:|---:|---|
| Übergang und Nachvollziehbarkeit aus der Markterkundung | 15 |  |  |
| Nutzung des Templates und sinnvolle Strukturierung | 10 |  |  |
| Neutralisierung von Anbieter- und Technologiepositionen | 15 |  |  |
| Abgrenzung von Grundleistung, Optionen und offenen Punkten | 15 |  |  |
| Qualität der MUSS-/KANN-/Kandidaten-Systematik | 15 |  |  |
| Betriebsmodell, Datenaustausch, Migration und Exit | 10 |  |  |
| Datenschutz, Informationssicherheit und Barrierefreiheit mit Leistungsbezug | 10 |  |  |
| Trennung zu Wertung, Eignung, Vertrag und gesonderten Anlagen | 5 |  |  |
| Transparenz zu Annahmen, Risiken und Prüfbedarf | 5 |  |  |
| **Gesamt** | **100** |  |  |

### 7.2 Rubric B – nur für Testmodus B

| Bereich | Maximum | Erreicht | Kurzbegründung |
|---|---:|---:|---|
| Erkennung des Fortsetzungs- und Markterkundungskontexts | 10 |  |  |
| Erkennung von Anbieter-, Produkt- und Technologievorfestlegungen | 20 |  |  |
| Erkennung widersprüchlicher und unbestimmter Leistungsanforderungen | 15 |  |  |
| Prüfung von Grundleistung, MUSS, KANN, Kandidaten, Optionen und offenen Punkten | 15 |  |  |
| Prüfung von Betriebsmodell, Schnittstellen, Migration, Portabilität und Exit | 10 |  |  |
| Prüfung von Datenschutz, Informationssicherheit, Barrierefreiheit und Rollenrechten | 10 |  |  |
| Trennung zu Wertung, Eignung, Vertrag und gesonderten Unterlagen | 10 |  |  |
| Qualität der konkreten Änderungs- und Neutralisierungsvorschläge | 10 |  |  |
| **Gesamt** | **100** |  |  |

### 7.3 Ergänzende Dokumentation – nur für Testmodus B

Die folgenden Tabellen sind nur bei Testmodus B auszufüllen. Bei Testmodus A können sie entfernt oder als nicht anwendbar gekennzeichnet werden.

### Bewusst beibehaltene tragfähige Bestandteile

| Passage oder Regelung | Begründung für die Beibehaltung | Nur konkretisiert oder unverändert? |
|---|---|---|
|  |  |  |

### Änderungsart bei der Entwurfsprüfung

| Fundstelle | Beibehalten | Konkretisieren | In anderes Dokument verschieben | Streichen oder neutralisieren | Kurzbegründung |
|---|---:|---:|---:|---:|---|
|  |  |  |  |  |  |

## 8. KO-Fehler

Bei Testmodus B liegt ein KO-Fehler nur vor, wenn der Assistent eine problematische Aussage aus dem geprüften Entwurf übernimmt, bestätigt, als sachgerecht stehen lässt oder selbst erneut empfiehlt. Die kritische Benennung oder Wiedergabe eines erkannten Fehlers ist kein KO-Fehler.

| KO-Fehler | Vom Assistenten übernommen oder begangen? | Anmerkung |
|---|---|---|
| Empfehlung oder Bevorzugung eines Marktteilnehmers |  |  |
| Festlegung auf `SchulFach 9`, Low-Code, Open Source oder eine andere Technologie allein aufgrund einer Marktantwort oder verdeckten Produktvorprägung |  |  |
| Darstellung des Übergabevermerks als tatsächlich dokumentierter früherer Assistenten-Output |  |  |
| Ungeprüfte Übernahme anbieterspezifischer Aussagen als Mindestanforderung |  |  |
| Vollständige Kriterienmatrix trotz gegenteiliger Anweisung |  |  |
| Erfundene Punkte oder Gewichtungen |  |  |
| KI-Funktionen, Chatbot oder Mehrsprachigkeit werden ohne Grundlage als zwingende Startanforderung behandelt |  |  |
| Historische Migration wird ohne Zweckabgrenzung als vollständige Zwangsmigration behandelt oder ohne Prüfung pauschal verworfen |  |  |
| Direkte oder herstellergebundene Schnittstellen werden allein aufgrund von Anbieterangaben zwingend |  |  |
| Leihgeräteverwaltung wird allein wegen Produkt- oder Standardmodulgrenzen ohne interne Entscheidung zur Option erklärt |  |  |
| BundID oder E-Payment werden ohne Grundlage zwingende Startanforderungen oder verbindliche Umsetzungsleistungen ohne geklärten Zeitpunkt und Abrufmechanismus |  |  |
| Pauschale Datenschutz- oder Sicherheitskonzepte werden ungefragt erzeugt |  |  |
| Vertragsklauseln werden ungefragt erzeugt |  |  |
| Exit-, Lock-in-, Schnittstellen- oder Migrationsrisiken werden vollständig ignoriert oder vorhandene tragfähige Exit-Ansätze pauschal als fehlend behandelt |  |  |
| Marktrückläufe werden als verbindliche Angebote oder technische Nachweise behandelt |  |  |
| Eine abschließende Losbildungs-, Betriebsmodell- oder Verfahrensentscheidung wird erfunden |  |  |

## 9. Qualitative Beobachtungen

### Stärken

*

### Schwächen und Unschärfen

*

### Abweichungen vom Erwartungshorizont

*

## 10. Fazit

`[Gesamtbewertung, Punkteklasse und kurze Begründung]`

## 11. Prüfende Person

`[Name / Rolle]`
