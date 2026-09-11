# Entscheidungslog

Jede getroffene Richtungsentscheidung mit Datum, Begründung und Bedingung für eine
Wiedervorlage. Wer später einsteigt, versteht hier in fünf Minuten, warum die Dinge so sind.

---

## D-001 Ambitionsniveau bleibt offen

**Datum:** 2026-09-11
**Entscheidung:** Keine Vorabfestlegung auf Verein, Bootstrapped Business oder skalierbare
Plattform. Die Entscheidung fällt nach dem MVP anhand von Daten.
**Begründung:** Der Wiener Markt ist zu klein, um vorab beurteilt zu werden, und die
Skalierbarkeitsfrage lässt sich nur durch den Versuch in einer zweiten Stadt beantworten.
**Wiedervorlage:** Meilenstein M6 (120 aktive Nutzer) und M7 (zweite Stadt).

---

## D-002 Eigene PWA statt Zero-Code-Pilot

**Datum:** 2026-09-11
**Entscheidung:** Es wird von Anfang an ein eigenes Produkt gebaut, keine Kombination aus
WhatsApp, Luma und Strava als dauerhafte Lösung.
**Begründung:** Sauberer Markenaufbau, volle Kontrolle über die Kernmechanik (Tempo-Matching),
die mit Standardwerkzeugen nicht abbildbar ist.
**Bekanntes Risiko:** Das Produkt startet in einen leeren Raum.
**Kompensation:** Rituale starten in Woche 1 über WhatsApp, die App landet in Woche 8 bis 10 und
erbt eine bestehende Gruppe. Die Bauentscheidung wird in Woche 4 anhand der Wiederkehrrate
nochmals überprüft.
**Wiedervorlage:** Woche 4.

---

## D-003 Athletinnen und Athleten zahlen nicht

**Datum:** 2026-09-11
**Entscheidung:** Kein Mitgliedsbeitrag, kein Zugangsentgelt. Erlöse aus Brand-Partnerschaften
und einem angebotsseitigen Marktplatz.
**Begründung:** Die Eintrittshürde in eine Community ist die Zahlungsaufforderung. Bei einem
Produkt, dessen Wert an der Dichte hängt, ist Reichweite wichtiger als früher Umsatz.
**Bekanntes Risiko:** Nahezu null Umsatz im ersten Jahr.
**Kompensation:** Durchreichmodell ohne Marge für Curated Sessions ab Monat 1, damit früh ein
Zahlungsvorgang und Preissensitivitätsdaten existieren.
**Wiedervorlage:** Bei circa 500 aktiven Nutzern in einer Stadt, dann als freiwilliger
Supporter-Tier, nicht als Zugangsschranke.

---

## D-004 3com bleibt Arbeitstitel

**Datum:** 2026-09-11
**Entscheidung:** Weiterarbeiten unter 3com, finaler Name bis Woche 8. Longlist und
Prüfprotokoll in `docs/08-naming.md`.
**Begründung:** Der Name hat erhebliche Schwächen bei Auffindbarkeit und Bedeutungstransport
sowie ein markenrechtliches Restrisiko durch die frühere 3Com Corporation. Ein Namenswechsel
vor dem Launch kostet nichts, danach viel.
**Empfehlung der Shortlist:** Windschatten, Wechselzone, Kadenz.
**Wiedervorlage:** Woche 8, vor dem App-Launch.

---

## D-005 Keine Direktnachrichten in v1

**Datum:** 2026-09-11
**Entscheidung:** Nur Gruppenchat pro Session, keine 1:1-Nachrichten zwischen Nutzern.
**Begründung:** Moderationsaufwand und das Risiko, dass die Plattform als Dating-Umfeld
wahrgenommen wird. Das würde die weibliche Zielgruppe kosten, und damit die Hälfte des Marktes.
**Wiedervorlage:** Wenn Moderationskapazität existiert, frühestens ab 300 aktiven Nutzern.

---

## D-006 Multi-City im Datenmodell ab Tag eins

**Datum:** 2026-09-11
**Entscheidung:** `city_id` auf Nutzern und Sessions von Beginn an, in der Oberfläche aber
verborgen.
**Begründung:** Der Wiener Markt trägt kein Geschäft. Die Migration eines
Einzelstadt-Schemas ist ein vermeidbarer Aufwand.
**Wiedervorlage:** keine.

---

## D-007 Sprachkonvention im Repo

**Datum:** 2026-09-11
**Entscheidung:** Strategie- und Community-Dokumente auf Deutsch, technische Dokumente auf
Englisch.
**Begründung:** Markt und Ansprache sind deutschsprachig, Entwicklung ist englischsprachig.
**Wiedervorlage:** bei Internationalisierung.

---

## D-008 Zwei Gründer, beide mit eigenem Bedarf

**Datum:** 2026-09-11
**Entscheidung:** 3com wird von zwei Gründern getragen, die beide selbst im Aufbau auf eine
Langdistanz im Sommer 2027 sind.
**Begründung:** Der Grenzaufwand, andere zur eigenen Einheit mitzunehmen, liegt nahe null. Damit
ist das Angebot ohne Zusatzaufwand gesichert und das Cold-Start-Risiko weitgehend neutralisiert.
Gleichzeitig verdoppelt sich das verfügbare Zeitbudget von 416 auf rund 830 Stunden pro Jahr.
**Bekanntes Risiko:** Gleiches Rennen bedeutet gleichzeitiger Ausfall nach dem Rennen (R10) und
eine gemeinsame Blindstelle gegenüber Einsteigern (R11).
**Rollen:** Beide alles, aufgeteilt nach Zeit, aber mit einem Namen pro wiederkehrendem Ergebnis.
**Wiedervorlage:** Anteile und Ausstiegsfall schriftlich vor Phase 1.

---

## D-009 Wiederkehrende Serien statt Ad-hoc-Board in v1

**Datum:** 2026-09-11
**Entscheidung:** Das Posten einzelner Ad-hoc-Sessions fliegt aus v1. Der MVP ist ein Werkzeug
für wiederkehrende Serien mit Zusage, Gastgeberrolle und Erinnerung.
**Begründung:** Gemeinsames Training braucht vier gleichzeitige Übereinstimmungen: Zeit, Ort,
Disziplin, Tempo. Unter etwa 250 aktiven Nutzern pro Stadt sind die meisten Kombinationen leer.
Wiederkehrende Termine ersetzen Zufall durch Konvention. Zusätzlich sind alle vier geplanten
Startformate ohnehin wiederkehrend und zentral organisiert.
**Wirkung:** Bauumfang etwa halbiert.
**Wiedervorlage:** Bei circa 250 aktiven Nutzern in einer Stadt.

---

## D-010 Tempo als Name, nicht als Zahl

**Datum:** 2026-09-11
**Entscheidung:** Drei benannte Gruppen auf der Oberfläche: Kaffeefahrt, Tempo, Vollgas. Das
numerische Band existiert nur im Hintergrund.
**Begründung:** Sich selbst in ein Intervall einzutragen fühlt sich an wie eine Einstufung.
Sich zu einer benannten Gruppe zu bekennen fühlt sich an wie eine Einladung. Die Ränder
überlappen bewusst, wer dazwischen liegt, bekommt beide Gruppen angeboten.
**Wiedervorlage:** keine.

---

## D-011 Der Gastgeber ist der primäre Nutzer

**Datum:** 2026-09-11
**Entscheidung:** Jede Produktentscheidung wird daran gemessen, ob sie es jemand anderem
leichter macht, eine Einheit zu übernehmen und zu führen.
**Begründung:** Die bindende Einschränkung sind Gründerstunden. Der einzige Hebel dagegen ist
Delegation des Gastgebens. Zusätzlich ist es die einzige Absicherung gegen das Post-Race-Loch
im August 2027.
**Messgröße:** fünf fremdgeführte Serien bis Ende Mai 2027 (M5).
**Wiedervorlage:** keine.

---

## D-012 Kein Markenevent zum Start

**Datum:** 2026-09-11
**Entscheidung:** Der geplante Kick-off findet ohne Markenpartner statt. Stattdessen ein
Saisonauftakt-Abend im November mit inhaltlichem Vortrag durch einen respektierten Coach.
**Begründung:** Die ersten dreißig Menschen prägen die Kultur. Ein Produktsampling als erstes
gemeinsames Erlebnis erzeugt ein Publikum, keinen Stamm. Eine Marke, die zu diesem Zeitpunkt
zusagt, tut es als Gefallen und ist damit für den späteren, wertvolleren Moment verbrannt.
**Ausnahme:** Ein lokaler Radshop, der Raum stellt und genannt wird, ist Nachbarschaft und kein
Sponsoring.
**Wiedervorlage:** zweiter Winter, also ab Herbst 2027.

---

## D-013 Bauen in der Grundlagenphase

**Datum:** 2026-09-11
**Entscheidung:** Die App wird zwischen November 2026 und Februar 2027 gebaut. Ab Mai 2027 wird
nicht mehr entwickelt, nur betrieben.
**Begründung:** Die Periodisierung der Gründer ist der verlässlichste Kalender, den das Projekt
hat. Im Winter sind die Abende planbar und die mentale Last niedrig. In der spezifischen Phase
ab Mai liegen die Trainingsumfänge bei 15 bis 20 Stunden pro Woche, dann ist kein Bauen möglich.
**Wiedervorlage:** keine.

---

## D-014 Abgrenzung über Trainingslast statt über Sportart

**Datum:** 2026-09-11
**Entscheidung:** 3com richtet sich an Ausdauer-Generalisten, triathlon-verankert. Die Grenze
verläuft bei **acht Stunden Training pro Woche oder mehr, strukturiert, mit einem Renndatum**.
Hyrox, Trail und Ultra, Marathon mit strukturiertem Plan gehören dazu. Gelegenheitssport nicht.
**Begründung:** Der gemeinsame Nenner zwischen Ironman, UTMB und Hyrox ist nicht die Disziplin,
sondern die Last, die Terminlogik und die Sprache. Der bedienbare Markt in Wien verdreifacht
sich dadurch grob auf 5.000 bis 12.000 Personen, und die Saisonalität verschwindet. Beide
Gründer sind selbst Generalisten und damit ganzjährig glaubwürdig.
**Preis:** Identität. Eine Kategorie hält keinen Stamm zusammen (Risiko R13). Der Ausschluss des
Gelegenheitssportlers ist deshalb wichtiger als die Aufnahme des Trailläufers: er hält Niveau
und Sprache intakt.
**Messgröße:** Hypothese H3 in 01, geprüft über den Saisonwechsel im Sommer 2027 (Meilenstein M6).
**Wiedervorlage:** September 2027.

---

## D-015 Anker konstant, Zusatzformate saisonal

**Datum:** 2026-09-11
**Entscheidung:** Die drei wöchentlichen Anker stehen ganzjährig an derselben Stelle im
Kalender. Nur die Special Sessions wechseln mit der Saison: Kraft und Hyrox im Winter, Trail im
Frühjahr und Herbst, Freiwasser und lange Ausfahrten im Sommer.
**Begründung:** Der Vorteil liegt in der Kommunikation, nicht in der Logistik. Wer weiß, dass
samstags um acht etwas stattfindet, muss nichts nachschlagen. Ein Kalender, der sich saisonal
umbaut, verliert genau diese Eigenschaft.
**Wiedervorlage:** keine.

---

## D-016 Name muss disziplinoffen sein

**Datum:** 2026-09-11
**Entscheidung:** Alle Namenskandidaten, die auf drei Disziplinen oder auf Triathlon festgelegt
sind, scheiden aus: 3com, Wechselzone, Brick, Tripod, Trico, Trikot, T2.
**Neue Shortlist:** Windschatten, Kadenz, Rudel. Vierter Kandidat zur Prüfung: Grundlage.
**Begründung:** Folge aus D-014. Der Name muss für eine Krafteinheit im Januar genauso
funktionieren wie für eine vierstündige Ausfahrt im Juni. Zusätzlich trägt der Name nach der
Verbreiterung die Zugehörigkeit, die vorher die Sportart geliefert hat. Damit ist er die
dringendste offene Entscheidung, nicht die unwichtigste.
**Wiedervorlage:** Ende Oktober 2026, vor dem Winterprogramm.

---

## D-017 Gleiche Anteile, arbeitsteilige Rollen

**Datum:** 2026-09-11
**Entscheidung:** Anteile werden zu gleichen Teilen geteilt. In der täglichen Arbeit gilt eine
natürliche Teilung: einer eher Business Development, Vertrieb und Community, einer eher Bauen
und Produkt.
**Begründung:** Die Teilung liegt günstig zum Kalender. Von November bis Februar baut der eine,
während der andere Winterslots, Partner und den Saisonauftakt trägt. Die Lastspitzen ergänzen
sich statt sich zu überlappen.
**Auflage:** Der Builder führt auch im Bauzeitfenster mindestens eine Anker-Einheit pro Woche
(Risiko R15). Und: Vesting und Ausstiegsfall schriftlich, auch bei gleichen Anteilen.
**Wiedervorlage:** keine.

---

## D-018 Markenansprache erst ab einer Zahl, nicht ab einem Datum

**Datum:** 2026-09-11
**Entscheidung:** Der erste Markendeal wird erst angegangen, wenn drei Bedingungen gleichzeitig
erfüllt sind: 300 aktive Mitglieder in Wien, mindestens fünf nicht von den Gründern geführte
Serien, und ein Name samt Identität, die einen Sponsor überleben.
**Begründung:** Für Marken wird es erst interessant, wenn die Community existiert. Vorher ist
jedes Gespräch ein Bittgang, und jeder Bittgang verbrennt den Kontakt für den Moment, in dem er
etwas wert wäre. Die Zielgruppe bleibt attraktiv, Glaubwürdigkeit dagegen ist verderblich.
**Wiedervorlage:** sobald alle drei Bedingungen erfüllt sind.
