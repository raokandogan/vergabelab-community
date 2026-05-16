---
title: "VergabeLab Community"
version: "0.1.0"
status: "initial"
language: "de-DE"
type: "root-readme"
license: "CC-BY-4.0"
repository_area: "root"
spdx_file_copyright_text: "2026 Okan Doğan"
spdx_license_identifier: "CC-BY-4.0"
topics:
  - "VergabeLab Community"
  - "KI-Bausteine"
  - "Vergabewesen"
  - "Wissen"
  - "Netzwerk"
  - "Open Knowledge"
  - "Open Source"
---

<!--
SPDX-FileCopyrightText: 2026 Okan Doğan
SPDX-License-Identifier: CC-BY-4.0
-->

<img width="1200" height="410" alt="VergabeLab-Community" src="https://github.com/user-attachments/assets/1a2a22a4-b393-4b9e-9e3a-655342ba0a44" />

---

# VergabeLab Community - Freie KI-Bausteine für Vergabestellen

Dieses Repository sammelt **offene KI-Bausteine** – insbesondere Konfigurationstexte (Systemprompts, Hinweistexte) für **OpenAI Custom GPTs**, **Claude Projects** sowie weitere „Expertensysteme“, daneben **Textmuster, Leitfäden und Wissensbausteine** – für typische Aufgaben im öffentlichen Beschaffungswesen: von der **Markterkundung** über **Leistungsbeschreibungen** bis hin zu **Vertragsgestaltung**, **Wertung** und **Zuschlag**.

Ziel von VergabeLab Community ist es, **Erfahrungswissen aus der Praxis** in wiederverwendbare Bausteine zu überführen und Vergabestellen bei der **sicheren und verantwortungsvollen Nutzung von KI** in Vergabeprozessen zu unterstützen.

**Was bringt das in der Vergabepraxis?**
- **Struktur und Tempo**: schneller vom „leeren Blatt“ zu belastbaren Entwürfen (Markterkundung → LB → Wertung).
- **Qualitätssicherung**: weniger Lücken/Widersprüche, konsistentere Anforderungen und Kriterien.
- **Bessere Dokumentation**: nachvollziehbare Begründungsbausteine (ohne Automatisierung der Entscheidung).

Der Fokus liegt ausdrücklich auf **Unterstützung**, nicht auf Vollautomatisierung von Vergabeentscheidungen. Verantwortlich für die Inhalte und Entscheidungen bleibt immer der Mensch.

**Abgrenzung:** VergabeLab Community ist die Open-Knowledge- und Open-Source-Ebene dieses Projekts. Separate kommerzielle Angebote (z. B. Integrations-/Update-Services oder Partner-Module) sind nicht Bestandteil dieses Repositorys und werden getrennt dokumentiert und vertraglich geregelt.

**Lizenzierung (Zusammenfassung):**  
- Alle **Textartefakte** in diesem Repository (Systemprompts/Hinweistexte, Templates, Guides, Muster, Wissensbausteine) stehen – soweit nicht in der Datei selbst anders gekennzeichnet – unter **CC BY 4.0** (Attribution, geringe Nutzungshürden).
- Echte **Software-/Tooling-Bestandteile** (z. B. Plugins, Skripte, Automatisierungstools) werden – sofern vorhanden – separat lizenziert und in einem eigenen Ordner (z. B. tooling/) geführt; hierfür ist **EUPL 1.2** vorgesehen.  
- Details, Pflichten und Beispiel-Attribution: siehe Abschnitt **[Lizenzierung](#5-lizenzierung)**.

---

## 1. Was finde ich hier konkret?

Beispiele für Bausteine, die hier nach und nach entstehen:

- **Markterkundung**  
  Systemprompts/Hinweistexte, mit denen KI-Assistenten strukturiert
  - Markterkundungen begleiten,
  - An Anbieter gerichtete Fragen formulieren,
  - Anbieter-Feedback zusammenfassen,
  - Risiken und Abhängigkeiten identifizieren.

- **Leistungsbeschreibungen**  
  Systemprompts/Hinweistexte, mit denen KI-Assistenten helfen,
  - technische und funktionale Anforderungen zu strukturieren,
  - Varianten- und Losbildung sauber abzubilden,
  - typische No-Gos (unzulässige Produkt-/Herstellervorgaben etc.) zu vermeiden.

- **Angebotswertung & Dokumentation**  
  Hilfen zur
  - Strukturierung von Zuschlagskriterien,
  - Dokumentation der Wertungsschritte,
  - Erzeugung von wertungsbegleitenden Begründungsbausteinen (ohne die Entscheidung zu „automatisieren“).

- **Muster-Dokumente (Wissensbasis)**  
  Leistungsfähige KI-Assistenten stehen und fallen mit der Wissensbasis. In diesem Repository sammeln wir daher auch
  - Muster-Anschreiben,
  - Muster-Fragenkataloge,
  - Muster-Leistungsbeschreibungen,
  - Vorlagen für Prüfschemata etc.

- **Begleitende Leitfäden**  
Kurze Handreichungen, wie die Bausteine
  - in Custom GPTs (chatgpt.com) und Pendants anderer Hersteller (z. B. Claude Projects),
  - in Azure OpenAI,
  - in selbst gehosteten LLM-Setups
eingebunden werden können.

- **Software-Tools, Skripte und Automatisierung (perspektivisch)**  
  Künftig können auch echte Software- und Tooling-Bestandteile hinzukommen, etwa
  - kleine Hilfsskripte,
  - Prüf- oder Konvertierungswerkzeuge,
  - Integrationsbeispiele,
  - Automatisierungshilfen für wiederkehrende Arbeitsschritte.

  Solche Bestandteile werden getrennt von Textartefakten geführt (z. B. in `tooling/`) und gesondert lizenziert (EUPL 1.2).

---

## 2. Quickstart: So nutzt du den ersten Prompt

> Wenn du es bis hierhin geschafft hast, bist du bereit, dein erstes KI-Expertensystem (Custom GPT & Co.) zu erstellen.

**Beispiel: Markterkundungs-GPT (Systemprompt/Hinweistext)**

- **I. Datei wählen**  
Öffne den Ordner [`prompts/markterkundung/it-beschaffung`](./prompts/markterkundung/it-beschaffung)

- **II. Inhalt kopieren**  
Öffne die Datei `01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md` und kopiere nur den Abschnitt zwischen **„KOPIERBEREICH START“** und **„KOPIERBEREICH ENDE“** in die Zwischenablage.

- **III. GPT konfigurieren (am Beispiel ChatGPT)**  
1.  Gehe zu **[chatgpt.com/gpts](https://chatgpt.com/gpts)** (oder klicke links auf "GPTs erkunden").
2.  Klicke oben rechts auf **"+ Erstellen"**.
3.  Wähle im Editor oben links den Reiter **"Konfigurieren"**.
4.  Füge den kopierten Text in das Feld **"Hinweise"** ein.
5.  Ergänze Name (z. B. "Vergabe-Assistent") und Beschreibung.

- **IV. Kontext hinzufügen (Optional)**  
Ergänze bei Bedarf projektspezifische Parameter (z. B. Bundesland, Behörde/Organisationseinheit) direkt im Anweisungsfeld oder lade Dokumente (z. B. TVgG, Verwaltungsvorschriften) als **"Wissen"** (Knowledge) hoch.

- **V. Testen**  
Klicke oben rechts auf "Erstellen" (oder "Update") und teste den Assistenten mit einer typischen Frage.

> **Community-Tipp:** VergabeLab-Bausteine sind bewusst so angelegt, dass sie **angepasst und verbessert** werden. Wenn du Änderungen vornimmst, freuen wir uns, wenn du sie – im Sinne der Community – wieder teilst (z. B. per Issue oder Pull Request).

---

## 3. Struktur dieses Repositorys
Dieses Repository ist bewusst in vier Bereiche getrennt. Ziel ist eine klare Trennung zwischen (1) Modell-Steuerung, (2) fachlicher Wissensbasis, (3) wiederverwendbaren Output-Artefakten und (4) Nutzungs-/Integrationsanleitungen.

- **prompts/**
Systemprompts und Hinweis-/Konfigurationstexte zur Steuerung von LLMs (z. B. ChatGPT Custom GPTs, Claude Projects). Enthält modulbezogene Prompt-Dateien und jeweils ein README pro Modul.

- **wissen/**
Fachliche Wissensbasis und Referenzmaterial (Leitfäden, Grundlagen, Begriffsdefinitionen, Fallstricke) zur inhaltlichen Unterfütterung der Module und als Wissens-Upload für LLMs.  
Wichtig: Keine Systemprompts und keine ausfüllbaren Mustertexte/Templates.

- **templates/**
Wiederverwendbare Muster und Arbeitsmittel für die Praxis (z. B. Gliederungen, Checklisten, Matrizen, Musteranschreiben, Textbausteine). Fokus: „Copy/Paste“ bzw. unmittelbar einsetzbare Artefakte.

- **guides/**
Anleitungen zur Nutzung und Einbindung (z. B. Nutzung von GitHub, Einrichtung/Einbindung in Custom GPTs, Arbeitsabläufe, Handling-Hinweise, Best Practices). Fokus: „So nutzt du die Bausteine sicher und konsistent“.

- **LICENSES/**
Lizenztexte und Referenzen. Maßgeblich sind die Lizenzhinweise in den jeweiligen Dateien, insbesondere YAML-Frontmatter und SPDX-Kommentar.

> Hinweis: Markdown-Dateien sollen am Anfang ein YAML-Frontmatter mit Metadaten und anschließend einen SPDX-Kommentar enthalten. Dadurch bleiben Lizenzzuordnung, Rechtekette und fachliche Einordnung auch bei Kopie/Weitergabe nachvollziehbar.

Daraus ergibt sich die folgende - nach und nach befüllte - Struktur:

```text
/
├─ prompts/
│  ├─ markterkundung/
│  │  └─ it-beschaffung
│  │     └─ 01_hinweistext_systemprompt_markterkundung_chatgpt_customgpt_de.md
│  │     └─ README.md
│  │  └─ ...
│  └─ weitere_module/...
│
├─ guides/
│  ├─ 00_github_basics_de.md
│  ├─ 01_lizenz_faq_de.md
│  └─ ...
│
├─ templates/
│  ├─ markterkundung
│  │  └─ it-beschaffung
│  │     └─ 01_anschreiben_und_fragenkatalog_de.md
│  └─ ...
│
├─ wissen/
│  ├─ markterkundung
│  │  ├─ 01_leitfaden_markterkundung_de.md
|  |  ├─ 02_typische_fehler_markterkundung_de.md
|  |  └─ ...
│  └─ README.md
│
├─ LICENSES/
│  ├─ EUPL-1.2.txt
│  └─ CC-BY-4.0.txt
│
├─ CONTRIBUTING.md
├─ DCO.md
├─ POLICIES/
│  └─ SPDX.md
└─ README.md
```
---

## 4. Wie kann ich beitragen?

Dieses Projekt lebt vom Erfahrungswissen der Community. Beiträge sind ausdrücklich erwünscht, egal ob du **Vergabepraktiker:in**, **Jurist:in** oder **Entwickler:in** bist. Du musst kein Git-Profi sein, um zu helfen!

### Neu bei GitHub?
- Wenn du GitHub nicht kennst, starte hier: [guides/00_github_basics_de.md](guides/00_github_basics_de.md).
- Alternativ reicht für den Anfang oft schon ein Beitrag in den **„Discussions“** (siehe unten).

### Wer ist angesprochen?
- **Öffentliche Auftraggeber & Vergabestellen** (Einbringen von Praxis-Perspektive, fachlichen Anforderungen etc.)
- **Rechtsberatung & Justiziariate** (Steigerung der Rechtssicherheit, Formulierungshilfen etc.)
- **Tech-Community** (Input bzgl. Integration, Prompt-Engineering, Automatisierung etc.)

### ⚠️ Bitte beachten (wichtig für Vergabestellen)
Damit **VergabeLab Community** öffentlich nutzbar bleibt, gilt:
* **Keine personenbezogenen Daten** (Namen, Kontaktdaten, Signaturen etc.).
* **Keine Details laufender Vergaben** und keine Betriebs- und Geschäftsgeheimnisse.
* Bitte nur **abstrahierte/anonymisierte Beispiele** („Bieter A/B“, „Projekt X“, „Leistungskategorie Y“).
* Falls interne Freigaben erforderlich sind: **bitte vor Veröffentlichung intern klären**.

### Wege der Mitarbeit

Es gibt drei Hauptwege, wie du dich einbringen kannst:

#### A. Der offene Weg: Discussions (Ideen, Fragen & Erfahrungsaustausch) 💬
Nutze die **"Discussions"** (den Reiter oben), für alles, was noch kein fester Arbeitsauftrag ist. Das ist unser Community-Forum.
- **Ideen einreichen:** Welche Anwendungsfälle fehlen noch (z. B. Bieterfragen & -antworten)?
- **Rechtliche Hinweise:** Gibt es neue Urteile oder Vorschriften, über die wir sprechen müssen?
- **Pilot-Feedback:** Teile deine Erfahrungen aus realen Projekten. Was spart Zeit? Wo entstehen Risiken?
> 👉 **[Direkt zu den Discussions](https://github.com/vergabelab/vergabelab-community/discussions)**

#### B. Der strukturierte Weg: Issues (Konkrete Fehler & Aufgaben) 🎯
Nutze die **"Issues"**, wenn du einen klaren Fehler gefunden hast oder ein konkretes Arbeitspaket vorschlagen möchtest.
- **Fehler melden:** Wo entstehen Missverständnisse oder Halluzinationen in einem bestimmten Prompt?
- **Konkrete Wünsche:** Anfragen für spezifische neue Templates, Leitfäden usw.
> 👉 **[Direkt zu den Issues](https://github.com/vergabelab/vergabelab-community/issues)**

#### C. Der direkte Weg: Pull Requests (Änderungen direkt umsetzen) 🛠️
Du fühlst dich sicher im Umgang mit GitHub? Dann freuen wir uns über direkte Verbesserungsvorschläge via **Pull Request**.
- **Hinweistexte/Systemprompts optimieren:** Bessere Formulierungen für bestehende Dateien.
- **Erweiterungen:** Neue fertige Bausteine für weitere Phasen des Vergabeprozesses hochladen.

**Hinweis:** Beiträge erfolgen standardmäßig per DCO (Signed-off-by). Pull Requests ohne Sign-off werden nicht gemergt (verpflichtender Check: **`DCO / DCO sign-off check`**). Details: [CONTRIBUTING.md](./CONTRIBUTING.md)


---

## 5. Lizenzierung
Dieses Repository enthält überwiegend Textartefakte (Systemprompts/Hinweistexte, Templates, Guides, Muster, Wissensbausteine). Um die Nutzung in Vergabestellen und bei Partnern möglichst reibungsarm zu halten, sind Textartefakte grundsätzlich unter CC BY 4.0 lizenziert. Echte Software-/Tooling-Bestandteile (Code) werden – sofern vorhanden – separat behandelt.

### 5.1 Lizenz-Matrix (Ordner / typische Inhalte → Lizenz → Pflichten)

| Bereich/Ordner | Typische Inhalte | Lizenz | Kernpflichten |
|---|---|---|---|
| prompts/** | Systemprompts, Hinweistexte, Konfigurationstexte | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| wissen/** | Leitfäden, Grundlagen, Wissensbausteine, fachliche Referenzmaterialien | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| templates/** | Mustertexte, Vorlagen, Prüfschemata, Textbausteine | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| guides/** | Handreichungen, Anleitungen, Einbindungshinweise | CC BY 4.0 | Attribution + Hinweis auf Änderungen |
| tooling/** (sofern vorhanden) | Code/Plugins/Skripte/Tools | EUPL 1.2 | Lizenz-/Copyright-Hinweise beibehalten; Bedingungen der EUPL 1.2 beachten |

**Vorrang von Datei-Hinweisen:** 
Soweit eine Datei einen YAML-Frontmatter + SPDX-Kommentar oder einen gleichwertigen Lizenzhinweis enthält, ist dieser für die jeweilige Datei maßgeblich.

### 5.2 Offizielle Lizenztexte

- **CC BY 4.0**: siehe `LICENSES/CC-BY-4.0.txt` sowie die offizielle Veröffentlichung:  
  https://creativecommons.org/licenses/by/4.0/
- **EUPL 1.2**: siehe `LICENSES/EUPL-1.2.txt` sowie die offizielle Veröffentlichung:  
  https://joinup.ec.europa.eu/collection/eupl/eupl-text-11-12
  
### 5.3 Praktische Hinweise:

**CC BY 4.0 (Textartefakte):**
- Bei Veröffentlichung/Weitergabe bitte Attribution (Projektname, Autor, Lizenz, Link) an geeigneter Stelle (z. B. Doku/Impressum/„Über“-Seite/Projektakte).
- Wenn du Inhalte bearbeitest, kennzeichne zusätzlich Änderungen knapp (z. B. „angepasst für Organisation/Abteilung X, Datum“).

**EUPL 1.2 (nur für `tooling/**`, sofern vorhanden):**
- Lizenz- und Urheberhinweise im Quelltext beibehalten.
- Bei Weitergabe, Bearbeitung oder öffentlicher Zugänglichmachung von EUPL-lizenzierten Softwarebestandteilen sind die Bedingungen der EUPL 1.2 zu beachten.

Weitere typische Fragen: siehe **[Lizenz-FAQ](./guides/01_lizenz_faq_de.md)**.

> Hinweis: Diese Hinweise sind eine pragmatische Orientierung. Maßgeblich sind die jeweiligen Lizenztexte sowie die Lizenzzuordnung je Datei.
---

## 6. Projektprinzipien & Fair-Use (nicht Teil der Lizenz)

Rechtlich maßgeblich sind ausschließlich die Lizenztexte und die Lizenzzuordnung je Datei (siehe Abschnitt **[Lizenzierung](#5-lizenzierung)**).  
Die folgenden Punkte sind **keine zusätzlichen Lizenzbedingungen**, sondern beschreiben, was VergabeLab unter einem fairen, community-orientierten Umgang versteht.

### Warum diese Lizenzierung?

Die VergabeLab Community soll in Vergabestellen und bei Partnern möglichst niedrigschwellig nutzbar sein. Deshalb stehen Textartefakte (inkl. Systemprompts/Hinweistexte) grundsätzlich unter **CC BY 4.0.** Daraus resultiert  eine klare Attributionspflicht, aber wenig Reibung innerhalb von Compliance-Prozessen.

Für echten Code/Tooling (sofern vorhanden) ist eine separate Lizenzierung vorgesehen (**EUPL 1.2**), um Softwarebestandteile sauber von Textartefakten zu trennen.

### Was wir als faire Nutzung verstehen

- **Transparenz statt "Black-Box"**  
  Wenn VergabeLab-Prompts/Hinweistexte in eigenen Systemen **verändert** und anschließend Dritten bereitgestellt werden, ist es im Sinne des Projekts, Verbesserungen wieder zugänglich zu machen (z. B. via Fork/Pull Request oder eigene Veröffentlichung unter kompatibler Lizenz).

- **Keine "stille" Übernahme als verdeckter Produktbestandteil**  
  VergabeLab soll nicht als unsichtbare Produktkomponente „mitlaufen“. Wer Inhalte produktiv – auch kommerziell – nutzt, sollte
  - die Herkunft transparent machen (Hinweis auf VergabeLab/Projekt-URL), und
  - Erkenntnisse/Verbesserungen möglichst zurückspielen.

- **Community first**  
  VergabeLab ist als Community-Projekt angelegt. Für Organisationen, die darüber hinaus Unterstützung benötigen (z. B. Anpassungen, Integrationskonzepte, Schulungen, Support), können Leistungen separat vertraglich vereinbart werden.

- **Respekt vor Urheberschaft und Lizenzhinweisen**  
  Bitte entferne bei eigenen Veröffentlichungen keine Hinweise auf Herkunft und Lizenz. Wo du darauf aufbaust, sollte erkennbar sein
  - dass die Basis aus der VergabeLab Community stammt, und
  - unter welcher Lizenz die abgeleiteten Inhalte stehen.
---

## 7. Empfohlener Urheberhinweis / Attribution
Soweit im Einzelfall nichts anderes vereinbart wird, freuen wir uns bei Nutzung von VergabeLab-Inhalten (z. B. in Custom GPTs, Fachverfahren oder Dokumentationen) über folgenden Hinweis:

```text
Basierend auf Bausteinen aus dem Open-Knowledge- und Open-Source-Projekt:
VergabeLab Community – KI-Bausteine für Vergabestellen
© 2026 Okan Doğan.
Lizenz: CC BY 4.0, sofern in der jeweiligen Datei nicht anders angegeben.
Für Code/Tooling im Ordner tooling/** gilt – sofern dort ausgewiesen – EUPL 1.2.
Projekt/Quelle: https://github.com/VergabeLab/vergabelab-community
Hinweis zu Änderungen: ggf. „Inhalte angepasst für [Organisation/Projekt], [Datum]“.
```
Der Hinweis kann z. B. in der technischen Dokumentation, im Impressum, in einer „Über dieses System“-Seite oder im Projektdokument platziert werden.

---
## 8. Über den Initiator
VergabeLab Community wurde von [Okan Doğan](https://github.com/raokandogan) ins Leben gerufen und mit ersten Prompts und Textbausteinen initial befüllt.

Als Fachanwalt für IT-Recht mit Schwerpunkt im Vergaberecht arbeitet Okan an der Schnittstelle von Digitalisierung, Legal Tech und öffentlicher Beschaffung. Sein Ziel ist es, öffentlichen Auftraggebern, Sektorenauftraggebern und Konzessionsgebern einen sicheren, rechtlich fundierten und pragmatischen Einstieg in die Nutzung von Künstlicher Intelligenz zu ermöglichen. 

Das Projekt ist aus der Überzeugung heraus entstanden, dass die Herausforderungen der KI-Adaption bei der öffentlichen Hand durch offenen Wissenstransfer und eine starke Community besonders gut angegangen werden können. Vernetz dich gerne oder tausche dich direkt aus: 
* **GitHub:** [@raokandogan](https://github.com/raokandogan)
* **LinkedIn:** [/ra-okan-dogan](https://de.linkedin.com/in/ra-okan-dogan)
* **Kanzlei:** [doganpfahler.de](https://doganpfahler.de/team/rechtsanwalt-okan-dogan/)

---
## Meldung von Rechts- und Urheberrechtsverletzungen (Notice and Takedown)

VergabeLab Community ist ein Open-Knowledge- und Open-Source-Projekt, das vom Erfahrungswissen und den Beiträgen seiner Nutzerinnen und Nutzer lebt. Wir nehmen den Schutz von Urheberrechten und geistigem Eigentum sehr ernst.

Alle Mitwirkenden bestätigen im Rahmen des DCO und der Projektregeln, dass sie nur Inhalte beisteuern, an denen sie die erforderlichen Rechte besitzen oder die sie rechtmäßig unter der jeweiligen Projektlizenz einreichen dürfen. Eine vollständige proaktive Prüfung sämtlicher Beiträge auf Rechte Dritter kann nicht erfolgen. Nachvollziehbaren Hinweisen auf mögliche Rechtsverletzungen gehen wir unverzüglich nach.

### So meldest du eine Rechtsverletzung

Solltest du der Ansicht sein, dass ein in diesem Repository veröffentlichter Textartefakt (Prompt, Musterdokument, Leitfaden etc.) deine Urheberrechte oder die Rechte deiner Organisation verletzt, bitten wir um einen kurzen, formlosen Hinweis. **Wir handeln unverzüglich.**

Bitte sende eine E-Mail an **kontakt [at] vergabelab [dot] de** mit folgenden Informationen:

* Einen direkten Link (URL) zu der betroffenen Datei oder dem Code-Abschnitt in diesem Repository.
* Eine kurze Erläuterung, warum der Inhalt deine Rechte verletzt (z. B. "Text wurde 1:1 aus unserem proprietären Leitfaden kopiert").
* Einen Nachweis deiner Urheberschaft oder Rechteinhaberschaft (z. B. Link zum Originaldokument).

**Ablauf:** Nachdem uns eine nachvollziehbare Beschwerde vorliegt, werden wir den betroffenen Inhalt im Sinne eines "Notice and Takedown"-Verfahrens unverzüglich entfernen oder unsichtbar schalten, bis der Sachverhalt abschließend geklärt ist. Von sofortigen anwaltlichen Abmahnungen bitten wir zur Schonung unnötiger Kosten und Ressourcen im Sinne der Open-Source-Community abzusehen.
