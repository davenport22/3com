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

---

## D-019 Zwei getrennte Dimensionen: Intensität und Niveau

**Datum:** 2026-09-11
**Ersetzt:** D-010 in der Benennung, bestätigt es im Grundsatz.
**Entscheidung:** Das Produkt trennt strikt zwei Dimensionen.
**Intensität** gehört zur Einheit und kommt aus dem Trainingsplan. Sie wird in der Sprache der
Zielgruppe benannt (GA1, GA2, Schwelle, Intervall, Long, Koppel, Recovery,
Wettkampfsimulation), dazu eine Zeile Struktur im Klartext, etwa "4x8min Schwelle, 4min Pause".
**Niveau** gehört zum Menschen, ist ein Korridor in der Einheit der Disziplin und ändert sich
über Monate, nicht über Tage.
**Begründung:** Die Benennung Kaffeefahrt, Tempo, Vollgas vermischte beides und suggerierte
zusätzlich, die härteste Einheit sei die unsozialste. Das ist falsch. Auch Vollgas ist gemeinsam
besser, und zwar messbar: Windschatten, geteilte Führungsarbeit, präziseres Tempo auf der Bahn.
**Folge für das Matching:** Niveau wird berechnet und als passende Gruppe angezeigt. Planpassung
wird nur dargestellt, nie berechnet. 3com kennt keinen Trainingsplan und tut nicht so.
**Wiedervorlage:** keine.

---

## D-020 Anker-Einheiten müssen zwei Planphasen bedienen

**Datum:** 2026-09-11
**Entscheidung:** Jede wiederkehrende Anker-Einheit wird so entworfen, dass Aufbau- und
Entlastungswoche nebeneinander laufen können: zwei Längenoptionen auf derselben Route, variable
Wiederholungszahl bei identischer Serienstruktur, variabler Umfang bei identischem Hauptsatz.
**Begründung:** Direkte Folge aus H1. Gleiches Niveau reicht nicht, wenn die Planphase nicht
passt. Eine Einheit, die nur eine Planphase bedient, verliert jede Woche die Hälfte der Leute.
**Kommunikationsregel:** Jede Einladung nennt Intensität und beide Längenoptionen.
**Wiedervorlage:** keine.

---

## D-021 Distanzen werden vorgegeben, genau zwei Optionen

**Datum:** 2026-09-11
**Entscheidung:** Jede Einheit nennt eine konkrete Distanz oder Dauer, und genau zwei Optionen.
Gemeinsamer Start, Trennung an einem benannten Abzweig. Nie drei Optionen, nie "such dir was aus".
Die Zahlen bleiben über Monate gleich.
**Begründung:** Eine Einladung ohne Zahl ist keine Einladung, sondern eine Frage, und sie
verlagert die Arbeit auf den Empfänger. Ohne Zahl kommen weniger Leute, nicht mehr. Bei zwei
Optionen entscheidet man, bei drei vergleicht man und sagt ab. Zusätzlich entfernt eine
festgelegte Distanz eine Dimension aus dem Raster aus Niveau, Intensität, Zeit, Ort und
Disziplin und erhöht damit die Trefferwahrscheinlichkeit multiplikativ.
**Nebenwirkung, die erwünscht ist:** "Der Samstag ist 110" ist ein Satz, den ein Mitglied über
die Gruppe sagt. Feste Größen erzeugen Zugehörigkeit, Beliebigkeit erzeugt keine.
**Gegenprobe:** Zwei Samstage mit angesagter Distanz, zwei ohne, Zusagen und Erschienene zählen.
Kostet nichts und liefert die Stärke des Effekts.
**Wiedervorlage:** nach vier Ausfahrten.

---

## D-022 Maximal fünf Serien im ersten Jahr

**Datum:** 2026-09-11
**Entscheidung:** Höchstens fünf wiederkehrende Serien im ersten Jahr. Eine neue entsteht nur,
wenn eine bestehende dauerhaft über fünfzehn Teilnehmende kommt und sich teilen muss.
Zusatzwünsche wandern in saisonale Special Sessions, nicht in neue wöchentliche Serien.
**Begründung:** Die Verbreiterung auf mehrere Disziplinen hat die Zahl möglicher Zellen
vervielfacht. Bei geringer Dichte verdünnt jede zusätzliche Serie alle anderen. 100 Mitglieder
auf fünf Serien sind zehn Erscheinende pro Termin, auf fünfzehn Serien drei bis vier.
**Wachstumslogik:** Zellteilung statt Neugründung.
**Wiedervorlage:** bei 250 aktiven Mitgliedern in einer Stadt.

---

## D-023 Gestaltungsprinzip: Trainingsprotokoll statt Kampagne

**Datum:** 2026-09-11
**Entscheidung:** Das gesamte Erscheinungsbild folgt der Logik eines Trainingsprotokolls. Jede
Aussage ist eine Feststellung mit Uhrzeit, Ort, Intensität und beiden Distanzen. Keine
Adjektive, keine Superlative, keine Motivationssprache. Eine Akzentfarbe (Signal-Amber),
dunkel als Standard, eine Schriftfamilie in drei Rollen.
**Begründung:** Die Zielgruppe ist gegen Sportmarketing immunisiert. Glaubwürdigkeit entsteht
über Zahlen und über Termine, die stattgefunden haben, nicht über Bilder und Versprechen.
**Bildzeichen:** eine Linie, die an einem markierten Punkt zwei Wege nimmt. Das ist zugleich die
Regel aus D-021 (gemeinsamer Start, benannter Abzweig) und das Windschatten-Bild. Kein
Icon-Logo, nur Wortmarke plus Gabelung, damit ein Namenswechsel das System nicht zerstört.
**Sprachregel:** Fachsprache ist erwünscht und wirkt als Türsteher. Das Wort "Community" wird in
der Selbstbeschreibung nicht verwendet.
**Wiedervorlage:** nach der Namensentscheidung.

---

## D-024 Erwartungskorrektur nach dem Wettbewerbs-Realitätscheck

**Datum:** 2026-09-11
**Entscheidung:** Das Gewicht verschiebt sich von der Produktthese zur Community. Die App bleibt
im Plan, aber als Betriebssystem für wenige Serien, nicht als Startup. Wenn im Winter die Wahl
zwischen Feature-Arbeit und Gastgeberakquise steht, gewinnt ab jetzt immer die Akquise.
**Begründung:** Die Annahme "es gibt keinen direkten Wettbewerber" war falsch. Strava Group
Events haben bereits Tempogruppen, OnlyTri filtert nach Pace, Volumen und Level, Pace
(paceclubapp) hat Serien plus Tempogruppen plus RSVP. Der einzige verifizierte weiße Fleck ist
das Intensitätsvokabular, und ein Datenfeld ist kein Burggraben. Entscheidender ist das Muster
über alle Anbieter: sie scheitern an Dichte, nicht an Funktionen.
**Der härteste Einzelbefund:** Sechs Hyrox-Partner-Apps, rund 1,5 Mio Starter, ein zwingender
Partnerbedarf, und trotzdem keine Traktion. Wenn ein Muss-Bedarf kein Produkt trägt, trägt ein
Kann-Bedarf vermutlich auch keines.
**Folge für das Ambitionsniveau:** Der Pfad "skalierbare Plattform" aus Dokument 00 wird
unwahrscheinlich. Realistisch bleiben Verein oder kleines, kostendeckendes Geschäft in einer
Stadt.
**Wiedervorlage:** nach Meilenstein M5.

---

## D-025 Erst ein Anker, zwölf Wochen ohne Ausfall

**Datum:** 2026-09-11
**Entscheidung:** Verschärfung von D-022. Im ersten Quartal läuft genau **eine** Serie, nicht
drei. Weitere Anker kommen erst, wenn die erste zwölf Wochen ohne Ausfall gelaufen ist.
**Begründung:** parkrun, November Project, Midnight Runners und HYROX sind alle auf genau einem
invarianten Format gewachsen. Gründer-Guides nennen wechselnde Treffpunkte und zu viele parallele
Termine als Abbruchgrund Nummer eins.
**Wiedervorlage:** nach zwölf Wochen.

---

## D-026 Der Verbal: öffentliches Commitment statt Anmeldung

**Datum:** 2026-09-11
**Entscheidung:** Am Ende jeder Einheit sagt jeder laut, ob er beim nächsten Termin dabei ist.
Übernommen von November Project.
**Begründung:** Es ist das wirksamste bekannte Mittel gegen No-Shows und kostet nichts. Die
Kennzahl Zusage zu Erscheinen entscheidet laut Roadmap über das Go/No-Go für den Bau, also lohnt
sich jedes Mittel, das sie hebt. Eine soziale Verpflichtung gegenüber Menschen, die man in drei
Tagen wiedersieht, wirkt stärker als jede Push-Nachricht.
**Wiedervorlage:** keine.

---

## D-027 Monatlicher identischer Benchmark

**Datum:** 2026-09-11
**Entscheidung:** Ein monatlicher, immer gleicher, gestoppter Benchmark. Kandidaten: Kahlenberg
als Bergzeitfahren, 5 km Prater Hauptallee, oder eine Hyrox-Stationskombination.
**Begründung:** November Project hat den PR Day, Rapha die Festive 500, HYROX das weltweit
identische Rennformat. Für eine Zielgruppe mit acht und mehr Wochenstunden ist messbarer
Fortschritt der eigentliche Bindungstreiber. Beleg dafür aus der Gegenrichtung: parkrun entfernte
2024 Streckenrekorde und erntete eine Petition.
**Nebennutzen:** liefert gleichzeitig Trainingsreiz, Fortschrittsnachweis, Inhalt und
Gesprächsstoff.
**Wiedervorlage:** keine.

---

## D-028 Erkennungszeichen wird verdient, nicht verkauft

**Datum:** 2026-09-11
**Entscheidung:** Konkretisierung des Erkennungszeichens aus D-023. Ein Patch oder Sprüh-Tag pro
zehn absolvierten Einheiten, angebracht beim Termin selbst, auf das eigene Trikot. Kein Shop.
**Begründung:** November Project besprüht die Shirts beim Workout per Schablone, immer am ersten
Mittwoch im Monat. Jedes Stück ist dadurch ein Unikat und belegt Anwesenheit. Black Roses vergibt
das Singlet nur auf Einladung. Ein käufliches Zeichen ist fälschbar und signalisiert nichts.
**Nebennutzen:** null Lagerrisiko, und es löst das Wiedererkennungsproblem im Wettkampf.
**Wiedervorlage:** keine.

---

## D-029 Aufwandsschätzung für den App-Bau korrigiert

**Datum:** 2026-09-25
**Entscheidung:** Das Bauzeitfenster November bis Februar entfällt als Planungsgröße. Der
Umfang aus `05-product-mvp-spec.md` ist mit KI-gestützter Entwicklung eher ein Wochenende plus
zwei bis drei Abende Nachschärfen.
**Begründung:** Die alte Schätzung unterstellte Handarbeit. Damit war der Bau ein Engpass, der
ein eigenes Quartal brauchte, und das hat den ganzen Plan verzerrt.
**Folge:** Der Bau braucht kein Zeitfenster mehr. Er passiert, wenn die Community ihn braucht.
Das ändert nichts an der Reihenfolge: erst Dichte, dann Werkzeug. Es senkt nur die Kosten,
falsch zu liegen.
**Wiedervorlage:** keine.

---

## D-030 Sichtbarer Prototyp für die Ansprache

**Datum:** 2026-09-25
**Entscheidung:** Website und klickbarer App-Prototyp werden in der Ansprache der ersten Leute
eingesetzt, um das Vorhaben zu zeigen. Beides ist als Entwurf gekennzeichnet.
**Begründung:** Eine Einladung zu einer Ausfahrt bleibt eine Einladung zu einer Ausfahrt. Wer
aber nachfragt, wohin das gehen soll, bekommt eine Antwort, die er sich ansehen kann. Das hebt
die Zusagequote und zieht Menschen an, die Lust auf den Aufbau haben, nicht nur auf die Runde.
**Regel:** Der Prototyp wird nie als bestehendes Produkt dargestellt. Beide Seiten tragen
sichtbar den Hinweis Entwurf.
**Wiedervorlage:** keine.

---

## D-031 Der Name ist Windschatten

**Datum:** 2026-10-13
**Entscheidung:** Das Projekt heißt Windschatten. 3com entfällt, die Shortlist aus `08-naming.md`
ist abgeschlossen. Kadenz, Rudel und Grundlage werden nicht weiterverfolgt.
**Begründung:** Windschatten ist das einzige Wort auf der Liste, das die Sache selbst beschreibt
und nicht nur klingt: vorne fährt jemand, hinten spart man ein Drittel, man wechselt sich ab. Das
ist gleichzeitig die Erklärung, warum Gruppentraining besser ist als Alleintraining, und die
Umgangsform, die diese Gruppe haben soll. Kadenz ist Radsprache und schließt Laufen und Schwimmen
aus. Rudel ist eine Behauptung über Härte. Grundlage ist zu nah an GA1 und damit zu eng.
**Eingestandener Nachteil:** dreizehn Zeichen, deutsch, international nicht tragfähig. Das ist in
Wien kein Problem und im Fall einer zweiten Stadt im DACH-Raum auch nicht. Falls das Projekt
jemals darüber hinausgeht, ist ein Namenswechsel das kleinste der dann anstehenden Probleme.
**Folge:** Domain und Instagram-Handle werden auf Windschatten geprüft und gesichert. Die
Domainprüfung konnte aus der Arbeitsumgebung heraus nicht durchgeführt werden (RDAP nicht
erreichbar), sie steht noch aus.
**Wiedervorlage:** nur bei Expansion außerhalb des deutschsprachigen Raums.

---

## D-032 Die App ist gebaut und läuft

**Datum:** 2026-10-13
**Entscheidung:** Statt eines weiteren Prototyps gibt es ein funktionierendes Terminwerkzeug mit
geteilter Datenbank: Einheiten anlegen, Niveaugruppe wählen, zusagen, sehen wer kommt. Quelltext
in `app/windschatten.html`.
**Begründung:** D-029 hat festgehalten, dass der Bau kein Engpass mehr ist. Ein Klickprototyp zu
zeigen, obwohl das echte Ding in derselben Zeit entsteht, wäre nach dieser Erkenntnis nur noch
Gewohnheit. Ein Werkzeug, das wirklich läuft, kostet nichts extra und beantwortet eine Frage, die
kein Prototyp beantwortet: ob Leute tatsächlich zusagen.
**Grenze:** Zusagen kann nur, wer Schreibrecht auf dem Artefakt hat. Das passt für die ersten
zehn bis fünfzehn Personen und ist ab dort neu zu bewerten. Für alle anderen bleibt WhatsApp.
**Regel aus D-030 bleibt:** Die App wird nicht als fertiges Produkt dargestellt. Sie ist das
Terminbrett der Gruppe, mehr behauptet sie nicht.
**Wiedervorlage:** sobald mehr als fünfzehn Personen zusagen wollen.

---

## D-033 Neustart am 17.10.2026, der Samstag ist der einzige Anker

**Datum:** 2026-10-13
**Entscheidung:** Die erste Ausfahrt findet am 17.10.2026 statt. Bis auf Weiteres gibt es genau
einen wiederkehrenden Termin: Samstag, 08:00, Reichsbrücke. Dienstag und Donnerstag kommen erst
dazu, wenn der Samstag mehrere Wochen ohne Lücke stattgefunden hat.
**Begründung:** Der ursprünglich geplante Termin am 19.09. hat nicht stattgefunden, weil keine
Zeit war. Genau das ist das Ausfallrisiko aus `09-risiken-und-offene-fragen.md`, und es ist
eingetreten, bevor ein einziger Teilnehmer da war. Drei Anker gleichzeitig zu starten, erhöht
dieses Risiko um das Dreifache. Ein Termin, der stattfindet, schlägt drei, die auf dem Papier
stehen.
**Abbruchkriterium unverändert:** Verhältnis Zusage zu Erscheinen über sechs Wochen unter
50 Prozent, dann wird nichts weiter gebaut.
**Wiedervorlage:** nach der dritten durchgeführten Ausfahrt.

---

## D-034 Keine Monetarisierung. Nur Kostendeckung.

**Datum:** 2026-10-14
**Entscheidung:** Windschatten verfolgt kein Erlösziel. Es gibt keine Take Rate, keine Beiträge,
kein Abo, keinen Markenumsatz. Was Geld kostet (Hallenzeit, Bahn, Studio, Coach), wird durch die
geteilt, die daran teilnehmen. Marken sind nur als Übernahme konkreter Kosten oder Sachleistung
denkbar, nie als Einnahme.
**Begründung:** Vorgabe des Gründers, bestätigt am 14.10.2026. Das war von Anfang an die
Prämisse ("kein Unternehmen für maximalen Gewinn"), stand aber bis jetzt als Verschiebung im
Plan statt als Festlegung. Die Verschiebung hat Arbeit erzeugt, die nie gebraucht wurde.
**Folgen:**
- D-001 (Ambitionsniveau bleibt offen) ist damit beantwortet und geschlossen. Das hier ist eine
  Gruppe mit einem Werkzeug, kein Unternehmen. Die Frage nach Verein, Bootstrapped Business oder
  Plattform stellt sich nicht mehr.
- `03-geschaeftsmodell.md` ist ab jetzt ein Kostenmodell. Unit Economics, Erlöslogik und
  Take-Rate-Rechnungen sind gegenstandslos.
- Meilenstein M7 ("Erster Euro") entfällt ersatzlos.
- Die Belastungsgrenze ist nicht mehr Geld, sondern Aufmerksamkeit. Ohne Erlös gibt es keine
  Möglichkeit, Arbeit einzukaufen. Die einzige Währung ist die Bereitschaft anderer, eine Einheit
  zu führen. **M5 (fünf fremdgeführte Serien) ist damit nicht mehr ein Meilenstein unter acht,
  sondern die einzige Überlebensbedingung des Vorhabens.**
- Was wegfällt, fällt ersatzlos weg: kein Pitch, keine Investorenlogik, keine Bewertungsfrage,
  keine zweite Stadt aus Wachstumsgründen. Eine zweite Stadt entsteht höchstens, weil jemand dort
  dasselbe machen will.
**Wiedervorlage:** nur wenn laufende Kosten entstehen, die sich nicht umlegen lassen.

---

## D-035 Zwei Ebenen: fixer Anker am Wochenende, bewegliche Einheiten unter der Woche

**Datum:** 2026-10-14
**Entscheidung:** Das Terminmodell bekommt zwei Ebenen mit unterschiedlichen Regeln.

| | Fixer Anker | Bewegliche Einheit |
|---|---|---|
| Wann | Samstag, 08:00, immer dieselbe Stelle | unter der Woche, Termin wechselt |
| Was | lange Ausfahrt, langer Lauf | Intervalle, Gym, Bahn, Koppel |
| Wer legt an | die Gastgeber | jede und jeder |
| Gilt | findet statt, egal wer zusagt | findet statt, wenn wer mitmag |
| Vorlauf | wochenlang bekannt | ein bis drei Tage |

**Begründung:** Die bisherige Annahme war, dass alle drei Anker ganzjährig an derselben Stelle im
Kalender stehen müssen, weil Wiederholung Verlässlichkeit erzeugt. Für das Wochenende stimmt das
und bleibt. Unter der Woche ist es falsch, und zwar aus demselben Grund, aus dem das ganze Projekt
existiert.

Ein fester Dienstagstermin verlangt, dass zehn Trainingspläne sich einem Slot anpassen. Das ist
genau die zweidimensionale Peer-Knappheit aus `01-problem-und-nutzer.md`, nur mit einer
zusätzlichen Bedingung: jetzt muss auch noch der Wochentag passen. Ein bewegliches Angebot dreht
das um. Wer ohnehin Schwelle im Plan hat, sagt es an, und wer etwas Kompatibles im Plan hat,
kommt mit. Die Zuordnung passiert über das Angebot, nicht über den Kalender.

**Die allgemeine Regel dahinter:** Feste Slots sind ein dichteabhängiges Instrument. Unterhalb
einer gewissen Gruppengröße schlägt Zuordnung die Terminplanung, oberhalb ist es umgekehrt, weil
sich dann jeder Slot füllt und der Ritualwert überwiegt. parkrun und November Project arbeiten
oberhalb dieser Schwelle. Windschatten mit acht Leuten arbeitet darunter.

**Warum das Wochenende die Ausnahme ist:** Die lange Einheit ist durch Arbeitszeiten ohnehin auf
das Wochenende synchronisiert. Da ist der Slot keine Zumutung, sondern eine Feststellung.

**Verhältnis zu Council-Runde 2:** Dort wurde das Ad-hoc-Board gestrichen, weil ein leeres Board
sichtbares Scheitern ist. Das Argument gilt weiter und ist der Grund, warum diese Ebene begrenzt
und rücknehmbar ist. Gestrichen wurde damals ein Board, das die Serien *ersetzt*. Hier bleibt der
Anker unangetastet.

**Risiko und Gegenmaßnahme:** Eine leere Angebotsliste wirkt tot. Deshalb bleibt WhatsApp der
primäre Kanal für bewegliche Einheiten, die App bildet sie nur ab, und der Leerzustand ist als
Aufforderung formuliert, nicht als Lücke.
**Abbruchkriterium für diese Ebene:** Wenn nach vier Wochen niemand außer den Gastgebern eine
Einheit angeboten hat, fliegt sie wieder raus.
**Umgesetzt:** `app/windschatten.html`, getrennte Ablage `sessions` (Anker) und `offers`
(beweglich, jede Person schreibt nur in die eigene).
**Wiedervorlage:** bei mehr als 25 aktiven Personen, dann ist die Dichteschwelle möglicherweise
überschritten und feste Wochentermine schlagen wieder das Anbieten.

---

## D-036 Kein natives iOS. Der Flow wird im Web gebaut.

**Datum:** 2026-10-14
**Auslöser:** Gewünschter Ablauf: eine Einheit anlegen ("ich mach am Mittwoch die 1h
Intervalle"), den Link zusätzlich in die WhatsApp-Gruppe stellen, andere klicken drauf, sagen zu
und übernehmen den Termin in ihren Kalender.
**Entscheidung:** Der Ablauf wird gebaut, die native App nicht. Nichts an diesem Ablauf verlangt
eine native App, mit einer Ausnahme.

| Schritt | Geht heute | Bemerkung |
|---|---|---|
| Einheit anlegen | ja | jede Person, nicht nur die Gastgeber (D-035) |
| Eigener Link pro Einheit | ja | Ankertext hinter der Adresse, öffnet direkt diese Einheit |
| In WhatsApp teilen | ja | fertiger Text mit Ort, Zeit, Dauer und Link, ein Knopf |
| Draufklicken und zusagen | eingeschränkt | nur mit Zugang zum Artefakt, siehe unten |
| In den Kalender | teilweise | Google ja, Apple nein |

**Was nativ wirklich dazukäme:** verlässliche Push-Nachrichten, Eintrag direkt in den
Apple-Kalender, Platz am Homescreen, später ein Widget.
**Was es kostet:** 99 Euro im Jahr für das Entwicklerprogramm, Review vor jedem Update, und vor
allem eine Installationshürde. Bei acht Leuten ist "installier dir diese App" ein ungleich
größerer Schritt als "klick auf diesen Link". Dazu fehlt Android, also etwa die Hälfte.

**Der Kern des Arguments:** Bei acht bis fünfzehn Personen ist WhatsApp der Push. Eine Nachricht
in der Gruppe erreicht diese Gruppe zuverlässiger als jede Push-Nachricht und kostet nichts. Eine
eigene App ist ein zweiter Kanal, den dieselben Leute zusätzlich beachten müssten.

**Die echte Hürde ist nicht nativ gegen Web, sondern der Zugang.** Das aktuelle Werkzeug liegt
auf claude.ai und verlangt Anmeldung plus Schreibrecht. Ein Link in der WhatsApp-Gruppe
funktioniert für Fremde deshalb nicht. Das löst eine native App genauso wenig, die bräuchte
dasselbe eigene Backend.

**Stufenplan:**

| Stufe | Wann | Was |
|---|---|---|
| 0, jetzt | bis etwa 15 Personen | aktuelles Werkzeug, Zugang einzeln per Einladung |
| 1 | ab etwa 15, oder sobald jemand ohne Einladung zusagen soll | eigene Web-App auf eigener Adresse, Link ohne Anmeldung, iOS und Android, zum Homescreen hinzufügbar, Apple-Kalender über .ics. Aufwand: ein paar Stunden plus zwei Konten |
| 2 | nur wenn Erinnerungen der Engpass sind | Push, dann zuerst als PWA, nativ erst wenn das nicht reicht |

**Prüffrage für Stufe 1:** Sagt in den ersten vier Wochen jemand von sich aus, dass er den Termin
gern im Kalender hätte oder die Seite nicht öffnen kann? Wenn nein, war es nie das Problem.
**Wiedervorlage:** bei 15 aktiven Personen.

---

## D-037 Neustart am 09.01.2027, Winteranker ist der lange Lauf

**Datum:** 2026-11-04
**Ausgangslage:** Weder der 19.09. noch der 17.10. haben stattgefunden, auch keiner der Samstage
danach. Stand im `LOGBUCH.md`.
**Entscheidung:** Neustart am Samstag, 09.01.2027. Der einzige fixe Anker ist ab dann ein langer
Lauf, nicht mehr die Ausfahrt.

| | Bisher | Ab 09.01.2027 |
|---|---|---|
| Format | lange Ausfahrt, GA1 | langer Lauf, GA1 |
| Zeit | Samstag 08:00 | Samstag 09:00 |
| Treffpunkt | Reichsbrücke Nord | Praterstern, Beginn Hauptallee |
| Lang | 110 km | 18 km, zwei Runden Hauptallee bis Lusthaus und retour |
| Kurz | 70 km ab Abzweig Orth | 9 km, Ausstieg nach Runde 1 am Start |
| Gruppen | 30–32 / 33–35 km/h | 6:15–5:45 / 5:45–5:15 min/km |

**Begründung:**
- Eine 110-km-Ausfahrt ist von November bis Februar in Wien kein verlässlicher Termin. Kälte,
  Nässe, Glätte und Dunkelheit machen aus "findet statt, egal wer zusagt" ein Versprechen, das
  man nicht halten kann. Verlässlichkeit ist aber das ganze Angebot
- Der lange Lauf steht bei allen Formaten der Zielgruppe im Winterplan, Triathlon, Marathon,
  Trail und Hyrox. Er bedient damit die breiteste Gruppe aus D-014
- Kein Raum, keine Kosten, keine Verhandlung, kein Material. Die Hauptallee ist beleuchtet, flach
  und gut erreichbar
- Die Runde erfüllt D-021 von selbst: gemeinsamer Start, benannter Ausstieg nach Runde 1, und
  niemand ist am Ende weit weg vom Ausgangspunkt
- 09:00 statt 08:00, weil es im Jänner erst gegen 07:45 hell wird
- Jänner statt sofort: Anfang Jänner beginnt bei fast allen der Aufbau, Vorsätze sind frisch, und
  die Zeit bis dahin reicht, um die Einladungen rechtzeitig vor den Feiertagen rauszuschicken

**Nicht entschieden:** Ob die Ausfahrt im Frühjahr zurückkommt. Das entscheidet sich an den Zahlen
im Logbuch, frühestens im März.
**Prüfung:** Die Distanzen sind **[Hypothese]**. Die Runde wird bis 13.12. einmal gelaufen und
gemessen, im Rahmen des eigenen Trainings.
**Wiedervorlage:** nach dem dritten durchgeführten Samstag, spätestens März 2027.

---

## D-038 Der Engpass ist der Versand. Bis er erledigt ist, wird nichts anderes gemacht.

**Datum:** 2026-11-04
**Befund:** Der Start ist nicht am Konzept gescheitert, nicht am Wetter und nicht an der App. Die
acht Einladungen aus `docs/18-start-kit.md` sind nie verschickt worden. Gleichzeitig sind in
derselben Zeit 18 Dokumente, 36 Entscheidungen, eine Website und eine App entstanden. Schreiben
und Bauen fühlen sich wie Fortschritt an und haben das eine ersetzt, was den Plan testet.
**Entscheidung:**
1. **Versandfrist So 15.11.2026.** Bis dahin gehen acht Einzelnachrichten raus, als Ankündigung für
   den 09.01. Früh statt knapp, weil eine Einladung für Jänner für beide Seiten leichter ist als eine
   für übermorgen, und weil acht Leute, die Bescheid wissen, aus dem Plan eine Zusage machen
2. **Schreibstopp.** Bis die acht Nachrichten im Logbuch stehen, wird an diesem Repository nichts
   geändert außer dem Logbuch. Kein Konzept, keine Website, keine App
3. **Zeugen.** Der Mitgründer bekommt die Frist mitgeteilt und fragt am 15.11. nach
4. **Kleinster Schritt zuerst.** Erst die acht Namen in die Tabelle, das dauert zehn Minuten. Die
   Nachrichten sind fertig formuliert und werden nur kopiert

**Abbruchkriterium:** Wenn am 15.11. keine acht Nachrichten raus sind, ist das die Antwort, und
zwar eine ehrliche: dann ist es gerade nicht das richtige Projekt, und das Repository wird als
abgeschlossen markiert statt weiter gepflegt. Das ist kein Scheitern, sondern eine Entscheidung.
**Wiedervorlage:** 15.11.2026.

---

## D-039 Repository aufgeräumt, überholte Stände markiert

**Datum:** 2026-11-04
**Entscheidung:** Nur fünf Dateien sind ab jetzt lebendig: `README.md`, `LOGBUCH.md`,
`decisions/DECISIONS.md`, `docs/18-start-kit.md` und `app/windschatten.html`. Alle anderen Dokumente
tragen einen Hinweis, dass sie den Konzeptstand bis Mitte Oktober 2026 zeigen. Sie werden nicht
mehr nachgezogen.
**Damit hinfällig:**
- Anteile, Vesting und Ausstiegsfall (D-008, D-017). Ohne Geld und ohne Unternehmen (D-034) gibt es
  nichts zu verteilen. Was bleibt, ist die Rollenteilung
- Der Stack aus `docs/06-tech-architecture.md`. Gebaut wurde eine einzelne Datei mit geteilter
  Datenbank (D-032). Das bleibt so bis Stufe 1 aus D-036
- Die Phasen der Roadmap. Die neue Abfolge steht in `docs/10-roadmap.md` oben
**Wiedervorlage:** keine.
