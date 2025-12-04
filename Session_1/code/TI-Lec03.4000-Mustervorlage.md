
# Muster‑Vorlage (Markdown) für Studierende

> **Hinweis:** Diese Vorlage ist zum Ausfüllen gedacht. Ersetzen Sie Platzhalter `_(...)_` und Häkchenkästchen.

## 0. Meta

* **Systemname:** *(…)*
* **Team/Iteration/Datum:** *(…)*

## 1. Business Goals & Value (max. 5)

*

## 2. Functional Overview (Capabilities)

Kurzliste zentraler Fähigkeiten (Verb‑Nomen):

* *(Erheben von …)*
* *(Generieren von …)*
* *(Personalisieren …)*
* *(Exportieren/Teilen …)*

## 3. Business Context (Blackbox‑Tabelle)

| Nachbarsystem | Richtung (In/Out) | Schnittstelle/Protokoll | Zweck |
| ------------- | ----------------- | ----------------------- | ----- |
| *(…)*         | *(…)*             | *(…)*                   | *(…)* |

## 4. Stakeholder & Personas

**Persona‑Schablone**

```
Name/Alias, Alter, Rolle
Ziele (Top‑3):
Schmerzen/Hürden:
Erfolgskriterien/KPIs:
```

Erstellen Sie ≥3 Personas und verlinken Sie daraus Journeys/Stories.

## 5. Constraints

**Organisatorisch:** *(Gesetze, Sprachen, Termine, Teamgrößen, Budget …)*
**Technisch:** *(Technologie‑Vorgaben, Cloud/On‑Prem, Datenhaltung …)*

## 6. Quality Goals (Top‑3) + Messgrößen

* **QG‑1 (#…):** *(Ziel)* → **Metrik:** *(p95, Fehlerquote …)*
* **QG‑2 (#…):** *(…)*
* **QG‑3 (#…):** *(…)*

## 7. Risks & Architectural Hypotheses

* **Annahme/Hypothese A:** *(riskant, teuer, entscheidungsrelevant)*
* **Risiko R1:** *(Auswirkung, Gegenmaßnahme)*

## 8. Solution Strategy (Skizze)

* **Bausteine:** *(Frontend, Backend‑Services, Persistenz …)*
* **Runtime‑Flows:** *(Sequenzen pro Journey)*
* **Deployment:** *(Region, Sicherheitszonen, Observability)*

## 9. KPIs & SLAs

* **T2X:** *(Definition)*
* **p95‑Latenzen:** *(…)*
* **Erfolgsraten:** *(…)*

---

## A. User Journeys (Template)

```
Journey Jx – <Titel>
1) <Schritt 1>
2) <Schritt 2>
3) <Schritt 3>
Messpunkte/KPIs: <z. B. p95, Dauer, Zufriedenheit>
```

Erstellen Sie mind. zwei Journeys (Privat/B2B o. ä.).

## B. User Stories (Template)

```
Als <Rolle> möchte ich <Fähigkeit>, um <Nutzen>.
Akzeptanzkriterien (testbar):
- [ ] Given <Context> When <Action> Then <Outcome>
- [ ] …
```

Erstellen Sie mind. acht Stories; markieren Sie Epic‑Zugehörigkeiten.

## C. Qualitäts‑Szenarien (Template, nach arc42/Q42)

```
<Attribut‑Label>  
Environment: <z. B. 200 gleichzeitige Nutzer:innen>  
Stimulus: <Aktion/Ereignis>  
Response: <Systemverhalten>  
Measure: <p95/p99, Prozent, Dauer>
```

Erstellen Sie mind. fünf Szenarien inkl. Messwerten.

## D. ADR‑Vorlage (Nygard)

```
# ADR‑<Nummer>: <Titel>
Status: Proposed/Accepted/Superseded  |  Datum: YYYY‑MM‑DD
Kontext:
Entscheidung:
Alternativen (mit Gründen):
Konsequenzen (±):
Link zu Tests/Vertragstests/Dokumentation:
```

Pflicht‑ADRs: Austauschbarkeit kritischer Provider, Datenhaltung/Region, Rendering/Export.

## E. Definition of Done (Checkliste)

*

## F. Bewertungsraster (Dozent:in)

| Kriterium                            | 0 | 1 | 2 |
| ------------------------------------ | - | - | - |
| Zielklarheit & Value                 |   |   |   |
| Traceability (Persona→Journey→Story) |   |   |   |
| Qualitätsszenarien (Messbarkeit)     |   |   |   |
| ADR‑Reife (Alternativen/Trade‑offs)  |   |   |   |
| Konsistenz der Architektur‑Skizze    |   |   |   |

---

*Tipps:* Bevorzugen Sie knappe, messbare Aussagen; halten Sie Story‑AK und Quality‑Szenarien eng verzahnt; referenzieren Sie ADR‑Nummern direkt in Stories/Tasks.
