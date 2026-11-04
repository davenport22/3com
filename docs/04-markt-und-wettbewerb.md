# 04 Markt und Wettbewerb

> **Konzeptstand bis Mitte Oktober 2026, wird nicht mehr nachgezogen (D-039).** Was aktuell gilt, steht im README und im Entscheidungslog. Der Arbeitstitel 3com heißt heute Windschatten (D-031).

Neu berechnet in v0.3 nach der Verbreiterung auf Ausdauer-Generalisten (siehe 01).

## Marktgröße

### Belegte Zahlen

| Quelle | Zahl | Stand |
|---|---|---|
| Österreichischer Triathlonverband | rund 15.000 Mitglieder in 305 Vereinen | 2021 **[Beleg, veraltet]** |
| Vienna City Marathon | über 42.000 Finisher über alle Bewerbe, Sonntagsbewerbe ausverkauft | 2026 **[Beleg]** |
| Hyrox Vienna (Open European Championships) | rund 8.000 Athletinnen und Athleten aus 79 Ländern | Feb 2025 **[Beleg]** |

Der VCM und Hyrox Vienna sind die beiden größten Aktivsportveranstaltungen des Landes nach
Teilnehmerzahl. Das sagt wenig über die Zielgruppe, aber viel über die Tiefe der Wiener Szene.

### Abgeleitete Marktgröße

Zielgruppendefinition: **trainiert acht Stunden pro Woche oder mehr, strukturiert, auf ein
Renndatum hin, wohnhaft im Großraum Wien.**

| Teilsegment | Schätzung Wien | Grundlage |
|---|---|---|
| Triathlon, Mittel- und Langdistanzambition | 1.500 bis 5.000 | ÖTRV-Ableitung **[Hypothese]** |
| Hyrox, strukturiert trainierend | 1.200 bis 2.500 | Hyrox Vienna 8.000 Starter, davon 79 Nationen, Wien-Anteil 15 bis 25 Prozent **[Hypothese]** |
| Trail und Ultra, mit Renndatum | 800 bis 2.500 | **[Hypothese]** |
| Marathon und Halbmarathon mit strukturiertem Plan über 8 h/Woche | 1.500 bis 4.000 | Ableitung aus VCM-Teilnehmerstruktur **[Hypothese]** |
| Abzug für Mehrfachzählung (dieselben Personen in mehreren Segmenten) | 20 bis 30 Prozent | genau diese Überschneidung ist die Zielgruppe **[Hypothese]** |
| **Serviceable Market Wien** | **5.000 bis 12.000 Personen** | **[Hypothese]** |

**Prüfmethode:** Startlisten auswerten und nach Wiener Postleitzahlen filtern. Ironman Austria
Klagenfurt, 70.3 St. Pölten, Vienna Triathlon, Hyrox Vienna, VCM Marathondistanz, die großen
österreichischen Trailrennen. Das ist die härteste verfügbare Datenquelle, öffentlich, und
kostet einen Nachmittag. Das gehört in die ersten drei Wochen.

### Einordnung

Gegenüber der reinen Triathlon-Definition (1.500 bis 5.000) verdreifacht sich der bedienbare
Markt ungefähr. Mit realistischen Penetrationsraten von 10 bis 20 Prozent ergibt das **500 bis
2.400 aktive Nutzer in Wien**.

Das verschiebt die zentrale Aussage aus v0.1:

> Alt: Wien allein trägt kein Geschäft. Wien ist der Beweis, nicht der Markt.
>
> **Neu: Wien trägt knapp ein kleines Geschäft. Für alles darüber braucht es weiterhin die
> zweite Stadt.**

Das ändert die Ambitionsfrage nicht grundsätzlich, aber es entschärft sie. Ein kostendeckendes
Wien ist jetzt ein plausibles Ergebnis und nicht nur ein Zwischenschritt.

## Wettbewerbslandschaft

### Direkte Substitute in Wien

| Anbieter | Was sie bieten | Wo 3com anders ist |
|---|---|---|
| Triathlonvereine (Tri4You, Sports Monkeys, USC Austria, Triathlon Wien) | Feste Trainingsgruppen, Vereinsstruktur, Lizenzen | Kein Beitrag, keine Verpflichtung, vereins- und disziplinübergreifend |
| Hyrox-affiliierte Gyms und Boxen | Kraft und Format, oft mit Community-Charakter | Deckt die langen Ausdauereinheiten drumherum nicht ab, an ein Studio gebunden |
| Lauftreffs und Shop-Läufe | Regelmäßige Gruppen, meist kostenlos | Eine Disziplin, selten Leistungsdifferenzierung, kein Renndatumsbezug |
| Trail- und Bergsportgruppen | Wochenendtouren, starke Kultur | Saisonal, ortsgebunden, kein Wochenrhythmus |
| Strava Clubs | Rückblickende Aktivitätsanzeige | Vorausschauend, Verabredung statt Dokumentation, Tempo-Matching |
| WhatsApp-Gruppen | Koordination im Bekanntenkreis | Skaliert über den Bekanntenkreis hinaus, durchsuchbar, mit Onboarding |
| Kommerzielle Coachings mit Gruppentraining | Angeleitetes Training | 3com konkurriert nicht, sondern ist deren Distributionskanal |

**Wichtige Beobachtung zur Verbreiterung:** Der Wettbewerb wird dichter, aber er bleibt
fragmentiert. Jeder Anbieter deckt genau eine Disziplin oder genau ein Studio ab. Niemand deckt
den Menschen ab, der über das Jahr zwischen Formaten rotiert. Das ist die Lücke, die durch die
Verbreiterung erst sichtbar wird.

### Produktseitige Analogien

| Produkt | Kategorie | Lernpunkt |
|---|---|---|
| TrainingPeaks, Intervals.icu, MOTTIV | Trainingsplanung | Lösen die Planung. Kein Sozialteil. Integration statt Konflikt. |
| Strava | Aktivitätsnetzwerk | Der Gigant. Konkurrenz nur, wenn 3com den Fehler macht, ein Feed-Produkt zu bauen. |
| Spond, Teamer | Vereinsorganisation | Terminkoordination in bestehenden Gruppen. Kein Discovery, kein Matching. |
| Meetup, Luma | Event-Discovery | Generisch, kein Sportkontext, kein Tempo-Matching |
| Racefully, Runkeeper-Gruppen | Lauf-Communities | Zeigen, wie schwer soziale Layer im Ausdauersport monetarisierbar sind. Warnsignal. |
| Hyrox als Format selbst | Community-getriebenes Rennformat | Das interessanteste Vorbild: Hyrox ist in wenigen Jahren gewachsen, weil Gyms es als Grund zum gemeinsamen Trainieren genommen haben. Genau derselbe Mechanismus. |

### Ehrliche Wettbewerbsbeurteilung, korrigiert in v0.8

**Die frühere Aussage "es gibt keinen direkten Wettbewerber" war falsch.** Die Recherche in
`16-wettbewerb-realitaetscheck.md` hat mehrere nahe Produkte gefunden, darunter Strava Group
Events mit bereits existierenden Tempogruppen, OnlyTri mit Level- und Volumenfiltern, und Pace
mit genau der Serien-plus-Tempogruppen-plus-RSVP-Mechanik aus Dokument 05.

Wichtiger noch: Alle diese Produkte scheitern nicht an Funktionen, sondern an Dichte. BikeCrew
hat 3.000 Nutzer in ganz Europa, CorrerJuntos 1.100 nach Jahren, SportJoe 30 Bewertungen nach
sieben Jahren. Das ist dieselbe Wand, gegen die auch 3com läuft, nur empirisch belegt statt
hergeleitet.

**Siehe Dokument 16 für die vollständige Analyse und die Konsequenzen.**

Der stärkste Wettbewerber ist kein Produkt, sondern **die Gewohnheit, allein zu trainieren,
kombiniert mit WhatsApp**. Gegen "gut genug und schon installiert" gewinnt man nicht mit
Features, sondern damit, dass man Menschen zusammenbringt, die sich vorher nicht kannten. Das
ist der einzige Vorteil, den WhatsApp strukturell nicht haben kann.

## Differenzierungsthese

3com gewinnt, wenn vier Dinge stimmen:

1. **Dichte in einer Stadt.** Genug Leute, dass immer etwas los ist.
2. **Glaubwürdiges Tempo-Matching.** Damit die Angst vor der Fehlpaarung verschwindet.
3. **Verlässliche Rituale.** Damit Zugehörigkeit statt Transaktion entsteht.
4. **Ein Jahresrhythmus statt einer Saison.** Damit niemand im Februar abspringt und im Mai neu
   gewonnen werden muss.

Punkt 4 ist neu in v0.3 und ist der eigentliche Ertrag der Verbreiterung.

## Quellen

- [Österreichischer Triathlonverband, Wikipedia](https://de.wikipedia.org/wiki/%C3%96sterreichischer_Triathlonverband)
- [Vienna City Marathon 2026: über 42.000 Finisher, SPOFERAN](https://spoferan.com/news/vienna-city-marathon-2026-neuer-streckenrekord-und-ueber-42000-finisher-feiern-lauf-festival)
- [Wien Marathon 2026: Sonntagsbewerbe ausgebucht, German Road Races](https://news.germanroadraces.de/wien-marathon-2026-sonntagsbewerbe-sind-ausgebucht-laufbegeisterung-hat-neues-level-erreicht/)
- [Hyrox in Wien, rund 8.000 Athleten aus 79 Ländern, sportsbusiness.at](https://sportsbusiness.at/hyrox-auch-in-wien-kraft-ausdauer-und-globales-wachstum-exklusiv/)
- [HYROX Vienna, Red Bull](https://www.redbull.com/at-de/hyrox-vienna)
- [Tri4You Triathlonverein Wien](https://www.triathlonverein-wien.at/)
- [Sports Monkeys Triathlon Club](https://www.tri.sportsmonkeys.at/)
- [Triathlon Wien](https://triathlon-wien.com/)
- [USC Austria Trainingsgruppen](https://www.ultimatesportclub.com/traininggroups)
- [Intervals.icu](https://www.intervals.icu/)
- [Indoor-Cycling Studios Wien, Eversports](https://www.eversports.at/l/indoor-cycling/wien)
