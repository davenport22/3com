# 01 Problem und Nutzer

## Das Problem in drei Sätzen

Triathlontraining für eine Mitteldistanz oder Langdistanz bedeutet 8 bis 15 Stunden pro Woche,
verteilt auf drei Disziplinen, über neun bis zwölf Monate. Der Großteil dieser Stunden wird
allein absolviert, obwohl fast jede dieser Einheiten in Gesellschaft besser wäre: der lange
Radausfahrt-Sonntag, die Bahneinheit, das Schwimmen, die Koppeleinheit. Das Ergebnis ist ein
Sport, in dem Menschen mit identischem Ziel, identischem Tempo und identischem Wohnbezirk
monatelang nebeneinander her trainieren, ohne sich zu kennen.

## Warum das Problem heute nicht gelöst ist

| Bestehende Lösung | Warum sie das Problem nicht löst |
|---|---|
| Triathlonverein | Feste Zeiten, Mitgliedsbeitrag, Lizenzkultur, oft Leistungsorientierung. Passt schlecht zum Berufstätigen, der Dienstag kurzfristig doch kann und Mittwoch doch nicht. |
| Strava Club | Rückblickend. Zeigt, was jemand gemacht hat, nicht was jemand vorhat. Keine Koordinationsfunktion. |
| WhatsApp-Gruppe | Funktioniert bis circa 30 Leute, danach Lärm. Kein Tempo-Matching, keine Historie, keine Auffindbarkeit, kein Onboarding für Neue. |
| Facebook-Gruppen | Demografisch im Rückzug, Reichweite algorithmisch gedeckelt, kein Terminobjekt. |
| Trainingsplan-Apps (TrainingPeaks, MOTTIV, Intervals.icu) | Lösen die Planung, nicht die Gesellschaft. Explizit einzelsportlich gedacht. |
| Lauftreffs / Gruppenausfahrten von Shops | Existieren, aber eindisziplinär, unregelmäßig kommuniziert und ohne Triathlonbezug. |

**Die Lücke:** Es gibt kein Produkt für den Moment zwischen "ich weiß, was ich diese Woche
trainieren muss" und "ich mache es". Genau dort entsteht die Einsamkeit.

## Der eigentliche Blocker: das Tempoproblem

Die Hypothese, die das ganze Konzept trägt:

> **[Hypothese H1]** Der Hauptgrund, warum Age-Grouper nicht mit anderen trainieren, ist nicht
> fehlende Gelegenheit, sondern die Angst vor der Tempo-Fehlpaarung. Zu langsam heißt Blamage,
> zu schnell heißt kaputte Einheit. Beides ist schlimmer als allein fahren.
>
> *Prüfmethode:* 15 qualitative Interviews mit Wiener Age-Groupern. Frage nicht "würdest du
> gerne in der Gruppe trainieren" (Antwort immer ja), sondern "erzähl mir von der letzten
> Gruppeneinheit, die du ausgelassen hast, obwohl du Zeit hattest".

Daraus folgt: Tempo-, Watt- und Zielbandbreite sind kein Nice-to-have-Filter, sondern das
Kernfeature. Ohne glaubwürdiges Matching ist das Board ein schwarzes Brett und kein Produkt.

## Zweite tragende Hypothese

> **[Hypothese H2]** Wiederkehrende, verlässliche Rituale erzeugen Community. Ad-hoc-Matching
> erzeugt nur Transaktionen. Ein Produkt, das nur ad hoc kann, bleibt leer.
>
> *Prüfmethode:* Zwei feste wöchentliche Anker-Einheiten über acht Wochen laufen lassen und
> messen, ob die Wiederkehrrate über 40 Prozent liegt.

## Personas

Segmentiert nach Lebenssituation, nicht nach Leistungsniveau. Leistung ist ein Filter im
Produkt, nicht ein Segment im Markt.

### P1 Der ambitionierte Berufstätige (Kernzielgruppe)

- 32 bis 45, Angestellter oder Selbstständiger, oft mit Reisetätigkeit
- 10 bis 14 Stunden Training pro Woche, Ziel 70.3 oder Ironman
- Knappster Faktor ist Zeit, nicht Motivation und nicht Geld
- Trainiert nach Plan, meist mit Coach oder gekauftem Plan
- **Job to be done:** "Ich will die Stunden, die ich ohnehin trainiere, nicht auch noch allein
  verbringen. Aber ich kann mich nicht auf Dienstag 18:30 festlegen."
- **Was ihn hält:** Verlässlichkeit und Tempopassung. Zwei schlechte Erfahrungen und er ist weg.

### P2 Die Einsteigerin

- 26 bis 38, kommt aus Laufen oder Schwimmen, erstes Olympisches oder erstes 70.3
- Das größte Hindernis ist nicht Fitness, sondern Unsicherheit: Wechselzone, Neopren,
  Windschattenregeln, Bahnetikette
- **Job to be done:** "Ich will jemanden, der es schon gemacht hat, und ich will nicht diejenige
  sein, auf die alle warten."
- **Wert für 3com:** höchste Bindung und höchste Weiterempfehlungsrate, wenn der erste Kontakt
  gut läuft. Gleichzeitig das größte Abbruchrisiko bei schlechtem Matching.

### P3 Der Vereinsmüde

- 35 bis 50, war mal im Verein oder hat sich bewusst dagegen entschieden
- Will Training in Gesellschaft ohne Verpflichtung, Beitrag, Vereinspolitik
- Oft erfahren, oft bereit anzuleiten
- **Job to be done:** "Ich will die guten Teile eines Vereins ohne die Struktur."
- **Wert für 3com:** wird zum Session-Host. Diese Gruppe erzeugt Angebot, nicht nur Nachfrage.
  Ohne P3 skaliert nichts.

### Angebotsseite (keine Personas, aber Stakeholder)

| Rolle | Motiv | Was sie von 3com brauchen |
|---|---|---|
| Coaches | Kundenakquise, Auslastung von Gruppeneinheiten | Zugang zu qualifizierter Zielgruppe ohne Werbebudget |
| Studios, Bäder, Bahnen | Auslastung in Randzeiten | Planbare Gruppenbuchungen |
| Marken (Nutrition, Gear, Bike) | Produkttest, Sampling, Glaubwürdigkeit bei Age-Groupern | Zugang zu einer echten, aktiven Zielgruppe statt Influencer-Reichweite |
| Lokale Radshops | Kundenbindung, Frequenz | Gruppenausfahrten mit Startpunkt beim Shop |

## Nicht-Zielgruppen

Explizit ausgeschlossen, damit das Produkt scharf bleibt:

- Profis und Elite-Age-Grouper mit fixem Trainingsumfeld
- Reine Läuferinnen ohne Triathlonambition (eigener, größerer, aber anders gelagerter Markt)
- Fitnessstudio-Publikum ohne Wettkampfziel
- Jugend- und Nachwuchsbereich (Vereinsdomäne, andere Regulatorik, Aufsichtspflicht)
