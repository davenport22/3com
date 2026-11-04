# 02 Lösungskonzept

> **Konzeptstand bis Mitte Oktober 2026, wird nicht mehr nachgezogen (D-039).** Was aktuell gilt, steht im README und im Entscheidungslog. Der Arbeitstitel 3com heißt heute Windschatten (D-031).

## Die atomare Einheit: die Session

Alles in 3com hängt an einem einzigen Objekt: **eine geplante Trainingseinheit mit offenen
Plätzen.** Kein Feed, kein Profil, keine Gruppe. Eine Session.

Eine Session hat:
- Disziplin (Schwimmen, Rad, Lauf, Trail, Kraft und Funktional, Koppel, Sonstiges)
- Zeitpunkt und Startort
- **Intensität**, in der Trainingssprache der Zielgruppe: GA1, GA2, Schwelle, Intervall, Long,
  Koppel, Recovery, Wettkampfsimulation. Das ist die Dimension, an der jemand erkennt, ob die
  Einheit zu seinem Plan an diesem Tag passt.
- **Niveaugruppen**, vom Gastgeber gesetzt, konkret in der Einheit der Disziplin
  (zum Beispiel 30 bis 32 km/h, oder 4:30 bis 4:50 pro Kilometer). Ein Korridor, kein Wert.
- Kapazität und Hostmodus (offen, auf Anfrage, geschlossen)
- Optional: Kosten, Coach, Ort mit Buchung

Alles Weitere im Produkt existiert nur, weil es Sessions entstehen lässt, füllt oder nachwirken
lässt.

## Drei Schichten

MECE nach Herkunft des Angebots:

### Schicht 1 Peer Sessions (kostenlos, nutzergeneriert)

Jemand postet, was er ohnehin vorhat. Andere joinen. Kein Geld, kein Veranstalter, keine
Haftung über das hinaus, was auch bei einer privaten Verabredung gilt.

*Funktion im System:* erzeugt Liquidität und Alltagsrelevanz. Das ist das Produkt.

### Schicht 2 Curated Sessions (kuratiert, kostenpflichtig oder kostenbeteiligt)

Von 3com organisiert oder vermittelt: Bahntraining mit Coach, Schwimmbahn mit Technikanalyse,
Indoor-Cycling-Einheit im Winter, Koppeltraining, Trainingslager.

*Funktion im System:* erzeugt Qualität, Verlässlichkeit und den ersten Umsatzpfad. Diese
Sessions finden statt, egal wie viele kommen. Sie sind der Takt, an dem sich die Community
ausrichtet.

### Schicht 3 Brand Events (markenfinanziert)

Nutrition-Testing, Gear-Demo, Laufschuh-Testlauf, Bikefitting-Abend, Neopren-Test am
Saisonstart, Vortragsabend.

*Funktion im System:* Monetarisierung und Community-Erlebnis in einem. Diese Events sind für
Teilnehmende gratis, weil die Marke zahlt.

## Der Kernloop

```
   [ Ich plane meine Woche ]
              |
              v
   [ Ich poste eine Session ]  <----------------+
              |                                 |
              v                                 |
   [ Jemand mit passendem Tempo joint ]         |
              |                                 |
              v                                 |
   [ Wir trainieren gemeinsam ]                 |
              |                                 |
              v                                 |
   [ Kurzer Post danach, Kudos, Foto ]          |
              |                                 |
              v                                 |
   [ Beide sehen: das war gut ]-----------------+
```

Der Loop schließt sich über die Nachbereitung. Ohne den letzten Schritt bleibt es eine
Terminvermittlung. Mit ihm entsteht Bindung, weil sichtbar wird, dass die Community lebt.

## Der Motivations-Layer

Der zweite Wunsch aus dem Briefing: sich gegenseitig über Posts zu Einheiten motivieren.
Wichtig ist die Abgrenzung zu Strava, sonst baut man ein schlechteres Strava.

| Strava | 3com |
|---|---|
| Zeigt geleistete Aktivitäten mit Leistungsdaten | Zeigt geplante Absichten und gemeinsame Momente |
| Vergleich und Wettbewerb (Segmente, KOM) | Verabredung und Zugehörigkeit |
| Global, Follower-basiert | Lokal, Session-basiert |
| Zahlen im Mittelpunkt | Menschen im Mittelpunkt |

### Die zwei Dimensionen, konsequent getrennt

Intensität gehört zur Einheit, Niveau gehört zum Menschen. Diese Trennung ist die wichtigste
Designentscheidung im Produkt, weil die Verwechslung beider Dimensionen die eigentliche Ursache
des Problems ist (siehe H1 in 01).

|  | **Intensität** | **Niveau** |
|---|---|---|
| Gehört zu | der Einheit, aus dem Trainingsplan | dem Menschen, aus seiner Leistungsfähigkeit |
| Wird gesetzt von | dem Gastgeber beim Anlegen | dem Mitglied im Profil, optional aus Strava abgeleitet |
| Ändert sich | täglich | über Monate |
| Beispiel | 4x8min Schwelle | 30 bis 32 km/h im Flachen |

Eine Einheit passt zu dir, wenn beides stimmt. Eine harte Intervalleinheit in der falschen
Niveaugruppe ist genauso unbrauchbar wie eine passende Niveaugruppe in einer Woche, in der dein
Plan Entlastung vorsieht.

### Gemeinsam heißt nicht locker

Ein Grundsatz, der in der Kommunikation nach außen genauso gilt wie im Produkt: **Auch Vollgas
ist gemeinsam besser.** Harte Einheiten sind nicht die unsozialen, sie sind die, bei denen die
Gruppe den größten messbaren Unterschied macht. Windschatten bei hoher Intensität, geteilte
Führungsarbeit, präziseres Tempo auf der Bahn, das Anschwimmen im Wasser, die Wiederholungen im
Kraftraum, die man allein auslässt.

Jede Formulierung, die suggeriert, gemeinsames Training sei das langsamere Training, ist damit
falsch und schadet bei genau der Zielgruppe, auf die es ankommt.

**Designregel:** Im 3com-Feed erscheint keine Einheit ohne sozialen Bezug. Eine Solo-Einheit
wird nicht automatisch importiert und gepostet. Gepostet wird: "waren zu viert bei Regen am
Donauinselring", "Erste 4-Stunden-Ausfahrt der Saison geschafft", "Noch zwei Plätze für
Samstag". Alles andere ist Rauschen und macht den Feed zum Strava-Klon.

Ein leichter Streak- oder Konsistenzmechanismus ist sinnvoll, aber gruppenbezogen, nicht
individuell: "Diese Gruppe war 6 Wochen in Folge samstags unterwegs" schlägt "Du hast 12 Tage
Streak".

## Was 3com explizit nicht ist

Diese Liste ist so wichtig wie das Konzept selbst, weil sie das Produkt vor Aufblähung schützt.

- **Kein Trainingsplan.** Keine Periodisierung, keine Plangenerierung, keine FTP-Tests.
- **Kein Tracking-Ersatz.** Garmin und Strava bleiben, wo sie sind. 3com liest höchstens.
- **Kein Coaching-Marktplatz im Sinne von 1:1-Vermittlung.** Coaches kommen über Sessions ins
  Spiel, nicht über Profile und Suchfilter.
- **Kein Dating.** Klare Community-Regeln nötig, sonst kippt die Wahrnehmung und die weibliche
  Zielgruppe geht verloren. Dieses Risiko ist real und wird in 09 behandelt.
- **Kein Rennveranstalter.** Keine eigenen Wettkämpfe, zumindest nicht in den ersten zwei Jahren.
- **Kein Verein.** Keine Mitgliedschaft, keine Beiträge, keine Funktionärsstruktur.

## Der Jahresrhythmus statt der Saison

Ein reines Triathlonangebot hat in Wien vier bis fünf tote Monate: Radfahren draußen
unattraktiv, Freiwasser unmöglich. Durch die Abgrenzung über Trainingslast statt Sportart
(siehe 01) verschwindet dieses Loch. Es wird zu einem Schwerpunktwechsel.

**Die Anker bleiben konstant, die Zusatzformate wechseln mit der Saison.** Das ist die
Entscheidung: drei feste wöchentliche Termine, die das ganze Jahr an derselben Stelle im
Kalender stehen, plus Special Sessions, die dem Jahreslauf folgen.

| Zeitraum | Anker (konstant) | Zusatzformate |
|---|---|---|
| Nov bis Feb | Lange Einheit, Intervalle, Schwimmen | Hyrox- und Krafteinheiten, Indoor-Cycling-Slots, Hallenbad-Technik, Saisonplanung |
| Mär bis Mai | dieselben drei | Trail und Höhenmeter, erste lange Ausfahrten, Koppeltraining |
| Jun bis Aug | dieselben drei | Freiwasser, lange Ausfahrten, Rennbegleitung |
| Sep bis Okt | dieselben drei | Trail und Ultra, Saisonausklang, Auswertung |

Der Vorteil der konstanten Anker liegt nicht in der Logistik, sondern in der Kommunikation. Wer
weiß, dass samstags um acht etwas stattfindet, muss nichts nachschlagen. Ein Kalender, der sich
saisonal umbaut, verliert genau diese Eigenschaft.

**Der Winter bleibt trotzdem das wertvollste Fenster.** Im Januar ist die Einsamkeit am größten
und die Konkurrenz am geringsten. Wer dann einen Grund hat, um 6:30 aus dem Haus zu gehen,
kommt im Mai auch zur Ausfahrt.
