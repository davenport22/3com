# 01 Problem und Nutzer

> **Konzeptstand bis Mitte Oktober 2026, wird nicht mehr nachgezogen (D-039).** Was aktuell gilt, steht im README und im Entscheidungslog. Der Arbeitstitel 3com heißt heute Windschatten (D-031).

Überarbeitet in v0.3 (Abgrenzung über Trainingslast statt Sportart) und in v0.5 (Kernproblem als
zweidimensionale Peer-Knappheit neu gefasst).

## Das Problem in drei Sätzen

Wer auf eine Langdistanz, einen Ultra oder ein Hyrox-Rennen hin trainiert, verbringt acht bis
fünfzehn Stunden pro Woche in strukturierten Einheiten, über Monate, fast immer allein. Der
Großteil dieser Stunden wäre in Gesellschaft besser: die lange Ausfahrt, der lange Lauf, die
Bahneinheit, das Schwimmen, die Krafteinheit im Januar. Das Ergebnis ist ein Feld von Menschen
mit identischem Ziel, identischem Tempo und identischem Wohnbezirk, die monatelang nebeneinander
her trainieren, ohne sich zu kennen.

## Die Abgrenzung: Last statt Sportart

Der gemeinsame Nenner zwischen einem Ironman-Aufbau, einem UTMB-Aufbau und einer
Hyrox-Vorbereitung ist nicht die Disziplin. Es ist:

> **Acht Stunden pro Woche oder mehr, strukturiert, überwiegend allein, mit einem Datum im
> Kalender.**

Wer das tut, hat unabhängig von der Sportart dasselbe Problem, dieselbe Terminlogik und
dieselbe Sprache. Wer zweimal die Woche zum Spaß läuft, hat es nicht, und ist deshalb auch nicht
die Zielgruppe.

Diese Abgrenzung hat vier Folgen:

1. **Der Markt wird zwei- bis dreimal größer**, ohne dass die Identität verwässert (siehe 04).
2. **Die Saisonalität verschwindet.** Hyrox und Kraft im Winter, Trail im Frühjahr und Herbst,
   Rad und Freiwasser im Sommer. Es gibt keine tote Jahreszeit mehr, nur einen Wechsel im
   Schwerpunkt.
3. **Die Gründer sind glaubwürdig über das ganze Jahr**, weil sie selbst zwischen den Formaten
   rotieren und jede Einheit mitgehen können.
4. **Der Name 3com wird endgültig falsch**, weil die Drei auf drei Disziplinen festgelegt ist.
   Dasselbe gilt für die Shortlist-Option Wechselzone (siehe 08).

Die Verankerung bleibt trotzdem triathlon-nah: Triathlon ist das Format mit der höchsten
Trainingslast, der stärksten Sprache und der klarsten Zugehörigkeit. Es ist der Kern, nicht die
Grenze.

## Warum das Problem heute nicht gelöst ist

| Bestehende Lösung | Warum sie das Problem nicht löst |
|---|---|
| Triathlonverein | Feste Zeiten, Mitgliedsbeitrag, Lizenzkultur. Passt schlecht zum Berufstätigen, der Dienstag kurzfristig doch kann. Und deckt nur eine Sportart ab. |
| Hyrox-Gym oder Box | Löst Kraft und Format, aber nicht die langen Ausdauereinheiten drumherum. |
| Lauftreff, Trailgruppe | Eindisziplinär, oft ohne Leistungsdifferenzierung, selten mit Renndatum im Blick. |
| Strava Club | Rückblickend. Zeigt, was jemand gemacht hat, nicht was jemand vorhat. Keine Koordination. |
| WhatsApp-Gruppe | Funktioniert bis circa 30 Leute, danach Lärm. Kein Tempo-Matching, keine Historie, kein Onboarding. |
| Trainingsplan-Apps (TrainingPeaks, Intervals.icu, MOTTIV) | Lösen die Planung, nicht die Gesellschaft. Explizit einzelsportlich gedacht. |

**Die Lücke:** Es gibt kein Produkt für den Moment zwischen "ich weiß, was ich diese Woche
trainieren muss" und "ich mache es". Genau dort entsteht die Einsamkeit, und sie ist in jedem
der drei Formate dieselbe.

## Der eigentliche Blocker: zweidimensionale Peer-Knappheit

Das ist die Kernhypothese, und sie ist in v0.5 deutlich schärfer gefasst als vorher.

> **[Hypothese H1]** Ambitionierte Ausdauersportler trainieren nicht deshalb allein, weil es
> keine anderen gäbe. Sie trainieren allein, weil sie kaum jemanden kennen, der **gleichzeitig
> zwei Bedingungen erfüllt**: ähnlich leistungsfähig, und an diesem Tag mit derselben Art von
> Einheit im Plan.
>
> *Prüfmethode:* Nicht "würdest du gerne in der Gruppe trainieren" (Antwort immer ja), sondern:
> "Wie viele Leute kennst du, mit denen du am Dienstag deine Intervalle machen könntest, ohne
> dass einer von euch die Einheit anpassen muss?" Die erwartete Antwort ist null, eins oder zwei.

### Warum das zwei Dimensionen sind und nicht eine

Die beiden Dimensionen werden ständig verwechselt, auch im ersten Entwurf dieses Dokuments:

| Dimension | Gehört zu | Beispiel |
|---|---|---|
| **Leistungsniveau** | zum Menschen | fährt im Flachen 30 km/h oder 35 km/h |
| **Intensität der Einheit** | zum Trainingsplan des Tages | GA1, Schwelle, Intervall, Recovery |

Zwei gleich schnelle Athleten können am selben Tag nicht miteinander trainieren, wenn einer in
der Aufbauwoche und der andere in der Entlastungswoche steht. Zwei Athleten mit derselben
Einheit im Plan können es nicht, wenn zwischen ihnen fünf km/h liegen. Beide Bedingungen müssen
gleichzeitig erfüllt sein, und genau deshalb ist die Menge der tatsächlichen Trainingspartner so
klein.

Rechne es an einem Bekanntenkreis von zehn Triathleten durch: Vielleicht vier sind ungefähr
gleich schnell. Von diesen vier hat an einem gegebenen Dienstag vielleicht einer dieselbe
Einheit im Plan. Ein Bekanntenkreis von zehn liefert also im Schnitt einen einzigen möglichen
Trainingspartner pro Einheit, und der kann an diesem Abend auch noch anders können.

**Das ist der Grund, warum WhatsApp-Gruppen das Problem nicht lösen.** Sie koordinieren Zeit.
Das Problem ist aber nicht die Zeit, sondern die Deckung von Niveau und Planphase. Eine Gruppe
mit 200 Leuten löst es, eine mit 10 nicht, und zwar unabhängig vom Werkzeug.

### Was daraus für das Produkt folgt

1. **Jede Einheit trägt ihre Intensität sichtbar**, in der Sprache, die diese Zielgruppe ohnehin
   spricht: GA1, Schwelle, Intervall, Long, Koppel, Recovery. Nicht als Marketingbegriff,
   sondern damit jemand in zwei Sekunden erkennt, ob es zu seinem Plan an diesem Tag passt.
2. **Jede Einheit trägt konkrete Niveaugruppen**, vom Gastgeber gesetzt, in der Einheit der
   Disziplin.
3. **Dichte ist kein Luxus, sondern die Lösung.** Der Wert des Produkts steigt nicht linear mit
   der Mitgliederzahl, sondern erst ab einer Schwelle sprunghaft, weil erst dann in jeder
   Zelle aus Niveau mal Intensität jemand steht.

### Und ein Korrektiv: harte Einheiten sind die besten Gruppeneinheiten

Die frühere Bezeichnung der Tempogruppen beschrieb sie danach, ob man reden kann. Das war ein
Fehler, weil es implizit sagt, die härteste Einheit sei die unsozialste. Das Gegenteil stimmt:

- Auf dem Rad ist der Windschatten bei hoher Intensität am wertvollsten, die Führungsarbeit wird
  geteilt
- Auf der Bahn hält eine Gruppe das Tempo präziser als jeder Einzelne, und das Zählen der Serien
  fällt leichter
- Im Wasser ist das Anschwimmen in der Bahn genau die Situation, in der man sich gegenseitig zieht
- Im Kraftraum und bei Hyrox macht die Gruppe die Wiederholungen, die man allein auslässt

**Gemeinsam bedeutet nicht locker.** Es bedeutet, dass man die Einheit besser trifft, als man sie
allein getroffen hätte. Das ist das stärkere Verkaufsargument und es richtet sich an genau die
Leute, die ernsthaft trainieren.

## Zweite tragende Hypothese

> **[Hypothese H2]** Wiederkehrende, verlässliche Rituale erzeugen Zugehörigkeit.
> Ad-hoc-Matching erzeugt nur Transaktionen. Ein Produkt, das nur ad hoc kann, bleibt leer.
>
> *Prüfmethode:* Drei feste wöchentliche Anker über acht Wochen und messen, ob das Verhältnis
> von Zusage zu Erscheinen über 50 Prozent liegt.

## Dritte Hypothese, neu in v0.3

> **[Hypothese H3]** Die Zugehörigkeit hält über den Formatwechsel hinweg. Wer im Winter zur
> Krafteinheit kommt, kommt im Sommer zur Ausfahrt, auch wenn er kein Triathlet ist.
>
> *Prüfmethode:* Anteil der Mitglieder, die über einen Saisonwechsel hinweg aktiv bleiben und
> dabei die Disziplin wechseln. Unter 30 Prozent ist die Gruppe in Wahrheit drei getrennte
> Gruppen, die zufällig denselben Kalender teilen.

H3 ist die Kehrseite der Verbreiterung und muss aktiv gemessen werden. Wenn sie scheitert, ist
die breite Definition ein Rechenfehler und nicht eine Chance.

## Personas

Segmentiert nach Lebenssituation, nicht nach Leistungsniveau oder Sportart. Sportart ist eine
Eigenschaft der Einheit, nicht des Menschen.

### P1 Der ambitionierte Berufstätige (Kernzielgruppe)

- 30 bis 45, angestellt oder selbstständig, oft mit Reisetätigkeit
- 8 bis 15 Stunden Training pro Woche, ein bis drei Renndaten im Jahr, oft über Formate hinweg
  (Hyrox im Winter, Trail im Frühjahr, Langdistanz im Sommer)
- Knappster Faktor ist Zeit, nicht Motivation und nicht Geld
- Trainiert nach Plan, meist mit Coach oder gekauftem Plan
- **Job to be done:** "Ich will die Stunden, die ich ohnehin trainiere, nicht auch noch allein
  verbringen. Aber ich kann mich nicht auf Dienstag 18:30 festlegen."
- **Was ihn hält:** Verlässlichkeit und Tempopassung. Zwei schlechte Erfahrungen und er ist weg.

### P2 Die Einsteigerin

- 25 bis 38, kommt aus dem Laufen, dem Fitnessstudio oder dem Schwimmen, erstes großes Renndatum
- Das größte Hindernis ist nicht Fitness, sondern Unsicherheit: Wechselzone, Neopren, Trailschuhe,
  Sled Push, Bahnetikette
- **Job to be done:** "Ich will jemanden, der es schon gemacht hat, und ich will nicht diejenige
  sein, auf die alle warten."
- **Wert:** höchste Bindung und höchste Weiterempfehlungsrate bei gutem ersten Kontakt, höchstes
  Abbruchrisiko bei schlechtem Matching.
- **Achtung:** Beide Gründer sind P1. Diese Persona wird ohne bewusste Gegensteuerung übersehen
  (siehe Risiko R11 in 09).

### P3 Der Vereinsmüde

- 35 bis 50, war im Verein oder hat sich bewusst dagegen entschieden
- Will Training in Gesellschaft ohne Verpflichtung, Beitrag und Vereinspolitik
- Oft erfahren, oft bereit anzuleiten
- **Job to be done:** "Ich will die guten Teile eines Vereins ohne die Struktur."
- **Wert:** wird zum Gastgeber. Diese Gruppe erzeugt Angebot, nicht nur Nachfrage. Ohne P3
  skaliert nichts und das Projekt bleibt an den beiden Gründern hängen.

### Angebotsseite

| Rolle | Motiv | Was sie von 3com brauchen |
|---|---|---|
| Coaches | Kundenakquise, Auslastung von Gruppeneinheiten | Zugang zu qualifizierter Zielgruppe ohne Werbebudget |
| Studios, Gyms, Bäder, Bahnen | Auslastung in Randzeiten | Planbare Gruppenbuchungen über eine ganze Saison |
| Marken (Nutrition, Gear, Bike, Schuh) | Produkttest, Sampling, Glaubwürdigkeit | Zugang zu einer echten, aktiven Zielgruppe statt Influencer-Reichweite |
| Lokale Shops | Kundenbindung, Frequenz | Gruppenausfahrten und Läufe mit Startpunkt beim Shop |

## Nicht-Zielgruppen

Explizit ausgeschlossen, damit das Produkt scharf bleibt:

- Profis und Elite-Athleten mit fixem Trainingsumfeld
- Gelegenheitssportler ohne Renndatum und unter fünf Stunden pro Woche. Das ist der
  entscheidende Ausschluss: er hält das Niveau der Gruppe und die Sprache intakt.
- Reines Fitnessstudio-Publikum ohne Wettkampfziel
- Jugend- und Nachwuchsbereich (Vereinsdomäne, Aufsichtspflicht, andere Regulatorik)
