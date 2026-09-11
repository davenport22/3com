# 16 Wettbewerb, Realitätscheck

Recherchiert am 11.09.2026. **Dieses Dokument widerlegt eine zentrale Annahme aus v0.1 bis v0.7.**

## Die Kernaussage

In Dokument 04 stand bisher: "Es gibt keinen direkten Wettbewerber." Das stimmt nicht. Es gibt
mehrere, teils sehr nahe, und den gefährlichsten baut Strava gerade selbst.

Gleichzeitig zeigt die Recherche etwas Zweites, das noch wichtiger ist: **Diese Produkte
scheitern nicht an Funktionen, sie scheitern an Dichte.** Das trifft exakt die Wand, gegen die
auch 3com läuft.

## Die Wettbewerbslandschaft

| Produkt | Was es tatsächlich tut | Wo es aufhört | Bedrohung |
|---|---|---|---|
| **Strava Group Events** | Club-Events mit Typ (Social, Workout, Competition), Route, RSVP-Limit und **bis zu vier Tempogruppen pro Event**, Einheit frei wählbar | Keine wiederkehrenden Events, nur Club-Admins dürfen erstellen, kein Intensitätsfeld, kein Matching | **hoch** |
| **Strava Events-Tab (Juli 2026)** | Neuer Reiter: Races, Gruppenläufe, Filter nach Distanz, Datum, Ort, Sportart. Runna-Integration. Über 1 Mio Clubs, Run-Club-Mitgliedschaften plus 59 Prozent in 2025 | Noch kein Tempo-Grouping im neuen Tab, keine Serien | **hoch** (Distribution) |
| **OnlyTri** | Triathlon-Netzwerk mit Filter nach **Pace, Wochenvolumen, Level**, Gruppen-Swims, Rides, Runs, Bricks und Race-Simulationen mit GPS-Startpunkt | Serien nicht bestätigt, kein Intensitätsvokabular, **null verifizierbare Traktion** | **hoch** |
| **Pace (paceclubapp.com)** | **Wiederkehrende Termine, Tempogruppen, RSVP pro Datum, Kapazität, Warteliste, Erinnerungen, Anwesenheit, Discovery-Map** | Werkzeug für bestehende Clubs, nicht für Fremde untereinander. Noch Waitlist | **hoch** |
| **CorrerJuntos** | Matching-Algorithmus mit Gewichtung: Pace 30, Zeitplan 25, Fitnesslevel 25, Ziele 10, Aktivitätstyp 10 Prozent | Praktisch nur Spanien, nur Laufen, **1.100 registrierte Läufer nach Jahren** | mittel |
| **SportLync** | Discovery nach Ort und Level, geplante Sessions mit RSVP und Anwesenheit | Multi-Sport-Breite statt Ausdauer-Tiefe, Traktion nicht verifiziert | mittel |
| **BikeCrew** | Radfahrer-Matching mit Profil, Bike-Typ und Pace, Gruppenfahrten | **3.000 aktive Fahrer in ganz Europa**, keine Serien | mittel |
| **Hyrox-Cluster** (RoxConnect, HYBUDDY, HyroxMatch, Roxly, HyPair, findhyroxpartner) | Matching nach Leistungslevel und Stationsstärken für Doubles und Relay | Rennpartnersuche, nicht wiederkehrendes Training. **RoxConnect: 16 Bewertungen nach über einem Jahr** | mittel |
| **Spond** | Vereinsverwaltung mit Serien, Verfügbarkeitsabfragen, Untergruppen | **Gruppen sind invite-only und nicht auffindbar.** Löst exakt nicht das Fremden-Problem | niedrig |
| **Komoot Group Activities** | Einladung zu geplanter Route, Echtzeit-Updates | Explizit kein Public Discovery, keine Serien, kein Level | niedrig |
| **Zwift Meetups** | "Keep Everyone Together" hält Fahrer unabhängig von der Leistung zusammen | Virtuell. Löst das Levelproblem durch Aufheben der Physik | niedrig |
| **DACH: Spontacts, sportpartner.com, SportJoe, spird** | Freizeit- und Sportpartnerbörsen, teils mit Wien-Seiten | Keine Session-Logik, kein Level, keine Serien. **SportJoe: 30 Bewertungen nach sieben Jahren** | niedrig |

## Die drei nächsten Nachbarn

**OnlyTri** ist konzeptionell etwa 80 Prozent deckungsgleich: Filter nach Pace, Volumen und
Level, plus Gruppen-Sessions inklusive Koppeleinheiten und Rennsimulationen. Was fehlt, ist das
Intensitätsvokabular und eine bestätigte Serienmechanik. Was auffällt: keine verifizierbare
Traktion, in keinem großen Branchenreview 2026 erwähnt. Konzeptionell nah, operativ möglicherweise leer.

**Strava Group Events** hat als einziges großes Produkt bereits Tempogruppen, bis zu vier pro
Event. Damit ist die Level-Dimension bei Strava gesetzt. Es fehlen Wiederholung,
Intensitätstaxonomie und das Erstellungsrecht für normale Nutzer. Etwa die Hälfte des Konzepts
existiert bereits bei einem Anbieter mit über einer Million Clubs.

**Pace (paceclubapp.com)** hat exakt die Mechanik aus Dokument 05: Serien plus Tempogruppen plus
RSVP pro Termin plus Kapazität plus Discovery. Unterschied ist nur das Framing, gebaut für
Organisatoren bestehender Clubs statt für den einzelnen Athleten.

## Gescheiterte Versuche

- **Any Distance** (2025 Open Source gegangen): Der Gründer nennt "co-founder issues, PMF (or
  rather a lack thereof), burnout, and fundraising challenges". Eine von Apple gefeaturete,
  designpreisgekrönte Running-App ohne Product-Market-Fit.
- **Racefully**: Pivot vom Consumer-Social-Running zu Corporate Wellness.
- **Runens** (2011, New York): Social-Running-App, TechCrunch nannte die Social-Features schon
  damals "considerably underdeveloped". Heute verschwunden.
- **spird** (AT): Website seit Januar 2023 unverändert, faktisch eingeschlafen.
- **SportJoe** (DE, seit 2018): nicht gescheitert, aber 30 Store-Bewertungen nach sieben Jahren.
  Das ist aussagekräftiger als ein Shutdown: Das Produkt lebt, der Markt nimmt es nicht an.

Kein einziger dokumentierter Shutdown eines gut finanzierten Trainingspartner-Startups. Der
Grund ist vermutlich nicht, dass die Kategorie funktioniert, sondern dass sie nie nennenswertes
Kapital eingesammelt hat.

## Was das für 3com bedeutet

### 1. Die Annahme "das gibt es noch nicht" ist widerlegt

Tempogruppen plus Sessiontyp gibt es bei Strava heute. Level-plus-Session-Matching gibt es bei
OnlyTri und CorrerJuntos. Serien plus Tempogruppen plus RSVP gibt es bei Pace. Die
Differenzierung muss präziser sein als "zweidimensionales Matching", weil beide Dimensionen
bereits bedient werden.

### 2. Der einzige verifizierte weiße Fleck ist das Intensitätsvokabular

Kein gefundenes Produkt führt GA1, Schwelle oder Intervall als strukturiertes Feld. Strava hat
nur Social, Workout, Competition. Das ist der schmale, aber echte Unterschied. Ob ein einzelnes
Datenfeld ein Unternehmen trägt, ist eine andere Frage. Als Community-Merkmal trägt es, als
Burggraben nicht.

### 3. Das Muster über alle Anbieter ist Dichteversagen

BikeCrew 3.000 Nutzer in ganz Europa. CorrerJuntos 1.100 nach Jahren. RoxConnect 16
Bewertungen. SportJoe 30 nach sieben Jahren. Die Produkte funktionieren technisch. Sie haben nur
nie genug Menschen am selben Ort zur selben Zeit. Das ist exakt die Wand aus H1 und aus Musks
Koinzidenzrechnung, nur diesmal empirisch belegt statt hergeleitet.

### 4. Der Hyrox-Cluster ist die unangenehmste Lektion

Sechs Anbieter, eine global schnell wachsende Sportart mit rund 1,5 Millionen Startern in der
Saison 2025/26, und ein **zwingender** Partnerbedarf: Ohne Doubles-Partner kann man nicht
starten. Trotzdem hat keiner dieser Anbieter Traktion.

Der Bedarf bei 3com ist schwächer als das. Man kann allein trainieren. Wenn ein Muss-Bedarf kein
Produkt trägt, trägt ein Kann-Bedarf vermutlich auch keines.

### 5. Strava ist die realistische Bedrohung, nicht die Startups

Runna-Übernahme 2025, The Breakaway 2025, Events-Tab 2026, Tempogruppen bereits gebaut,
Run-Club-Mitgliedschaften plus 59 Prozent. Wenn Strava wiederkehrende Club-Events ergänzt, ist
das Konzept ein Feature. Das ist ein plausibler nächster Schritt, kein Extremszenario.

### 6. Was das nicht bedeutet

Eine lokale, nicht skalierende Version für eine Stadt kann trotzdem funktionieren, **weil sie
das Dichteproblem umgeht statt es zu lösen**: über manuelle Kuratierung, feste Anker und eine
bestehende Offline-Community. Genau das ist der Weg, den die Roadmap ohnehin beschreibt.

**Als Community für Wien: plausibel. Als Produktthese: deutlich schwächer belegt als angenommen.**

## Die Konsequenz für das Konzept

Die Recherche verschiebt das Gewicht zwischen den beiden Hälften des Vorhabens:

| | Vorher | Nachher |
|---|---|---|
| Community in Wien | der Weg zum Produkt | **der eigentliche Wert** |
| Die App | das Produkt | ein Werkzeug für die Community, kein Geschäft |
| Skalierung über Städte | der Beweis | unwahrscheinlich, weil alle Vergleichsfälle daran gescheitert sind |
| Der Burggraben | Tempo-Matching | lokale Dichte und reale Beziehungen, die nicht migrierbar sind |

Das Ambitionsniveau aus Dokument 00 verschiebt sich damit weg von "skalierbare Plattform" und
hin zu "Community oder kleines, kostendeckendes Geschäft in einer Stadt". Das ist keine
schlechte Nachricht, es ist eine ehrliche.

**Praktische Folge:** Der Bau der App im Winter bleibt sinnvoll, aber mit klar reduziertem
Anspruch. Sie ist das Betriebssystem für fünf Serien, nicht ein Startup. Wenn im Winter die Wahl
zwischen zwei Wochen Feature-Arbeit und zwei Wochen Gastgeberakquise steht, gewinnt ab jetzt
immer die Akquise.

## Quellen

- [Strava Support: Group Events for Clubs](https://support.strava.com/hc/en-us/articles/216918607-Group-Events-for-Clubs)
- [9to5Mac: Strava gets an Events tab (Juli 2026)](https://9to5mac.com/2026/07/09/strava-gets-an-events-tab-with-upcoming-races-group-runs-more/)
- [DC Rainmaker: Strava Acquires Runna](https://www.dcrainmaker.com/2025/04/strava-acquires-runna-thoughts-forward.html)
- [OnlyTri](https://onlytri.app/)
- [Pace (paceclubapp)](https://paceclubapp.com/)
- [CorrerJuntos](https://www.correrjuntos.com/)
- [BikeCrew](https://www.bikecrew.app/)
- [RoxConnect](https://roxconnect.com/) · [HYBUDDY](https://hybuddy.net/)
- [Spond Help: Recurring Event](https://help.spond.com/app/en/articles/140738-recurring-event)
- [Komoot: Organize and manage group activities](https://support.komoot.com/hc/en-us/articles/10374965887130-Organize-and-manage-group-activities)
- [Zwift Insider: Keep Everyone Together](https://zwiftinsider.com/keep-everyone-together/)
- [Daniel Kuntz: Open Sourcing Any Distance](https://kuntz.io/blog/any-distance-oss.html)
- [Breadcrumb.vc: Network Liquidity, The Spontaneous Togetherness Problem](https://breadcrumb.vc/the-network-liquidity-map-why-time-matters-1cda5901fb49)
- [SportJoe im App Store](https://apps.apple.com/de/app/sportjoe-deine-sportcommunity/id1359031605)
- [Spontacts Laufen Wien](https://spontacts.com/laufen-joggen/wien)
