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
