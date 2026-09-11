# 10 Roadmap

Datiert auf den realen Kalender. Ausgangspunkt: September 2026. Gemeinsames Zielrennen beider
Gründer: Sommer 2027. Beide trainieren ganzjährig und rotieren zwischen Hyrox, Trail und Ultra
und Langdistanz.

## Das Prinzip

Gebaut wird im Winter, betrieben wird im Sommer. Nicht weil ihr im Winter weniger trainiert,
sondern weil draußen wenig passiert und die Abende planbar sind. Wer im Mai 2027 noch Code
schreibt, arbeitet gegen seine eigenen Trainingsumfänge.

## Phasenübersicht

| Phase | Zeitraum | Ziel | Abbruchkriterium |
|---|---|---|---|
| **Anker draußen** | Sep bis Okt 2026 | 3 laufende Anker, 40 bis 60 Personen, Winterslots gesichert | Verhältnis Zusage zu Erscheinen unter 50 Prozent nach 6 Wochen |
| **Winter und Bau** | Nov 2026 bis Feb 2027 | Winterprogramm als Kernangebot, PWA gebaut | Winterprogramm füllt sich nicht, dann nicht fertigbauen |
| **Launch** | Mär bis Apr 2027 | App im Betrieb, alle Serien migriert, neue Gastgeber angeworben | unter 2 fremdgeführten Serien nach 8 Wochen |
| **Saison und Betrieb** | Mai bis Jul 2027 | Kein Bauen. 5 fremdgeführte Serien. Herbstprogramm steht. | 5 Gastgeber nicht erreicht, dann bleibt es ein gut organisiertes Hobby |
| **Formatwechsel** | Aug bis Sep 2027 | Community trägt den Wechsel von Langdistanz zu Trail und Hyrox mit | unter 30 Prozent der Mitglieder wechseln die Disziplin (Hypothese H3 widerlegt) |
| **Jahr 2** | ab Okt 2027 | Erste Erlöse, Entscheidung über Ambitionsniveau, Test zweite Stadt | Stadt zwei funktioniert nur mit euch vor Ort, dann Pfad Verein wählen |

## Phase 1: Anker draußen (Sep bis Okt 2026)

Solange das Wetter hält. Kein Produkt, nur WhatsApp und Verlässlichkeit.

### Woche 1, ab 11.09.2026

- [ ] Jeder von euch listet 20 Namen aus dem eigenen Netzwerk
- [ ] Ergebnisverantwortung aufteilen (Tabelle in `07-go-to-market.md`), ein Name pro Zeile
- [ ] Anteilsaufteilung und Ausstiegsfall schriftlich klären
- [ ] WhatsApp-Community und Strava-Club anlegen
- [ ] **Erste Samstagsausfahrt für 19.09.2026 terminieren**, Startpunkt fix, zwei Tempogruppen angekündigt
- [ ] Startlisten sichten: Ironman Austria, 70.3 St. Pölten, Vienna Triathlon, Hyrox Vienna, VCM Marathondistanz, österreichische Trail- und Ultrarennen

### Woche 2 bis 3

- [ ] Erste Samstagsausfahrt durchführen, egal wie viele kommen
- [ ] Dienstagsintervalle ab 22.09.2026 starten
- [ ] **Winterslots ansprechen.** Zuerst das Billige: Gym oder Halle für Kraft- und
      Hyrox-Einheiten, oft mit Randzeitenkapazität. Parallel das Teure: Indoor-Cycling-Studio und
      Hallenbad-Bahn, jeweils als feste Serie über die ganze Saison, nicht als Einzeltermine
- [ ] 10 Gespräche mit Teilnehmenden nach den Einheiten, Leitfaden in `11-interview-leitfaden.md`
- [ ] Domainprüfung für die drei Namen der Shortlist

### Woche 4 bis 6

- [ ] Schwimmeinheit starten
- [ ] Ein Coach für die erste Special Session gewinnen, Durchreichmodell
- [ ] Erstes Gespräch mit einem Radshop über Startpunkt und Raum
- [ ] Erkennungszeichen bestellen: Aufkleber oder Kappe, nur durch fünfmaliges Erscheinen erhältlich
- [ ] **Startlisten über alle sechs Formate auswerten**, nach Wiener Postleitzahlen filtern.
      Das ersetzt die Marktschätzung in 04 durch echte Zahlen
- [ ] **Zwischenfazit: Verhältnis Zusage zu Erscheinen.** Unter 50 Prozent wird nichts gebaut

### Woche 7 bis 8, Ende Oktober

- [ ] Saisonauftakt-Abend planen (Vortrag, kein Markenevent)
- [ ] Winterprogramm terminieren und ankündigen
- [ ] **Go oder No-Go für den Bau.** Bedingungen: Zusage-zu-Erscheinen über 50 Prozent,
      mindestens 25 Personen aktiv, mindestens ein Winterslot gesichert
- [ ] Klären: hat einer von euch ein Hyrox-Rennen zwischen November und Februar? Wenn ja, baut
      der andere in dieser Phase den Hauptteil
- [ ] Finaler Name entschieden

## Phase 2: Winter und Bau (Nov 2026 bis Feb 2027)

Draußen passiert wenig, die Abende sind planbar. Das ist das Bauzeitfenster, unabhängig davon,
wie viel ihr in dieser Phase selbst trainiert. Falls einer von euch ein Hyrox-Rennen im Winter
hat, trägt der andere den Hauptteil des Baus.

**Betrieb parallel:**
- Die drei Anker laufen unverändert weiter, ganzjährig an derselben Stelle im Kalender
- Kraft- und Hyrox-Einheiten als Winterschwerpunkt
- Indoor-Cycling-Serie und Hallenbad-Bahn, sofern verhandelt
- Saisonauftakt-Abend im November
- Erste Coach-Sessions

**Bau, geschätzt 10 bis 15 Stunden pro Woche auf zwei Köpfe:**

| Zeitraum | Lieferung |
|---|---|
| Nov | Schema, Auth, Onboarding, Tempogruppen |
| Dez | Serien anlegen, Occurrences, Commit und Abmeldung |
| Jan | Host-Ansicht, Übernahme einer Serie, Erinnerungen und Bestätigung |
| Feb | Kuratierte Sessions mit Kapazität und Kosten, Verlässlichkeitsquote, Community-Regeln, geschlossene Beta |

Umfang und Datenmodell in `05-product-mvp-spec.md` und `06-tech-architecture.md`. Der Umfang ist
gegenüber dem ersten Entwurf etwa halbiert, weil das Ad-hoc-Board entfällt.

## Phase 3: Launch (Mär bis Apr 2027)

- [ ] Geschlossene Beta mit der bestehenden Gruppe, zwei Wochen
- [ ] Alle Serien auf die App migrieren, WhatsApp nur noch für Kurzfristiges
- [ ] Öffentlicher Launch in Wien
- [ ] **Gastgeber anwerben.** Das ist ab hier die wichtigste Aufgabe, nicht Nutzerakquise
- [ ] Outdoor-Saison startet, Serien entsprechend umstellen

## Phase 4: Saison und Betrieb (Mai bis Jul 2027)

**Ab hier wird nicht mehr gebaut.** Eure Trainingsumfänge liegen bei 15 bis 20 Stunden pro
Woche. Was jetzt nicht fertig ist, wird es bis August nicht.

- [ ] Fünf Serien werden von anderen geführt (M5, die wichtigste Zahl im ganzen Plan)
- [ ] **Herbstprogramm im Mai planen, nicht im August**
- [ ] Trainingswochenende oder Camp, hohe Bindungswirkung, trägt sich selbst
- [ ] Rennwoche als gemeinsames Community-Erlebnis gestalten, auch für die, die nicht starten

## Phase 5: Formatwechsel (Aug bis Sep 2027)

In v0.2 war das die gefährlichste Phase des Projekts. Durch das ganzjährige Training beider
Gründer ist sie deutlich entschärft: nach dem Zielrennen folgt bei euch das nächste Format, kein
Loch. Was hier stattdessen geprüft wird, ist Hypothese H3.

- [ ] Die fünf fremdgeführten Serien laufen weiter, auch in eurer Regenerationswoche
- [ ] Schwerpunkt der Zusatzformate wechselt auf Trail und Ultra
- [ ] **Messung H3:** Wie viele Mitglieder wechseln die Disziplin mit, statt abzuspringen?
      Unter 30 Prozent war die Verbreiterung ein Rechenfehler.
- [ ] Eine Veranstaltung, die keine Fitness braucht: Saisonauswertung, Planung 2028
- [ ] **Entscheidung Ambitionsniveau** anhand realer Daten, siehe `00-vision.md`

## Meilensteine mit Zahlen

| Meilenstein | Kennzahl | Termin |
|---|---|---|
| M1 Ritual trägt | Zusage zu Erscheinen über 50 Prozent über 6 Wochen | Ende Okt 2026 |
| M2 Winter gesichert | 2 Winterslots als Serie über die Saison gebucht | Ende Okt 2026 |
| M3 App live | PWA in Produktion, alle Serien migriert | Ende Mär 2027 |
| M4 Delegation beginnt | 2 Serien von anderen geführt | Ende Apr 2027 |
| M5 Ausfallsicherheit | **5 Serien von anderen geführt** | Ende Mai 2027 |
| M6 Formatwechsel trägt | über 30 Prozent der Mitglieder wechseln über die Saison die Disziplin | Sep 2027 |
| M7 Erster Euro | Take Rate oder Partnerdeal | Winter 2027/28 |
| M8 Reproduzierbar | Zweite Stadt, 8 Wochen stabil ohne euch vor Ort | 2028 |

M5 ist der wichtigste Meilenstein der gesamten Roadmap, weil er als einziger die Frage
beantwortet, die über das Ambitionsniveau entscheidet: läuft 3com ohne euch? M6 ist der
zweitwichtigste, weil er die Verbreiterung auf Ausdauer-Generalisten bestätigt oder widerlegt.

## Definition "aktiver Nutzer"

> Hat in den letzten 30 Tagen an mindestens einer Einheit teilgenommen oder eine geführt.
> Registrierung, App-Öffnung oder Feed-Konsum zählen nicht.

## Was diese Roadmap absichtlich nicht tut

Sie plant nicht über den September 2027 hinaus. Die Ambitionsfrage wird bei M6 mit realen Daten
beantwortet. Alles, was heute über Jahr 2 hinaus geschrieben würde, wäre Fiktion.
