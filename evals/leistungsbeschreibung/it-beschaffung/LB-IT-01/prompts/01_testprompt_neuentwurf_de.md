---
title: "Testakte LB-IT-01 – Testprompt Neuentwurf Leistungsbeschreibung"
version: "0.1.0"
last_reviewed: "2026-06-15"
status: "initial"
language: "de-DE"
type: "eval"
subtype: "test-prompt"
eval_role: "prompt"
eval_case_id: "LB-IT-01"
predecessor_eval_case_id: "M-IT-01"
relative_date: "T+14 Wochen"
timeline_mode: "relative"
timeline_anchor: "T0 = Eingang der initialen Bedarfsmeldung einschließlich ausgefülltem Bedarfserhebungsbogen beim zentralen Vergabe-/Beschaffungsteam"
data_notice: "vollständig fiktiv; keine echten Personen, Orte, Vergabestellen oder Anbieter"
license: "CC-BY-4.0"
repository_area: "evals/leistungsbeschreibung/it-beschaffung/LB-IT-01/prompts"
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

# Testprompt – Neuentwurf Leistungsbeschreibung

Werte die folgenden Input-Dateien aus:

* `01_uebergabevermerk_markterkundung.md`
* `02_interne_arbeitsgrundlage_leistungsbeschreibung.md`

Nutze außerdem folgende bereitgestellte Strukturreferenz:

* `templates/leistungsbeschreibung/it-beschaffung/01_vorlage_leistungsbeschreibung_it_de.md`

Erstelle daraus einen gegliederten Erstentwurf einer Leistungsbeschreibung für das Vorhaben `SchulServicePortal`.

Der Entwurf soll als interne Arbeitsfassung für die weitere fachliche, technische und vergabefachliche Prüfung nutzbar sein.
