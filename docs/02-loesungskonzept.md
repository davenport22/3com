# 02 Lösungskonzept

## Die atomare Einheit: die Session

Alles in 3com hängt an einem einzigen Objekt: **eine geplante Trainingseinheit mit offenen
Plätzen.** Kein Feed, kein Profil, keine Gruppe. Eine Session.

Eine Session hat:
- Disziplin (Schwimmen, Rad, Lauf, Koppel, Kraft, Sonstiges)
- Zeitpunkt und Startort
- Trainingsart und Intensität (GA1, Tempo, Intervall, Long, Recovery)
- Tempoband oder Wattband, nicht ein Wert sondern ein Korridor
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

## Das Winterproblem als Chance

Wien hat vier bis fünf Monate, in denen Radfahren draußen unattraktiv und Freiwasser unmöglich
ist. Für einen Outdoor-Community-Ansatz ist das ein saisonales Loch. Für 3com ist es das
stärkste Argument:

Indoor-Training ist die einsamste Phase im Triathlonjahr. Drei Stunden auf der Rolle im Keller
im Januar. Genau hier ist der gemeinsame Indoor-Slot, das Hallenbad-Bahntraining und die
Hallenlaufeinheit am wertvollsten. Ein Start in den Winter hinein ist daher nicht das
schlechtere, sondern das bessere Timing, weil das Problem am größten ist.
