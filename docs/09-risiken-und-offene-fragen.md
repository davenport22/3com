# 09 Risiken und offene Fragen

> **Konzeptstand bis Mitte Oktober 2026, wird nicht mehr nachgezogen (D-039).** Was aktuell gilt, steht im README und im Entscheidungslog. Der Arbeitstitel 3com heißt heute Windschatten (D-031).

## Top-Risiken, nach Eintrittswahrscheinlichkeit mal Schaden

### R1 Cold Start scheitert (deutlich entschärft)

Ursprünglich das Hauptrisiko: ein leeres Board, das sich selbst füllen muss. Durch die zentral
organisierten Events und zwei Gründer, deren eigenes Training das Angebot ist, ist dieses Risiko
weitgehend neutralisiert. Das Angebot ist von Tag eins garantiert.

**Verbleibende Restform:** Nicht "kein Angebot", sondern "kein fremdes Angebot". Wenn nach
Monaten immer noch ausschließlich ihr beide Einheiten führt, ist es ein Hobby mit Datenbank und
kein Projekt, das ohne euch existiert.

**Gegenmaßnahme:** Der MVP ist auf den Gastgeber optimiert, nicht auf den Teilnehmer (siehe 05).
Meilenstein M5 in der Roadmap macht die Zahl verbindlich.

### R2 Der Markt ist zu klein (hoch / hoch)

Wien allein trägt kein Geschäft (siehe 04). Wenn die zweite Stadt nicht ohne dich funktioniert,
bleibt es ein Verein mit App.

**Gegenmaßnahme:** Multi-City im Datenmodell von Tag eins. Playbook dokumentieren, während Wien
aufgebaut wird, nicht danach. Gleichzeitig die Option offenhalten, nach Disziplinen zu
erweitern (Radsport und Laufen sind jeweils deutlich größer als Triathlon).

**Ehrliche Alternative:** Wenn Wien funktioniert und die zweite Stadt nicht, ist das kein
Scheitern. Es ist die Antwort auf die Ambitionsfrage. Dann Verein oder kleines,
kostendeckendes Geschäft.

### R3 Kein Umsatz, aber laufende Kosten und Zeitaufwand (hoch / mittel)

Die gewählte Erlöslogik zahlt frühestens in Monat 12. Das Projekt stirbt an Erschöpfung, nicht
an Geld.

**Gegenmaßnahme:** Durchreichmodell für Curated Sessions ab Monat 1, damit früh ein
Zahlungsvorgang existiert. Ein kleiner lokaler Partner (Radshop) als erster Deal, der schnell
und klein ist. Klare persönliche Zeitgrenze definieren und einhalten.

### R4 Haftung bei Unfällen (mittel / hoch)

Jemand stürzt bei einer Ausfahrt oder ertrinkt beinahe beim Freiwasserschwimmen. Wer ist
verantwortlich?

**Gegenmaßnahme:** Rechtsberatung vor dem öffentlichen Launch, nicht danach. Grundsatz: 3com ist
Vermittler, nicht Veranstalter. Bei Peer Sessions ist der Gastgeber eine Privatperson, die eine
gemeinsame Trainingseinheit anbietet, keine Dienstleistung. Bei Curated Sessions mit bezahltem
Coach verschiebt sich die Lage deutlich, dort braucht es Vertrag und Versicherung auf Seiten
des Coachs. Freiwasserschwimmen ist die heikelste Kategorie und braucht eine eigene Regelung
(Begleitboje, Zweierregel, definierte Strecken).

**Offene Frage:** Reicht ein Haftungsausschluss in den Nutzungsbedingungen nach
österreichischem Recht, oder braucht es eine Vereinsstruktur als Haftungsschild? Das ist ein
Argument für den Verein, das bisher nicht gewürdigt wurde.

### R5 Die Plattform kippt in Richtung Dating (mittel / hoch)

Eine gemischte Sportcommunity mit Profilen und Direktnachrichten ist strukturell anfällig.
Wenn Frauen sich unwohl fühlen, verliert man die Hälfte des Marktes und den Ruf.

**Gegenmaßnahme:** Keine 1:1-Direktnachrichten in v1, nur Gruppenchat pro Session. Explizite
Community-Regeln bei der Anmeldung. Melde- und Blockfunktion ab Tag eins. Aktive Präsenz von
Frauen in den ersten 30 Mitgliedern, das prägt die Kultur dauerhaft. Frauen-geführte Sessions
aktiv fördern.

### R6 Vereine sehen 3com als Angriff (niedrig / mittel)

Die Wiener Triathlonszene ist klein und vernetzt. Ablehnung durch etablierte Vereine kostet
Zugang zu genau den erfahrenen Leuten, die als Gastgeber gebraucht werden.

**Gegenmaßnahme:** Von Anfang an als Ergänzung positionieren, nicht als Alternative. Vereine
dürfen ihre offenen Einheiten auf dem Board posten. Frühe Gespräche mit zwei bis drei
Vereinsobleuten, bevor öffentlich gelauncht wird.

### R7 Strava baut es selbst (hochgestuft in v0.8: hoch / hoch)

**Die frühere Einschätzung "Strava baut es nicht aus" ist überholt.** Strava Group Events haben
bereits bis zu vier Tempogruppen pro Event. Dazu kam die Runna-Übernahme 2025, The Breakaway
2025 und im Juli 2026 ein eigener Events-Tab. Run-Club-Mitgliedschaften auf Strava sind 2025 um
59 Prozent gewachsen. Es fehlen nur noch wiederkehrende Club-Events, und das ist ein plausibler
nächster Schritt.

**Gegenmaßnahme:** Es gibt keine produktseitige. Der einzige Schutz ist lokale Dichte und reale
Beziehungen, die nicht migrierbar sind. Praktische Konsequenz: nicht versuchen, Strava auf der
Feature-Ebene zu schlagen, sondern die Community so bauen, dass sie auch dann bestehen bliebe,
wenn Strava morgen dieselbe Funktion ausliefert.

### R16 Dichteversagen, empirisch belegt (neu, hoch / hoch)

Die Wettbewerbsrecherche zeigt ein durchgehendes Muster: BikeCrew 3.000 Nutzer in ganz Europa,
CorrerJuntos 1.100 nach Jahren, RoxConnect 16 Bewertungen, SportJoe 30 nach sieben Jahren. Die
Produkte funktionieren technisch und haben trotzdem nie genug Menschen am selben Ort zur selben
Zeit gehabt.

Besonders unangenehm ist der Hyrox-Cluster: sechs Anbieter, rund 1,5 Millionen Starter in der
Saison 2025/26, und ein zwingender Bedarf, weil man ohne Doubles-Partner nicht starten kann.
Trotzdem hat keiner Traktion. Der Bedarf bei 3com ist schwächer, weil man allein trainieren kann.

**Gegenmaßnahme:** Das Dichteproblem wird nicht gelöst, sondern umgangen. Feste Anker, manuelle
Kuratierung, eine bestehende Offline-Gruppe. Das ist der Weg, den die Roadmap ohnehin beschreibt.
Die Konsequenz betrifft die Erwartung, nicht den Plan: **als Community für Wien plausibel, als
Produktthese deutlich schwächer belegt als angenommen.**

### R17 Progressionsproblem und Formatsättigung (neu, mittel / mittel)

Zwei Befunde aus der Community-Recherche. Erstens: Der dokumentierte Haupt-Todesfall aktueller
Run Clubs ist, dass Mitglieder besser werden und das Format nicht mitwächst. Zweitens: Wien hat
bereits mindestens acht sichtbare Run Clubs mit sehr ähnlichem Muster.

**Gegenmaßnahme:** Beides spricht für dieselbe Positionierung. Die Wiener Clubs bedienen fast
durchgehend das soziale Segment. Strukturiertes, gestopptes, periodisiertes Training mit
Vergleichbarkeit fehlt. Ein monatlicher identischer Benchmark und ein gemeinsamer
Wettkampfkalender sind die operative Antwort (siehe 17).

### R8 Saisonalität (mittel / mittel)

Von November bis Februar bricht das Outdoor-Training ein, damit potenziell auch die Aktivität
auf der Plattform.

**Gegenmaßnahme:** Das Winterprogramm ist kein Notprogramm, sondern das strategische Kernstück
(siehe 02). Indoor-Slots, Hallenbad, Krafttraining, Vorträge, Saisonplanung. Der Winter ist die
Phase, in der die Einsamkeit am größten und der Nutzen am höchsten ist.

### R9 Kollision mit eurem eigenen Rennaufbau (herabgestuft: mittel / mittel)

Beide Gründer bereiten sich auf dasselbe Rennen im Sommer 2027 vor. In der spezifischen Phase
von Mai bis Juli liegen eure Trainingsumfänge bei 15 bis 20 Stunden pro Woche. Wer in dieser
Phase noch bauen muss, schafft weder das eine noch das andere.

**Gegenmaßnahme:** Die Periodisierung wird zum Bauplan (siehe 07 und 10). Gebaut wird von
November bis Februar, in eurer Grundlagenphase mit den verlässlichsten Abenden des Jahres. Ab
Mai wird nur noch betrieben.

**Herabstufung in v0.3:** Beide Gründer trainieren ganzjährig und rotieren zwischen Formaten
(Hyrox, Trail und Ultra, Langdistanz). Es gibt keinen einzelnen Saisonhöhepunkt, auf den alles
zuläuft, und damit auch keine Phase, in der das Angebot wegbricht. Die Trainingslast schwankt,
sie fällt aber nicht aus.

**Was bleibt:** Ein klar abgegrenztes Bauzeitfenster ist trotzdem nötig, weil Bauen und
Hochvolumentraining sich schlecht vertragen. Die Begründung hat sich nur verschoben, von
Saisonalität zu schlichter Wochenstundenrechnung.

**Nebeneffekt, der positiv ist:** In eurer umfangreichsten Trainingsphase ist euer Angebot an die
Community am größten, weil ihr ohnehin am längsten unterwegs seid.

### R10 Das Post-Race-Loch (herabgestuft: mittel / mittel)

Nach dem Rennen im Juli 2027 fallen bei euch beiden gleichzeitig Motivation, Trainingsvolumen
und Anwesenheit weg. Eine Community, die zu diesem Zeitpunkt noch an euch hängt, stirbt im
August 2027.

**Gegenmaßnahme:** Fünf fremdgeführte Serien bis Ende Mai 2027 (Meilenstein M5). Herbstprogramm
wird im Mai geplant, nicht im August. Eine Veranstaltung nach dem Rennen, die keine Fitness
braucht.

**Herabstufung in v0.3:** Die ursprüngliche Bewertung unterstellte einen einzelnen
Saisonhöhepunkt mit anschließendem Motivationsloch. Bei ganzjährig trainierenden
Ausdauer-Generalisten mit mehreren Formaten im Jahr existiert dieses Loch so nicht. Nach dem
Ironman im Juli folgt bei euch die Trail- oder Hyrox-Vorbereitung, nicht die Couch.

**Was bleibt:** Fünf fremdgeführte Serien bis Ende Mai 2027 bleiben im Plan, aber als
Skalierungsbedingung statt als Überlebensbedingung. Sie beantworten weiterhin die einzige Frage,
die über das Ambitionsniveau entscheidet: läuft es ohne euch?

**Strukturelle Alternative:** Staffelt eure Rennen, falls das noch offen ist. Dasselbe Rennen
ist gut für die Geschichte und schlecht für die Ausfallsicherheit.

### R11 Gründer-Blindstelle (mittel / mittel)

Beide Gründer sind Persona P1, ambitionierte Berufstätige mit Langdistanzziel. Ein Produkt, das
nur von P1 entworfen wird, wird für P1 gut und für Einsteigerinnen unzugänglich. Genau die
Einsteigergruppe hat aber die höchste Bindung und die höchste Weiterempfehlungsrate.

**Gegenmaßnahme:** Mindestens zehn der ersten dreißig Mitglieder sind Einsteigerinnen oder
Einsteiger. Eine der drei Anker-Einheiten wird ausdrücklich für sie ausgelegt. Und mindestens
eine Frau unter den ersten fünf Gastgebern, sonst prägt sich die Kultur falsch ein und ist
später nicht mehr korrigierbar.

### R12 Rollen und Anteile (herabgestuft: niedrig / mittel)

**Weitgehend gelöst:** Anteile werden zu gleichen Teilen geteilt, die Arbeitsteilung folgt einer
natürlichen Neigung, einer eher BD, Vertrieb und Community, einer eher Bauen und Produkt. Diese
Teilung liegt günstig zum Kalender, weil die Lastspitzen sich ergänzen statt zu überlappen
(siehe 07).

**Was offen bleibt, ist klein und wichtig:** Vesting und der Ausstiegsfall. Gleiche Anteile sind
die richtige Antwort, aber ohne Regelung hält jemand, der nach acht Monaten aussteigt, weiterhin
die Hälfte von etwas, das der andere weiterträgt. Eine halbe Stunde jetzt.

### R15 Der Builder verschwindet im Bauzeitfenster (neu, mittel / mittel)

Von November bis Februar sitzt einer von euch weitgehend am Rechner. Vier Monate ohne Präsenz
bei den Einheiten bedeuten, dass er danach für eine Community baut, die er nicht mehr kennt.
Bei einem Produkt, dessen einziger Wert soziale Dichte ist, ist das ein echtes Risiko und kein
Komfortthema.

**Gegenmaßnahme:** Der Builder führt auch im Bauzeitfenster mindestens eine Anker-Einheit pro
Woche. Anwesenheit ist bei einer Community nicht Beiwerk, sondern das Produkt.

### R13 Identitätsverwässerung durch die Verbreiterung (neu, mittel / hoch)

Die Abgrenzung über Trainingslast statt Sportart vergrößert den Markt um das Zwei- bis
Dreifache. Sie kostet aber genau das, was einen Stamm zusammenhält: die gemeinsame Sprache. Eine
"Ausdauersport-Community" ist eine Kategorie, kein Zugehörigkeitsgefühl, und konkurriert mit
jedem Lauftreff der Stadt.

**Gegenmaßnahme:** Die Verankerung bleibt triathlon-nah, weil Triathlon die höchste
Trainingslast, die stärkste Sprache und die klarste Zugehörigkeit mitbringt. Die Grenze wird
über die Last gezogen (acht Stunden plus, mit Renndatum), nicht über die Sportart. Der
Ausschluss des Gelegenheitssportlers ist dabei wichtiger als die Aufnahme des Trailläufers:
er hält das Niveau und damit die Sprache intakt.

**Messgröße:** Hypothese H3 in 01. Wenn unter 30 Prozent der Mitglieder über einen
Saisonwechsel hinweg die Disziplin wechseln, sind es in Wahrheit drei getrennte Gruppen mit
gemeinsamem Kalender, und die Verbreiterung war ein Rechenfehler.

### R14 Hyrox-Saison liegt im Bauzeitfenster (neu, mittel / mittel)

Das Bauzeitfenster November bis Februar war mit der Grundlagenphase eines Triathleten
begründet. Die Hyrox-Wettkampfsaison liegt aber genau dort. Wer im Januar ein Rennen hat, hat im
Januar keine ruhige Phase.

**Gegenmaßnahme:** Das Bauzeitfenster bleibt, die Begründung ändert sich: nicht "ihr habt Zeit",
sondern "draußen passiert wenig und die Abende sind planbar". Konkret zu klären, bevor die
Roadmap fixiert wird: hat einer von euch ein Hyrox-Rennen zwischen November und Februar. Wenn
ja, baut der andere in dieser Phase den Hauptteil.

## Offene Fragen zur Entscheidung

| # | Frage | Wann zu entscheiden | Wer entscheidet |
|---|---|---|---|
| Q1 | Rechtsform: Einzelunternehmen, Verein oder GmbH? Der Haftungsaspekt (R4) spricht stärker für den Verein als bisher berücksichtigt. | vor öffentlichem Launch | David plus Steuerberater und Anwalt |
| Q2 | ~~Allein oder mit Mitgründerin?~~ **Beantwortet:** zwei Gründer, beide mit eigenem Bedarf. Offen bleibt die schriftliche Klärung von Anteilen und Ausstiegsfall. | vor Phase 1 | beide Gründer |
| Q3 | Wie viel Zeit pro Woche real, über 12 Monate, je Gründer? Mit Rennaufbau ist die Grenze niedriger als sie sich heute anfühlt. | sofort | beide Gründer |
| Q8 | Bleiben beide beim selben Rennen, oder wird gestaffelt? | vor Jahresplanung | beide Gründer |
| Q9 | Liegt bei einem von euch ein Hyrox-Rennen zwischen November und Februar? Das verschiebt die Lastverteilung im Bauzeitfenster. | vor Oktober 2026 | beide Gründer |
| Q4 | ~~Triathlonspezifisch oder ausdauersportbreit?~~ **Beantwortet:** Ausdauer-Generalisten, triathlon-verankert, Abgrenzung über Trainingslast. Offen bleibt die Messung von H3. | laufend | beide Gründer |
| Q5 | Freiwasserschwimmen anbieten oder aus Haftungsgründen ausschließen? | vor Sommersaison | David plus Anwalt |
| Q6 | Wird der Strava-Import gebaut oder bleiben die Tempobänder selbstdeklariert? | Woche 1 der Entwicklung | David |
| Q7 | Finaler Name | Woche 8 | David |

## Was dieses Konzept noch nicht enthält

Bewusst ausgespart, weil verfrüht:

- Finanzmodell mit Monatsgranularität
- Markenidentität, Logo, Design-System
- Rechtstexte (AGB, Datenschutzerklärung, Community-Regeln im Wortlaut)
- Detaillierter Partner-Pitch für Marken
- Interview-Leitfaden für die Nutzervalidierung (nächster sinnvoller Schritt)
