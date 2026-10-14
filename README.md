# Windschatten

Community-Plattform für Triathletinnen und Triathleten. Start in Wien, danach DACH.

Arbeitstitel war 3com, der Name ist seit 13.10.2026 entschieden (D-031).

**Kurzfassung:** Hochvolumiges Ausdauertraining ist ein Mannschaftssport, der als Einzelsport
betrieben wird. Acht bis fünfzehn Stunden pro Woche, über Monate, fast alles allein. 3com macht
aus geplanten Einzeleinheiten gemeinsame Einheiten.

**Zielgruppe:** nicht eine Sportart, sondern eine Trainingslast. Acht Stunden pro Woche oder
mehr, strukturiert, mit einem Renndatum. Triathlon ist der Kern, Hyrox, Trail und Ultra sowie
Marathon mit strukturiertem Plan gehören dazu.

**Das Kernproblem:** nicht fehlende Gelegenheit, sondern zweidimensionale Peer-Knappheit. Man
kennt kaum jemanden, der gleichzeitig ähnlich leistungsfähig ist **und** an diesem Tag dieselbe
Art von Einheit im Plan hat. Intensität gehört zur Einheit, Niveau gehört zum Menschen. Nur
Dichte löst das, kein Werkzeug.

---

## Status

| Punkt | Stand |
|---|---|
| Phase | v1.0. Konzept eingefroren. **Es wird gefahren, nicht mehr geschrieben.** |
| Gründer | zwei, gleiche Anteile. Einer BD, Vertrieb und Community, einer Produkt und Technik |
| Ambitionsniveau | entschieden: Gruppe mit Werkzeug, kein Unternehmen (D-034) |
| Erster Termin | **Sa 17.10.2026, 08:00, Reichsbrücke Nord.** Ein Anker, nicht drei (D-033) |
| App | gebaut und im Betrieb, Quelltext in `app/windschatten.html` (D-032) |
| Terminmodell | zwei Ebenen: fixer Anker am Wochenende, bewegliche Einheiten unter der Woche (D-035) |
| Nächster Schritt | acht Nachrichten verschicken, siehe `docs/18-start-kit.md` |
| Geld | **Keine Monetarisierung (D-034).** Kosten werden durch die geteilt, die teilnehmen |
| Markt Wien | 5.000 bis 12.000 Personen (Schätzung, siehe 04) |
| Name | **Windschatten**, entschieden (D-031). Domain noch nicht geprüft |
| Datum | 2026-10-13 |

## Navigation

| Dokument | Inhalt |
|---|---|
| [docs/00-vision.md](docs/00-vision.md) | Nordstern, Ambition, Prinzipien |
| [docs/01-problem-und-nutzer.md](docs/01-problem-und-nutzer.md) | Problem, Personas, Jobs to be done |
| [docs/02-loesungskonzept.md](docs/02-loesungskonzept.md) | Drei-Schichten-Modell, Kernloop, Abgrenzung |
| [docs/03-geschaeftsmodell.md](docs/03-geschaeftsmodell.md) | Erlöslogik, Unit Economics, ehrliche Lücke |
| [docs/04-markt-und-wettbewerb.md](docs/04-markt-und-wettbewerb.md) | Marktgröße, Wettbewerbsmatrix, Differenzierung |
| [docs/05-product-mvp-spec.md](docs/05-product-mvp-spec.md) | Feature-Scope MVP (EN) |
| [docs/06-tech-architecture.md](docs/06-tech-architecture.md) | Stack, Datenmodell, Integrationen (EN) |
| [docs/07-go-to-market.md](docs/07-go-to-market.md) | Cold Start, Seeding, Rituale, Partner |
| [docs/08-naming.md](docs/08-naming.md) | Namensbewertung, Longlist, Shortlist |
| [docs/09-risiken-und-offene-fragen.md](docs/09-risiken-und-offene-fragen.md) | Top-Risiken, offene Entscheidungen |
| [docs/10-roadmap.md](docs/10-roadmap.md) | 90-Tage-Plan, Meilensteine, Abbruchkriterien |
| [docs/11-interview-leitfaden.md](docs/11-interview-leitfaden.md) | Leitfaden für die 15 Validierungsinterviews |
| [docs/12-startup-council.md](docs/12-startup-council.md) | Fünf Perspektiven, Debatte, fünf Änderungen |
| [docs/13-bd-playbook.md](docs/13-bd-playbook.md) | Slot-Verhandlung und die ersten 30 Menschen, mit Vorlagen |
| [docs/14-startup-council-runde-2.md](docs/14-startup-council-runde-2.md) | Zweite, härtere Council-Runde: Distanzen, Serien-Obergrenze, Konzeptstopp |
| [docs/15-design-und-ci.md](docs/15-design-und-ci.md) | Markenhaltung, Bildzeichen, Farbe, Typografie, Tonalität, Kanäle |
| [web/index.html](web/index.html) | Website-Entwurf inkl. App-Teaser, eine Seite, ohne Abhängigkeiten |
| [app/windschatten.html](app/windschatten.html) | **Die App.** Terminbrett mit geteilter Datenbank, läuft |
| [web/app-prototyp.html](web/app-prototyp.html) | Klickbarer Prototyp, überholt durch `app/` |
| [docs/16-wettbewerb-realitaetscheck.md](docs/16-wettbewerb-realitaetscheck.md) | Wer es schon gibt, warum die scheitern, was das heißt |
| [docs/17-community-playbook.md](docs/17-community-playbook.md) | Lehren aus parkrun, November Project, HYROX und anderen |
| [web/designsystem.html](web/designsystem.html) | Designsystem visuell: Bildzeichen, Palette, Typo, Vorlagen |
| [docs/18-start-kit.md](docs/18-start-kit.md) | **Die fertigen Texte für die nächsten zehn Tage** |
| [decisions/DECISIONS.md](decisions/DECISIONS.md) | Entscheidungslog |

## Sprachkonvention

Strategie- und Community-Dokumente auf Deutsch, weil der Markt und die Ansprache deutschsprachig
sind. Technische Dokumente (05, 06) auf Englisch, weil dort gebaut wird.

## Kennzeichnung von Zahlen

Jede Zahl in diesem Repo ist als **[Beleg]** oder **[Hypothese]** markiert. Hypothesen sind nicht
recherchiert, sondern Annahmen, die vor einer Investitionsentscheidung zu prüfen sind. Die
Prüfmethode steht jeweils dabei.
