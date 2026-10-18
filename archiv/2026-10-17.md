# Bundesliga-Tipps – 7. Spieltag 2026/27 (Stand: 17.10.2026)

**Ansetzung:** Freitag, 23.10. bis Sonntag, 25.10.2026.
**Vortagsstand:** 15.10.2026, **6. Spieltag** — also ein anderer, inzwischen angelaufener Spieltag. **Für alle neun Partien gilt daher: „neuer Spieltag — kein Vergleich möglich".**

**Ergebnis dieses Laufs in einem Satz:** **Der 6. Spieltag läuft, also wechsele ich auf den 7. Spieltag — neun neue Tipps ohne Vergleichsmöglichkeit.** **Zwei Dinge muss ich dabei ausdrücklich voranstellen:** ***erstens ist der Lauf vom 16.10. ausgefallen*** (kein Commit, kein Archiveintrag — der Vortagsstand ist zwei Tage alt, nicht einen), ***und zweitens sind zwei Partien des 6. Spieltags noch nicht gespielt*** (Leverkusen – Freiburg und Gladbach – Hoffenheim am Sonntag), **sodass die Tabelle, auf der diese Tipps stehen, bei vier Vereinen erst fünf statt sechs Spiele umfasst.** **Dazu die Abrechnung des 6. Spieltags: von sieben gespielten Partien habe ich drei Tendenzen richtig und keinen Endstand exakt getroffen.** **Die Quellensperre besteht zum siebten Tag.**

---

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Der Befund der Vortage ist heute erneut geprüft und unverändert.**

- **Der Proxy ist funktionsfähig.** `curl -sS "$HTTPS_PROXY/__agentproxy/status"` lief durch: `enabled: true`, `bundleCoversEveryHost: true`, `recentRelayFailures: []`.
- **Die Fußballquellen bleiben durch die Egress-Policy dieser Umgebung gesperrt.** Heute zwei Testabrufe, beide gescheitert: `www.kicker.de` und `www.bundesliga.com` enden mit `CONNECT tunnel failed, response 403`. ***Das ist eine Richtlinienablehnung, kein Quellenproblem*** — und `/root/.ccr/README.md` schreibt für 403 ausdrücklich vor, den gesperrten Host zu melden statt die Sperre zu umgehen.
- **Auch `WebFetch` scheitert weiterhin, und zwar schon bei der Namensauflösung.** Heute getestet: `anstosszeiten.de` → `getaddrinfo ENOTFOUND`. **Beide Abrufwege sind zu, auf zwei verschiedene Weisen** — das bestätigt den präzisierten Befund vom 15.10.
- ***Was der Nutzer tun kann, wenn er Volltexte will:*** **Im Menü der Cloud-Umgebung in der Titelzeile der Sitzung → „Edit" → Network access**: entweder eine breitere Zugriffsstufe wählen oder `kicker.de`, `bundesliga.com`, `weltfussball.de` und `transfermarkt.de` unter **Allowed domains** eintragen (Häkchen „Allow package managers" gesetzt lassen). Dokumentiert unter https://code.claude.com/docs/en/cloud-environments#network-access. **Solange das so bleibt, kann ich die vier im Routine-Prompt genannten Leitquellen dauerhaft nicht im Volltext lesen.**
- **`WebSearch` funktioniert und war wieder die tragende Quelle.** **Alles Folgende steht auf Suchergebnis-Zusammenfassungen und -Titeln, kein Volltext.**
- ***Qualitativer Befund des Tages:*** **Für einen Spieltag, der erst in sechs Tagen beginnt, ist die Lage naturgemäß dünn — es gibt keine Spieltags-Pressekonferenz, keine Aufstellung und kein Kaderaufgebot zum 7. Spieltag, und es kann sie heute auch nicht geben.** *Dafür ist die Ergebnis- und Verletzungslage zum gerade laufenden 6. Spieltag ungewöhnlich gut belegt: **sieben Spielberichte mit Torfolgen, dazu zwei Sonntags-Vorberichte mit Verletztenlisten für vier Vereine.*** **Zwei seit Tagen offene Lücken sind damit geschlossen** (Terriers Diagnose, eine belastbare Paderborner Ausfallliste).

### Der ausgefallene Lauf vom 16.10.

**Das gehört an den Anfang, weil es den Vergleichsmaßstab verschiebt.** **`git log` zeigt als jüngsten Commit „Bundesliga-Tipps 2026-10-15"; ein Commit vom 16.10. existiert nicht, und `archiv/` enthielt bis heute nur Stände bis zum 14.10.** **Der Lauf vom 16.10. ist also ausgefallen** — *den Grund kann ich von hier aus nicht feststellen; der Arbeitsbaum war sauber, es liegen keine nicht committeten Reste und keine Fehlerspuren im Repo.* **Folge für heute: der „Vortagsstand", mit dem ich vergleiche, ist der vom 15.10. und damit zwei Tage alt.** *Praktisch macht das hier wenig Unterschied, weil ohnehin der Spieltag wechselt — aber es heißt, dass die Freitagspartie Frankfurt – Köln nie einen Lauf nach ihrem Anpfiff gesehen hat.*

---

## Die Nachrichtenlage

**Der 6. Spieltag ist zu sieben Neunteln gespielt, und er hat die Tabellenspitze gedreht.** **Der FC Bayern hat RB Leipzig 6:1 geschlagen** — Luis Díaz mit einem Dreierpack (12., 47., 69.), dazu Pavlović (26.), Olise (34.) und Kane (53.), für Leipzig traf Andrija Maksimović in der Nachspielzeit. **Zur Pause stand es 3:0.** ***Für meine Tipps wichtiger als das Ergebnis: Jonas Urbig stand erneut im Tor, Manuel Neuer hat auch dieses Spiel nicht gespielt.*** *Damit ist die Frage vom 15.10. („Neuers Status für Samstag ist offen") in einem Punkt beantwortet — er hat gefehlt —, aber eine Diagnose oder ein Rückkehrdatum liegt weiterhin nicht vor.*

**Bei Leipzig ist daraus binnen Stunden eine Trainerdebatte geworden.** **Martín Demichelis steht „mehr denn je in der Kritik"**; **Lothar Matthäus bemängelte, dass der überraschende Startelfeinsatz von Lukas Klostermann nicht zur Pause korrigiert wurde**, Demichelis selbst wehrte sich dagegen, die Niederlage an einem Namen festzumachen („man könne in München verlieren, aber nicht so"), **Sportchef Marcel Schäfer zeigte sich nach dem Spiel verärgert.** *Ein englischsprachiger Bericht nennt die Ablösung Ole Werners im Rückblick eine schwache Entscheidung.* ***Das ist für Partie 4 der Kern: Leipzig empfängt Elversberg drei Tage nach dem Auswärtsspiel bei Real Madrid und mitten in dieser Debatte.***

**Der zweite große Strang ist Dortmunds Torflaute.** **Beim 0:0 bei Union Berlin ist der BVB das dritte Pflichtspiel in Folge ohne eigenen Treffer geblieben** (Remis gegen Werder, 0:1 in Bodø, 0:0 in Berlin). **23 Torschüsse zusammen, aber nur Dortmunds kamen aufs Tor; die beste Gelegenheit vergab Ethan Nwaneri kurz vor der Pause gegen Frederik Rönnow.** **Kovač lobte Leidenschaft und Intensität, sagte aber, man habe die Spielkontrolle nicht in genug gute Chancen übersetzt.** *Von den Rängen und in den Fanreaktionen kam „Kovac out"; Nils Petersen kritisierte, dass erst nach 60 Minuten gewechselt wurde.* **Dortmund steht mit 14 Punkten dennoch vorn — die Abwehr hat in sechs Spielen vier Gegentore.**

***Die kurioseste Szene des Spieltags hat sich als Nichtigkeit erwiesen, und das ist eine wichtige Entwarnung:*** **Schiedsrichter Daniel Schlager zeigte Nwaneri nach rund 18 Sekunden die Rote Karte, hatte aber die falsche Karte aus der Hosentasche gezogen.** **Er entschuldigte sich, nahm die Karte sofort zurück und gab Gelb — ohne Videobeweis.** **Nwaneri blieb auf dem Platz.** ***Es gibt also keine Dortmunder Sperre für Partie 7.*** *Nebenbei ist damit auch die Schlotterbeck-Frage erledigt, die am 15.10. meine schwierigste Entscheidung war: **Schlotterbeck hat in Berlin gespielt** und wird in den Einzelkritiken neben Anton als herausragend geführt.*

**Drittens die Aufsteiger, und hier liegt die Überraschung des Spieltags.** **Die SV Elversberg hat den FC Augsburg 4:3 geschlagen** — nach 28 Minuten stand es 3:0 (Petkov 4., Günther 7., Rohr 28.), Augsburg kam über Rieder (45.+9, Elfmeter), Gregoritsch (76., Elfmeter) und Kömür heran, Schmahl hatte in der 89. auf 4:2 gestellt. **Vier Elfmeter in einem Spiel; Noel Futkeu setzte einen davon in der Nachspielzeit an die Latte.** **Elversberg zieht damit an Augsburg vorbei.** **Der zweite Aufsteiger, Paderborn, hat bei Werder 2:2 gespielt und dabei 2:0 geführt** (Marino 18., Tigges 30.) — **Niclas Füllkrug drehte die Partie mit zwei Treffern (59., 65./66. per Elfmeter) fast allein**, und **Rayan Philippe traf in der Nachspielzeit aus wenigen Metern nur den Pfosten.** ***Werder ist damit die erste Bundesligamannschaft, die dreimal in Folge einen Zwei-Tore-Rückstand aufgeholt und wenigstens einen Punkt behalten hat; sechs Punkte nach Rückstand sind Ligabestwert.*** *Thioune war dennoch verärgert und sagte, nach den Torchancen müsse Werder das Spiel gewinnen; Mitchell Weiser kam zur Pause und stabilisierte das Spiel — **am 15.10. war er noch „wohl kein Startelf-Kandidat".***

**Viertens die beiden Kellerkinder des Spieltags.** **Schalke hat zu Hause 0:1 gegen Mainz verloren und ist im dritten Heimspiel nach dem Wiederaufstieg ohne eigenen Treffer geblieben.** **Phillip Tietz traf in der 24. Minute nach Vorlage von Anthony Caci — sein fünftes Ligator.** **Loris Karius wurde zum Spieler des Spiels gewählt und hat laut `reviersport.de` eine deutlichere Niederlage verhindert.** **Und Eintracht Frankfurt hat den 6. Spieltag mit einem 1:0 gegen Köln eröffnet** — **Younes Ebnoutalib traf in der 77. Minute nach Vorlage des eingewechselten Noël Aséko aus spitzem Winkel**, es war **Frankfurts erster Heimsieg in der Liga seit März**, sechs Tage nach dem 0:6 in Leipzig. *Hütter nannte den Sieg „aufgrund der zweiten Halbzeit verdient".*

**Fünftens, und für Partie 1 entscheidend: Gladbachs Verletzungslage ist die schlechteste der Liga.** **Vor dem Kellerduell gegen Hoffenheim am Sonntag fehlen Kapitän Tim Kleindienst (Muskelfaserriss, „diesmal an einer anderen Stelle" — also ein erneuter Rückschlag) und Jan Leszczyński (Kniestauchung); Fritz Fleck, Franck Honorat, Ko Itakura, Jens Castrop und Enzo Leopold sind nicht dabei oder angeschlagen.** **Kevin Diks ist nach Blessins Worten „frisch" und verfügbar, bei Nicolas Kühn ist nach Muskelbündelriss offen, ob er zurückkehrt.** *Ein Bericht spricht von einer „Muskel-Seuche", die den Trainer „fuchst".* **Gladbach ist punktlos Letzter, Blessin hat am Sonntag seine Heimpremiere.**

**Sechstens Kölns Sturmnotstand, der jetzt genauer belegt ist als an allen Vortagen.** **Ellyes Skhiri hat sich im Derby am 11.10. am Sprunggelenk verletzt; Trainer René Wagner rechnet in diesem Kalenderjahr nicht mehr mit ihm und hofft auf Anfang 2027.** **Thijs Dallinga hat sich im Testspiel gegen Viktoria Köln am 03.10. einen Kreuzbandriss zugezogen und fehlt Monate.** **Ragnar Ache hat aus demselben Spiel eine Muskelverletzung, ein Bericht erwartet ihn im November.** **Imad Rondic (Oberschenkelmuskulatur) und Rav van den Berg (Muskelverletzung) sind ohne Rückkehrdatum, Timo Hübers ist langzeitverletzt — und seit heute droht auch Joël Schmied auszufallen.** ***Neu und wichtig:*** **Köln hat keinen Ersatzstürmer verpflichtet; Sportdirektor Thomas Kessler will das Thema im Januar angehen. Luca Waldschmidt ist aus einer Verletzung zurück und kann vorn spielen, Marius Bülter ist die zweite Option.**

**An der Spitze liegt nach den Samstagsspielen der FC Bayern mit 22:5 Toren vor Dortmund, beide 14 Punkte; Freiburg kann am Sonntag wieder vorbeiziehen.** **Ein DFB-Pokalspiel liegt in der kommenden Woche nicht an, eine Länderspielpause läuft nicht.** ***Zu beachten: in der Nacht zum Sonntag, 25.10.2026, wird die Uhr auf Winterzeit zurückgestellt — die beiden Sonntagsspiele des 7. Spieltags finden also in MEZ statt.***

### Die Europapokalwoche vor dem 7. Spieltag — sieben deutsche Teams, alle vor dem Spieltag

**Das ist der wichtigste Belastungsbefund dieses Laufs, weil er sechs der neun Partien berührt.**

| Tag | Partie | Wettbewerb | Lage | Bundesligaspiel danach |
|---|---|---|---|---|
| **Di 20.10., 18:45** | Sabah FC – **Borussia Dortmund** | Champions League | **auswärts, Aserbaidschan** | Sa 18:30 **heim** (4 Tage) |
| **Di 20.10., 21:00** | **VfB Stuttgart** – Atlético Madrid | Champions League | heim | **Fr 20:30 heim (3 Tage)** |
| **Mi 21.10., 21:00** | **FC Bayern** – FC Arsenal | Champions League | heim | So 17:30 **auswärts** (4 Tage) |
| **Mi 21.10., 21:00** | Real Madrid – **RB Leipzig** | Champions League | **auswärts, Madrid** | **Sa 15:30 heim (3 Tage)** |
| **Do 22.10.** | **Bayer Leverkusen** – Gegner offen | Europa League, 3. Spieltag | offen | So 15:30 **auswärts** (3 Tage) |
| **Do 22.10.** | **TSG Hoffenheim** – Gegner offen | Europa League, 3. Spieltag | offen | So 15:30 **heim** (3 Tage) |
| **Do 22.10.** | **SC Freiburg** – Gegner offen | Conference League | offen | So 17:30 **heim** (3 Tage) |

**Belegt ist der Termin:** **der 2. Spieltag der Europa-League-Ligaphase war am 15.10., der 3. Spieltag ist am 22.10.2026** (deutsche Wikipedia zur Europa League 2026/27, dazu eine `kicker.de`-Spielplanzeile, die für Leverkusen den 22.10. als 3. Spieltag führt). **Die Gegner für den 22.10. habe ich zu keinem der drei Vereine auflösen können** — *die Lostöpfe sind bekannt (Hoffenheim: Lyon, Olympiakos, Ferencváros, Anderlecht, Sturm Graz, Crystal Palace, Beşiktaş, OFI Iraklion; Freiburg: Panathinaikos, Monaco, Twente, Trabzonspor, Jablonec, Kauno Žalgiris), aber nicht in Spieltagsreihenfolge.* **Das ist eine offene Lücke, die ich unten ausdrücklich führe.**

***Zwei Belastungsbefunde ragen heraus:*** **Stuttgart spielt Freitag 20:30, nur drei Tage nach Atlético Madrid — die kürzeste Pause des Spieltags.** **Und Leipzig empfängt Elversberg Samstag 15:30, drei Tage nach einem Auswärtsspiel im Bernabéu.** *Bei Hoffenheim – Leverkusen und Freiburg – Bayern heben sich die Belastungen dagegen weitgehend auf, weil beide Beteiligten jeweils international gespielt haben.*

---

## Abrechnung des 6. Spieltags — meine Tipps gegen die Ergebnisse

**Sieben der neun Partien sind gespielt. Das ist die Bilanz, ungeschönt:**

| Partie | Mein Tipp (15.10.) | Ergebnis | Tendenz |
|---|---|---|---|
| Frankfurt – Köln | **3:1** | **1:0** | **richtig** (Heimsieg) |
| Schalke – Mainz | **1:2** | **0:1** | **richtig** (Auswärtssieg) |
| Elversberg – Augsburg | **1:2** | **4:3** | falsch |
| Werder – Paderborn | **2:1** | **2:2** | falsch |
| Union – Dortmund | **1:2** | **0:0** | falsch |
| HSV – Stuttgart | **1:2** | **1:0** | falsch |
| Bayern – Leipzig | **2:1** | **6:1** | **richtig** (Heimsieg) |
| Leverkusen – Freiburg | **3:2** | *So 15:30* | offen |
| Gladbach – Hoffenheim | **1:1** | *So 17:30* | offen |

**Drei von sieben Tendenzen richtig, kein Endstand exakt.** ***Vier Punkte, die ich daraus mitnehme, und zwar die unbequemen:***

1. ***Meine beiden Änderungen vom 15.10. haben nichts verbessert.*** **Frankfurt – Köln habe ich von 2:1 auf 3:1 gezogen, weil Kölns Sturm zusammengebrochen war — tatsächlich endete es 1:0.** *Die Tendenz war beide Male richtig, aber der alte Tipp lag näher am Ergebnis. **Der Schluss „Gegner ohne Stürmer, also mehr Heimtore" war falsch: Köln hat zwar nicht getroffen, aber Frankfurt hat auch nur einmal getroffen** — die Partie wurde eng, nicht einseitig.* **Das ist ein Denkfehler mit Tendenz: Ausfälle beim Gegner schlagen sich eher in dessen Toren nieder als in meinen.**
2. ***Meine Zurückhaltung bei Union – Dortmund war richtig, aber nicht richtig genug.*** **Am 15.10. habe ich ausführlich begründet, warum ich nicht auf 1:3 gehe, und das 1:2 „die wahrscheinlichste Fehlstelle dieses Laufs" genannt.** **Es endete 0:0 — also lag 1:2 falsch, aber 1:3 wäre deutlich falscher gewesen.** *Was ich übersehen habe, ist nicht Dortmunds Personal, sondern Dortmunds Torflaute: der BVB war schon vor Berlin zwei Spiele ohne Treffer. **Diese Serie stand mir zur Verfügung und ich habe sie nicht gewichtet.*** **Das ist die eigentliche Lehre dieses Spieltags für mich, und sie geht direkt in Partie 7 ein.**
3. ***Die beiden Aufsteiger habe ich zweimal unterschätzt.*** **Elversberg habe ich eine Heimniederlage gegen Augsburg zugetraut (1:2) — sie führten nach 28 Minuten 3:0.** **Paderborn habe ich bei Werder eine 1:2-Niederlage zugetraut — sie führten 2:0 und standen in der Nachspielzeit am Pfosten vor dem Sieg.** *In beiden Fällen bin ich von der Tabelle ausgegangen, nicht von der Spielweise. **Für Partie 4 und Partie 6 korrigiere ich das heute ausdrücklich.***
4. ***HSV – Stuttgart ist der Tipp, der am klarsten an einer falschen Annahme hing.*** **Ich hatte Stuttgart nach dem 3:0 in Bratislava auswärts stärker eingeschätzt als den HSV zu Hause.** **Tatsächlich hatte Stuttgart die besseren Chancen** (Undav an den Pfosten in der 40., Poulsen und Undav an Heuer Fernandes), **verlor aber 0:1 durch Muheims Schuss aus 25 Metern in der 88.** *Die Chancenverteilung stützt meine Einschätzung, das Ergebnis nicht. **Ich führe das als Pech, nicht als Denkfehler — aber ich schreibe beides hin, damit der Unterschied nachprüfbar bleibt.***

---

## Korrekturen und geschlossene Lücken

**Fünf Punkte, davon zwei seit Tagen offene Lücken.**

1. **Terriers Diagnose ist belegt — Lücke seit 15.10. geschlossen.** **Martin Terrier fällt mit einer Oberschenkelverletzung aus**, zugezogen bei der frühen Auswechslung in Posen. *Am 15.10. stand dort: „Terriers Diagnose und Ausfalldauer sind unbekannt." **Die Dauer ist weiterhin unbekannt, die Art der Verletzung nicht mehr.***
2. **Es gibt erstmals eine belastbare Paderborner Ausfallliste — Lücke seit fünf Tagen geschlossen.** **Vor dem Werder-Spiel fehlten Timur Gayret, Nyamekye Awortwie-Grant und Sebastian Klaas; bei Awortwie-Grant zeichnet sich laut Kettemann ein baldiges Comeback ab. Mika Baur fehlt ebenfalls, Filip Bilbija ist zu Derby County gewechselt.** *Damit ist die undatierte `ligainsider.de`-Fundstelle vom 15.10. (Hoffmeier, Klaas, Gayret, Awortwie-Grant im Aufbautraining) in drei von vier Namen bestätigt — **zu Hoffmeier finde ich weiter keinen datierten Beleg.***
3. **Skhiris Ausfalldauer ist jetzt benannt.** *Am 15.10. führte ich ihn nur als „Ausfall".* **Jetzt: Sprunggelenksverletzung aus dem Derby vom 11.10., nach Wagners Worten in diesem Kalenderjahr kein Thema mehr, Hoffnung auf Anfang 2027** — **ohne verbindliche Prognose.**
4. **Dallingas Verletzungsart und -ursache sind belegt:** **Kreuzbandriss im Testspiel gegen Viktoria Köln am 03.10., Ausfall über Monate.** *Das war bisher nur ein Name auf der Liste.*
5. **Die Nwaneri-Rote-Karte ist keine.** *Sie taucht in Suchtiteln als „Rot nach 18 Sekunden" auf und wäre, genommen wie geschrieben, eine Sperre für Partie 7.* **Sie wurde sofort zurückgenommen (falsche Karte aus der Hosentasche), Nwaneri bekam Gelb und spielte weiter.** ***Ich hebe das hervor, weil es der Fundstellentyp ist, der am leichtesten zu einem falschen Tipp führt: korrekte Schlagzeile, gegenteiliger Inhalt.***

---

## Tabelle nach dem 6. Spieltag (sieben von neun Partien)

**Die Tabelle ist selbst gerechnet: Stand nach dem 5. Spieltag plus die sieben Ergebnisse von Freitag und Samstag.** ***Der Grund, warum ich rechne statt abzulesen:*** **alle vier heute geprüften Tabellenquellen zeigten Momentaufnahmen aus dem laufenden Spieltag** — `reviersport.de` führte Dortmund korrekt mit 14 Punkten, die meisten anderen Mannschaften aber noch bei fünf Spielen; `sport.de` und `sportschau.de` zeigten Freiburg und Dortmund mit je 13 vor dem Samstag; eine `kicker.de`-Tabelle war rund 112 Tage alt und zeigte drei Spiele. **Gegenbestätigt ist meine Rechnung an zwei Punkten: `reviersport.de` nennt Dortmund mit 14 Punkten nach sechs Spielen, und `fussballnationalmannschaft.net` schreibt, Bayern übernehme „zumindest bis Sonntag" die Spitze.**

**Vier Vereine haben erst fünf Spiele** (in der Spalte „Sp" sichtbar): **Freiburg und Leverkusen spielen Sonntag 15:30 gegeneinander, Gladbach und Hoffenheim Sonntag 17:30.** **Form = 1. bis 6. Spieltag von links nach rechts.**

| # | Verein | Sp | S | U | N | Tore | Diff | Pkt | Form | Europapokal in der Woche vor dem 7. ST |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | FC Bayern München | 6 | 4 | 2 | 0 | 22:5 | +17 | 14 | S U S S U S | **Mi, CL, heim (Arsenal)** |
| 2 | Borussia Dortmund | 6 | 4 | 2 | 0 | 11:4 | +7 | 14 | S S S S U U | **Di, CL, auswärts (Sabah)** |
| 3 | SC Freiburg | 5 | 4 | 1 | 0 | 14:4 | +10 | 13 | S S S U S – | **Do, Conference League** |
| 4 | Bayer 04 Leverkusen | 5 | 3 | 1 | 1 | 14:8 | +6 | 10 | N S U S S – | **Do, Europa League** |
| 5 | 1. FSV Mainz 05 | 6 | 3 | 1 | 2 | 14:10 | +4 | 10 | U S N S N S | — |
| 6 | SV 07 Elversberg | 6 | 3 | 1 | 2 | 12:11 | +1 | 10 | S S N U N S | — |
| 7 | RB Leipzig | 6 | 3 | 0 | 3 | 16:11 | +5 | 9 | S N S N S N | **Mi, CL, auswärts (Real Madrid)** |
| 8 | SV Werder Bremen | 6 | 2 | 3 | 1 | 12:12 | 0 | 9 | N S U S U U | — |
| 9 | Hamburger SV | 6 | 3 | 0 | 3 | 6:15 | −9 | 9 | N N N S S S | — |
| 10 | FC Augsburg | 6 | 2 | 2 | 2 | 16:12 | +4 | 8 | S S U N U N | — |
| 11 | Eintracht Frankfurt | 6 | 2 | 2 | 2 | 10:16 | −6 | 8 | U N S U N S | — |
| 12 | 1. FC Köln | 6 | 2 | 1 | 3 | 8:11 | −3 | 7 | S N U N S N | — |
| 13 | VfB Stuttgart | 6 | 2 | 0 | 4 | 8:10 | −2 | 6 | N S N N S N | **Di, CL, heim (Atlético)** |
| 14 | FC Schalke 04 | 6 | 1 | 2 | 3 | 5:7 | −2 | 5 | N U S U N N | — |
| 15 | SC Paderborn 07 | 6 | 1 | 2 | 3 | 5:9 | −4 | 5 | U N N S N U | — |
| 16 | 1. FC Union Berlin | 6 | 1 | 2 | 3 | 5:17 | −12 | 5 | U N N N S U | — |
| 17 | TSG Hoffenheim | 5 | 1 | 0 | 4 | 9:13 | −4 | 3 | N N S N N – | **Do, Europa League** |
| 18 | Bor. Mönchengladbach | 5 | 0 | 0 | 5 | 7:18 | −11 | 0 | N N N N N – | — |

**Was die Tabelle für den 7. Spieltag bedeutet:** **Bayern und Dortmund führen punktgleich, aber mit 22:5 gegen 11:4 ganz unterschiedlich zustande gekommen.** **Der HSV ist mit 6:15 Toren Neunter — drei Siege in Folge bei weiter schwacher Offensive.** **Schalke hat mit 5 Toren die schwächste Offensive der Liga, Union mit 17 Gegentoren die schwächste Abwehr.** **Gladbach ist nach fünf Spielen punktlos.**

---

## Heute geprüft und verworfen

1. **Eine `weltfussball.de`-Spielplanzeile „Dortmund – Stuttgart, Samstag 24.10., 15:30".** **Verworfen:** *sie passt zu keiner anderen Quelle; Dortmund spielt gegen Frankfurt (Sa 18:30), Stuttgart gegen Gladbach (Fr 20:30). **Beide Partien sind mehrfach und unabhängig belegt, darunter im DFB-Datencenter.***
2. **Eine `anstosszeiten.de`-Angabe „Hoffenheim – Leverkusen, Freitag 23.10., 15:30".** **Verworfen:** *eine Freitagspartie um 15:30 gibt es im Bundesligaraster nicht; der Schalke-Spielplan, das TSG-Ticketcenter und `sportschau.de` nennen einheitlich Sonntag, 25.10., 15:30, SNP Arena. **Die Seite ist laut Suchergebnis rund 96 Tage alt und führt den Spieltag noch als offenes Wochenendfenster.***
3. **`fussballnationalmannschaft.net` mit „Stuttgart – Gladbach am 24.10., 15:30" und „Freiburg – Bayern am 24.10., 15:30".** **Verworfen:** *beide widersprechen dem DFB-Datencenter, dem offiziellen VfB-Spielplan, der Deutschen Bahn (Sonderverkehr zum Freitagsspiel, 20:30), `hessenschau.de`, `sportschau.de` und `fussballdaten.de`. **Dieselbe Quelle ist bei den Ergebnissen des 6. Spieltags zuverlässig gewesen — bei Ansetzungen ist sie es nicht.***
4. **Eine `sofascore.com`-Angabe „16:30 UTC" für Freiburg – Bayern** (entspräche 18:30) **und „10:00 UTC am 24.10." für Hoffenheim – Leverkusen.** **Verworfen:** *die Mehrheit nennt 17:30 bzw. 15:30 Ortszeit. **Bei Hoffenheim – Leverkusen passt `bundesliga.com` mit „14:30 UTC" genau zu 15:30 MEZ — die Zeitumstellung in der Nacht zuvor erklärt, warum hier mehrere Quellen durcheinandergeraten.***
5. **Eine `goal.com`-Angabe „14:30" und eine ESPN-Angabe „12:30 PM" zu Stuttgart – Gladbach bzw. Dortmund – Frankfurt.** **Nicht als Widerspruch gewertet:** *es sind Zeitzonenumrechnungen (US-Zeit), die zu 20:30 bzw. 18:30 deutscher Zeit passen.*
6. **Eine `weltfussball.de`-Zeile „Hoffenheim gegen Ararat-Armenia am 15.10., 21:00".** **Nicht verwendet:** *sie widerspricht dem am 15.10. aus sechs Quellen belegten 2:3 gegen Beşiktaş mit vollständiger Torfolge. **Ich führe die Abweichung, ohne meinen Stand zu ändern.***
7. **Ein `sport1.de`-Bericht „HSV-Offensivsorgen: Polzin sucht neue Lösungen", der dem HSV „erst zwei Saisontore" zuschreibt und als nächstes Bundesligaspiel „bei der TSG Hoffenheim" nennt.** ***Nur teilweise verwendet:*** **die Verletztenangaben (Daka, Grönbaek, Remberg) übernehme ich, die Einordnung nicht** — *der HSV steht bei 6 Toren, und das Hoffenheim-Spiel liegt hinter ihm (Bernardos Rote Karte fiel dort). **Der Artikel ist älter, als die Trefferliste suggeriert.***
8. **Ein `sportschau.de`-Bericht vom 11.05.2026, nach dem Marie-Louise Eta mit Union in Mainz 3:1 gewann.** **Nicht als Trainerstand verwendet:** *er betrifft die Vorsaison. **Mauro Lustrinelli ist für 2026/27 belegt** (`sportschau.de`/rbb: „Union Berlins neuer Coach: Lustrinelli operiert am offenen Herzen"), **Vorgänger laut Kaderportal Steffen Baumgart.*** *Zwei `fotmob.com`-Seiten führen weiter Baumgart — veraltet.*
9. **`fotmob.com`-Kaderseiten zu Paderborn und Union sowie eine `whoscored.com`-Vorschau Mainz – Union.** **Verworfen:** *undatiert bzw. aus der Saison 2025/26.*
10. **Eine Union-Verletztenliste mit Rönnow, Nsoki, Skov, Markgraf und Skarke.** ***Nicht als aktueller Stand verwendet:*** **Rönnow hat am Samstag gegen Dortmund gespielt und gegen Nwaneri gehalten.** *Die Liste stammt aus der Saisonvorbereitung. **Das ist derselbe Fallentyp wie an den Vortagen, diesmal bei einer Verletztenübersicht.***
11. **Eine `comunio.de`- und eine Yahoo-Prognoseelf zu Leverkusen – Freiburg, die sich in der Offensive widersprechen** (Höler gegen Grifo). **Als Prognose geführt, nicht als Beleg** — *und für den 7. Spieltag ohnehin ohne Wert.*

---

## Offen benannte Restlücken

**Der 7. Spieltag beginnt in sechs Tagen. Vieles davon kann heute noch nicht vorliegen — ich trenne deshalb, was fehlt, von dem, was fehlen *muss*.**

***Strukturell noch nicht verfügbar (kein Mangel meiner Recherche):***
- **Keine Spieltags-Pressekonferenz zu einer der neun Partien** — die finden Donnerstag und Freitag der kommenden Woche statt.
- **Keine Aufstellung, kein Kaderaufgebot, keine voraussichtliche Elf zum 7. Spieltag.**
- **Keine Sperren aus dem 7.-Spieltags-Vorfeld** und keine Gelbsperren-Übersicht, die den Stand nach dem 6. Spieltag abbildet.

***Echte Lücken:***
- **Die Europapokalgegner vom 22.10. für Leverkusen, Hoffenheim und Freiburg sind nicht aufgelöst.** *Der Termin ist belegt, die Paarung nicht. **Damit weiß ich nicht, ob diese drei am Donnerstag auswärts oder zu Hause spielen und wie weit sie reisen** — für drei Partien des Spieltags ein relevanter Rest.*
- **Zwei Partien des 6. Spieltags sind noch nicht gespielt.** *Leverkusen – Freiburg und Gladbach – Hoffenheim am Sonntag. **Diese vier Vereine gehen mit einem Spiel weniger in meine Tabelle ein, und vier meiner neun Tipps (1, 8, 9) stehen auf einer Form, die sich morgen noch ändert.*** **Das ist die größte Unsicherheit dieses Laufs.**
- **Neuers Status bleibt offen.** *Belegt ist nur, dass Urbig gegen Leipzig im Tor stand und Neuer zwei Pflichtspiele nicht gespielt hat. **Keine Diagnose, keine Vereinsmeldung, kein Rückkehrdatum.***
- **Musialas Rückkehr bleibt offen** (Muskelfaserriss, kein Datum).
- **Rondics, van den Bergs und Aches Rückkehrdaten** sind unbekannt bzw. nur als Monatsangabe („November") belegt; **Joël Schmieds Ausfall ist erst angedroht, nicht bestätigt.**
- **Karetsas' Ausfalldauer bei Union ist unbekannt.** *Belegt ist das Umknicken und die Auswechslung gegen Dortmund sowie Ole Books Einschätzung, eine schnelle Rückkehr sei „schwer vorstellbar" — **keine Diagnose.***
- **Zu Mainz und Union finde ich für Oktober 2026 fast nichts.** *Zwei Suchen liefen praktisch ins Leere und gaben nur Material aus der Saison 2025/26 zurück. **Mainz' Heimschwäche und Auswärtsstärke führe ich deshalb unverändert nach dem Stand vom 15.10., nicht nach einem heutigen Beleg** — das ist eine gealterte Grundlage für Partie 5.*
- **Kohrs Ausfalldauer bei Mainz bleibt strittig** (Ende Oktober gegen Anfang Januar 2027).
- **Nicolas Kühns Rückkehr bei Gladbach ist offen**, Honorats, Itakuras, Castrops und Leopolds Status ist je nach Quelle „nicht dabei" oder „angeschlagen" — **keine einheitliche Liste.**
- **Keine Transfermeldung mit Spielrelevanz für den 7. Spieltag.** *Bilbijas Wechsel zu Derby County ist belegt, aber abgeschlossen; Kölns Stürmersuche ist ausdrücklich auf Januar verschoben.*
- **Direkte Vergleiche der letzten Duelle habe ich zu keiner der neun Partien belastbar erhoben.** *Die Suchtreffer dazu waren durchweg aus früheren Saisons oder undatiert. **Meine Tipps stehen daher auf Tabelle, Form, Personal und Belastung — nicht auf Historie.*** **Das war an den Vortagen ebenso und ich schreibe es erneut hin.**

---

## Die Tipps zum 7. Spieltag

**Für alle neun Partien gilt: „neuer Spieltag — kein Vergleich möglich."** *Der Vortagsstand betraf den 6. Spieltag, der inzwischen läuft.*

**Vier Regeln, nach denen ich diesen Spieltag angelegt habe** (die ersten beiden sind die Lehren aus der Abrechnung oben):

1. **Eine Torflaute wiegt schwerer als ein guter Tabellenplatz** — das ist die Lehre aus Union – Dortmund.
2. **Ausfälle beim Gegner senken dessen Tore, sie erhöhen nicht automatisch meine** — die Lehre aus Frankfurt – Köln.
3. **Drei Tage nach einem weiten Auswärtsspiel in Europa gebe ich einen halben Tor-Abschlag**, bei einem Heimspiel in Europa keinen.
4. **Die beiden Aufsteiger (Elversberg, Paderborn) tippe ich nach Spielweise, nicht nach Tabellenplatz.**

**Für jede Partie nenne ich außerdem eine Schwelle: die konkrete Information, die den Tipp bis zum Anpfiff ändern würde.** *Das ist dieselbe Mechanik wie in den Vorläufen — sie hat am 15.10. zwei Änderungen ausgelöst.*

---

### 1. VfB Stuttgart – Borussia Mönchengladbach
**Freitag, 23.10.2026, 20:30 Uhr, MHPArena**
**Tipp: 2:0**
***neuer Spieltag — kein Vergleich möglich***

**Gladbach ist nach fünf Spielen punktlos Letzter (7:18) und reist mit der schlechtesten Personallage der Liga an: Kleindienst fehlt mit erneutem Muskelfaserriss, Leszczyński mit Kniestauchung, dazu Fleck, Honorat, Itakura, Castrop und Leopold nicht dabei oder angeschlagen; Kühns Rückkehr nach Muskelbündelriss ist offen.** **Mit Kleindienst und Honorat fehlen die beiden Spieler, über die Gladbachs Offensive bisher lief.** **Stuttgart hat zwar in Hamburg 0:1 verloren, dabei aber die besseren Chancen gehabt** (Undav an den Pfosten, zwei weitere Gelegenheiten an Heuer Fernandes) **und steht zu Hause vor der Aufgabe, die seine schwache Ausbeute von 8 Toren in 6 Spielen am ehesten erklärt bekommt.**

***Der Gegenpunkt, den ich nicht unterschlage:*** **Stuttgart spielt Dienstag 21:00 gegen Atlético Madrid und hat damit die kürzeste Pause des Spieltags — drei Tage.** *Nach Regel 3 gibt es dafür keinen Abschlag, weil es ein Heimspiel ist; ich halte den Tipp aber bewusst bei zwei Toren statt drei.* **Kein Zu-Null-Automatismus wäre mir lieber, aber Gladbachs Offensive ist in dieser Besetzung die schwächste Begründung für ein Gegentor, die dieser Spieltag hergibt.**

***Schwelle:*** *Wird Kleindiensts **oder** Kühns Einsatz belegt (Kaderaufgebot oder Startelf, **nicht** Prognose), gehe ich auf **2:1**. Kündigt Hoeneß nach dem Atlético-Spiel belegt eine Rotation an **oder** wird ein Stuttgarter Innenverteidiger-Ausfall gemeldet, gehe ich auf **1:1**. **Gladbachs Sonntagsergebnis gegen Hoffenheim allein löst nichts aus — ein erster Punkt würde die Lage nicht personell ändern.***

---

### 2. FC Augsburg – 1. FC Union Berlin
**Samstag, 24.10.2026, 15:30 Uhr, WWK Arena**
**Tipp: 2:1**
***neuer Spieltag — kein Vergleich möglich***

**Augsburg ist zu Hause und hat mit 16 Toren in 6 Spielen die vierbeste Offensive der Liga, kassiert aber auch zuverlässig** — das 3:4 in Elversberg, bei dem Augsburg nach 28 Minuten 0:3 zurücklag und über zwei Elfmeter und Kömürs späten Treffer noch auf 3:4 herankam, **ist die Partie dieses Spieltags mit der klarsten Aussage: diese Mannschaft trifft und wird getroffen.** **Union hat mit 5 Toren in 6 Spielen die zweitschwächste Offensive und mit 17 Gegentoren die schwächste Abwehr der Liga** — **hat aber am Samstag gegen Dortmund 0:0 gespielt und dabei zu null gestanden.** **Dazu hat sich Konstantinos Karetsas dort den Fuß umgeknickt und musste verletzt vom Feld; Sportdirektor Ole Book hält eine schnelle Rückkehr für „schwer vorstellbar".**

**Bei Augsburg fehlen nach dem Stand vom 15.10. Noahkai Banks (Außenbandverletzung im Knie, „zwei, drei, vier Wochen mindestens") und Alexis Claude-Maurice (Muskelverletzung), Marius Wolf ist fit.** **Keine der beiden Mannschaften spielt international** — *die einzige Partie des Spieltags, bei der das für beide Seiten gilt und bei der ich deshalb ohne Belastungsannahme rechne.*

***Schwelle:*** *Wird ein weiterer Augsburger Offensivausfall mit genannter Ersatzlösung gemeldet, gehe ich auf **1:1**. Wird Unions Null-zu-null-Formation gegen Dortmund in einem Vorbericht als Linie für Augsburg bestätigt (Kovač-artiger Tiefbau, fünf Verteidiger), gehe ich auf **1:0**. Wird Karetsas' Ausfall als langfristig bestätigt, bleibe ich bei 2:1 — **er ist in meinem Tipp bereits als Ausfall gerechnet.***

---

### 3. 1. FC Köln – FC Schalke 04
**Samstag, 24.10.2026, 15:30 Uhr, RheinEnergieSTADION**
**Tipp: 1:0**
***neuer Spieltag — kein Vergleich möglich***

***Das ist die Partie mit den beiden kaputtesten Offensiven des Spieltags, und ich tippe sie entsprechend tief.*** **Köln hat keinen gesunden Mittelstürmer: Dallinga (Kreuzbandriss, Monate), Ache (Muskelverletzung, Rückkehr im November erwartet), Rondic (Oberschenkel, ohne Datum) fallen aus, dazu Skhiri im Mittelfeld bis mindestens Jahresende, van den Berg und der langzeitverletzte Hübers, und Joël Schmied droht auszufallen.** **Der Verein hat ausdrücklich keinen Ersatz verpflichtet und verschiebt das auf Januar; vorn sollen Luca Waldschmidt — gerade aus einer Verletzung zurück — und Marius Bülter spielen.** **Köln hat am Freitag in Frankfurt nicht getroffen.**

**Schalke steht dem in nichts nach: 5 Tore in 6 Spielen sind die schwächste Offensive der Liga, und im dritten Heimspiel nach dem Wiederaufstieg ist die Mannschaft erneut ohne eigenen Treffer geblieben** (0:1 gegen Mainz). **Moussa Sylla, nach dem Stand vom 15.10. erste Wahl vor Džeko, fehlt mit einer Beinverletzung ohne genannte Diagnose und Dauer.** **Loris Karius war gegen Mainz Spieler des Spiels und hat laut `reviersport.de` Schlimmeres verhindert** — *das ist das Muster: Schalke hält lange, trifft aber nicht.*

**Ich gebe Köln den Heimvorteil und damit das eine Tor, weil Waldschmidt belegt zurück ist und Schalke auswärts noch weniger Zugriff auf Tore hat als zu Hause.** ***Regel 2 angewandt: Ich widerstehe der Versuchung, Schalkes Sturmproblem in zwei oder drei Kölner Tore umzurechnen — genau dieser Fehler hat mich am 15.10. bei Frankfurt – Köln zwei Tore gekostet.***

***Schwelle:*** *Wird Aches **oder** Rondics Rückkehr für diesen Spieltag belegt (Kaderaufgebot, nicht Prognose), gehe ich auf **2:0**. Wird Syllas Rückkehr belegt **oder** fällt ein weiterer Kölner Innenverteidiger aus, gehe ich auf **1:1**. **Bleibt es bei beiden Ausfalllisten, bleibt es bei 1:0.***

---

### 4. RB Leipzig – SV 07 Elversberg
**Samstag, 24.10.2026, 15:30 Uhr, Red Bull Arena**
**Tipp: 2:1**
***neuer Spieltag — kein Vergleich möglich***

***Das ist der Tipp, bei dem ich am 15.10. am deutlichsten danebenlag — damals in der Gegenrichtung —, und ich behandle Elversberg heute entsprechend.*** **Elversberg hat Augsburg 4:3 geschlagen und nach 28 Minuten 3:0 geführt (Petkov, Günther, Rohr); Noel Futkeu setzte in der Nachspielzeit sogar noch einen Elfmeter an die Latte.** **Der Aufsteiger steht mit 10 Punkten vor Augsburg und über Leipzig, hat drei Siege aus sechs Spielen und spielt nicht international.** **Nach dem Stand vom 15.10. fehlen Onyeka (ohne Rückkehrdatum), Seifert (länger) und Zimmerschied (einige Wochen); Gyamerah ist einsatzbereit.**

**Leipzig steht dagegen am schlechtesten Punkt der Saison.** **Das 1:6 in München war die zweite Niederlage in drei Spielen, Demichelis steht „mehr denn je in der Kritik", Matthäus kritisiert öffentlich die Aufstellung (Klostermann) und das Ausbleiben einer Halbzeitkorrektur, Sportchef Schäfer war verärgert.** ***Und die Belastung ist die zweitschwerste des Spieltags: Mittwoch 21:00 im Bernabéu, dann Samstag 15:30 zu Hause — drei Tage nach einem weiten Auswärtsspiel.*** **Nach Regel 3 gibt es dafür einen Abschlag.**

**Ich tippe trotzdem Leipzig, aber knapp.** **Begründung: 16 Tore in 6 Spielen sind die zweitbeste Offensive der Liga, und eine Mannschaft unter diesem Druck spielt zu Hause gegen einen Aufsteiger in der Regel das Spiel, in dem sie antworten will.** ***Dies ist der unsicherste meiner neun Tipps*** — *die Kombination aus Madrid-Reise, Trainerdebatte und einem formstarken Aufsteiger ist genau die Lage, in der Heimsiege ausbleiben.*

***Schwelle:*** *Wird Demichelis vor dem Spieltag entlassen oder freigestellt, gehe ich auf **1:1** (ein Trainerwechsel in der Woche vor dem Spiel ist in beide Richtungen offen, aber nie stabilisierend). Kündigt Demichelis nach Madrid belegt eine Rotation an **oder** fällt ein Leipziger Offensivspieler mit genannter Ersatzlösung aus, gehe ich ebenfalls auf **1:1**. Wird ein Elversberger Ausfall in der Innenverteidigung gemeldet, gehe ich auf **3:1**.*

---

### 5. 1. FSV Mainz 05 – SV Werder Bremen
**Samstag, 24.10.2026, 15:30 Uhr, Mewa Arena**
**Tipp: 1:1**
***neuer Spieltag — kein Vergleich möglich***

**Mainz hat am Samstag in Gelsenkirchen 1:0 gewonnen — Tietz in der 24. nach Vorlage von Caci, sein fünftes Ligator — und steht mit 10 Punkten auf Platz 5.** ***Der Grund, warum ich hier trotzdem kein Heimspiel-Plus vergebe, ist ein Muster, das ich am 15.10. aus den Pressekonferenzberichten übernommen habe: Mainz ist auswärts ungeschlagen und zu Hause sieglos.*** **Urs Fischer hatte zudem zehn Gegentore in drei Bundesligaspielen beklagt und fehlende Kompaktheit als Problem benannt — die Null in Schalke ist die erste Gegenbewegung dazu.** *Kohrs Ausfalldauer bleibt strittig.*

**Werder ist die Mannschaft des Spieltags, die man nicht abschreiben kann.** **Gegen Paderborn lag Werder 0:2 zurück und holte durch Füllkrugs Doppelpack (59., 65. per Elfmeter) noch einen Punkt — als erste Bundesligamannschaft, die das dreimal in Folge geschafft hat; sechs Punkte nach Rückstand sind Ligabestwert.** **Thioune war dennoch unzufrieden („anhand der Torchancen müsse Werder das Spiel gewinnen") und brachte Mitchell Weiser zur Pause, der das Spiel strukturierte** — *am 15.10. galt Weiser noch als „wohl kein Startelf-Kandidat"; das hat sich in 48 Stunden geändert.* **Amos Pieper war schon für die Startelf zurück. Werder spielt nicht international.**

***Ehrlichkeitsvermerk, der zu diesem Tipp gehört:*** **Meine Grundlage für Mainz' Heimschwäche ist zwei Tage alt und stammt aus PK-Berichten, nicht aus einem heutigen Beleg** — *zwei Suchen zu Mainz im Oktober 2026 liefen heute praktisch ins Leere und gaben nur Material der Vorsaison zurück.* **Von allen neun Partien ist diese die mit der am stärksten gealterten Faktenlage.**

***Schwelle:*** *Wird Mainz' erster Heimsieg der Saison vor diesem Spieltag erzielt — den gibt es bis hierher nicht, also nur hypothetisch — oder wird in einem Vorbericht die Heimschwäche ausdrücklich als überwunden beschrieben, gehe ich auf **2:1**. Fällt Füllkrug aus (Meldung, nicht Vermutung), gehe ich auf **2:0**. Wird Kohrs Rückkehr belegt, gehe ich auf **2:1**.*

---

### 6. SC Paderborn 07 – Hamburger SV
**Samstag, 24.10.2026, 15:30 Uhr, Home Deluxe Arena**
**Tipp: 1:1**
***neuer Spieltag — kein Vergleich möglich***

***Hier wende ich Regel 4 ausdrücklich an.*** **Paderborn steht mit 5 Punkten auf Platz 15, hat aber bei Werder 2:0 geführt (Marino 18., Tigges 30.) und stand in der Nachspielzeit durch Rayan Philippe aus wenigen Metern am Pfosten vor dem Auswärtssieg.** **Torwart Nahuel Noll hielt mehrfach stark.** **Kettemann beschreibt seine Mannschaft als „Gruppe junger, unerfahrener Bundesliga-Menschen", der es vor allem an Torgefahr fehlt** — **5 Tore in 6 Spielen bestätigen das**, *aber zwei davon fielen am Samstag auswärts in Bremen.* **Es fehlen Gayret, Klaas und Baur; bei Awortwie-Grant zeichnet sich ein baldiges Comeback ab. Bilbija ist zu Derby County gewechselt.**

**Der HSV kommt mit drei Siegen in Folge, zuletzt 1:0 gegen Stuttgart durch Muheims Schuss aus 25 Metern in der 88. Minute vor 57.000 Zuschauern.** ***Aber die Zahlen hinter der Serie sind dünn: 6 Tore in 6 Spielen, 15 Gegentore, Torverhältnis −9 bei 9 Punkten.*** **Der HSV gewinnt enge Spiele spät, er dominiert sie nicht.** **Dazu fehlen Patson Daka und Albert Grönbaek, und Remberg hat einen Kreuzbandriss — seine Saison ist womöglich beendet.** **Polzin sucht laut `sport1.de` „neue Lösungen" für die Offensive.** **Keine der beiden Mannschaften spielt international.**

**Ein Remis ist hier nicht der bequeme Mittelweg, sondern das Ergebnis beider Befunde: eine Heimmannschaft, die gerade gezeigt hat, dass sie führen kann, gegen eine Auswärtsmannschaft, die mit 6 Saisontoren drei Spiele hintereinander gewonnen hat.**

***Schwelle:*** *Wird ein vierter HSV-Sieg in Folge durch eine belegte Offensivverstärkung plausibler (Daka oder Grönbaek im Kaderaufgebot), gehe ich auf **1:2**. Fällt bei Paderborn Tigges **oder** Marino aus, gehe ich ebenfalls auf **1:2**. Wird Awortwie-Grants Rückkehr belegt, gehe ich auf **2:1**.*

---

### 7. Borussia Dortmund – Eintracht Frankfurt
**Samstag, 24.10.2026, 18:30 Uhr, Signal Iduna Park**
**Tipp: 2:0**
***neuer Spieltag — kein Vergleich möglich***

***Dies ist die Partie, in die ich die Lehre aus dem 6. Spieltag am direktesten einbaue — und zwar in beide Richtungen.*** **Dortmund ist drei Pflichtspiele ohne eigenes Tor** (Remis gegen Werder, 0:1 in Bodø, 0:0 bei Union), **steht aber mit 14 Punkten und 4 Gegentoren in 6 Spielen an der Tabellenspitze.** **Kovač steht unter Fandruck („Kovac out"), Petersen kritisiert die späten Wechsel, und gegen Union kamen 12 Torschüsse ohne Tor zustande.** **Nwaneri ist nach der zurückgenommenen Roten Karte spielberechtigt; Schlotterbeck und Anton waren in Berlin die Herausragenden.** **Belastung: Dienstag 18:45 auswärts bei Sabah in Aserbaidschan — die weiteste Reise des Spieltags, aber mit vier Tagen Abstand und einem Gegner, gegen den rotiert werden kann.**

**Frankfurt ist der Gegner, gegen den eine Torflaute am ehesten endet: 16 Gegentore in 6 Spielen sind die zweitschwächste Abwehr der Liga, und vor einer Woche gab es ein 0:6 in Leipzig.** **Der 1:0-Sieg gegen Köln war Frankfurts erster Heimsieg in der Liga seit März — auswärts steht die Mannschaft also weiter ohne Ausweis.** **Ebnoutalib (77., Vorlage Aséko) wurde mit 60 Prozent der Stimmen Spieler des Spiels.**

**Ich tippe 2:0 und nicht höher, weil Regel 1 und Regel 2 hier gegeneinander arbeiten:** **Dortmunds Flaute ist real und drei Spiele lang, Frankfurts Abwehrschwäche ebenfalls.** ***Die Auflösung, für die ich mich entscheide: Dortmund trifft wieder, aber nicht in Serie.*** *Ein 0:0 wäre die Fortsetzung der Flaute und ist das Ergebnis, das mich hier am ehesten widerlegt.*

***Schwelle:*** *Bleibt Dortmund auch in Aserbaidschan ohne Tor (also vier Spiele), gehe ich auf **1:0**. Wird ein Dortmunder Innenverteidiger-Ausfall mit genannter Ersatzlösung gemeldet **oder** fällt Guirassy aus, gehe ich auf **1:1**. Wird Kovač vor dem Spieltag entlassen, gehe ich auf **1:1**. Wird bei Frankfurt ein weiterer Innenverteidiger-Ausfall gemeldet, gehe ich auf **3:0**.*

---

### 8. TSG Hoffenheim – Bayer 04 Leverkusen
**Sonntag, 25.10.2026, 15:30 Uhr (MEZ), SNP Arena**
**Tipp: 1:2**
***neuer Spieltag — kein Vergleich möglich***

**Hoffenheim ist Siebzehnter mit 3 Punkten aus fünf Spielen und hat nach Ilzers eigener Bilanz sechs Niederlagen aus acht Spielen; die 2:3-Niederlage gegen Beşiktaş war die vierte Pflichtspielniederlage in Folge, und Kapitän Baumann sagte, man habe „zu wenig Punkte für die Leistung" geholt.** **Bernardo hat gegen den HSV Rot gesehen und fehlt am Sonntag gegen Gladbach; für den 7. Spieltag ist er bei einem Spiel Sperre wieder spielberechtigt — das kann ich aber nicht belegen, weil mir die Länge der Sperre nicht vorliegt.** **Albian Hajdari ist verletzt.**

**Leverkusen ist Vierter mit 10 Punkten aus fünf Spielen und hat in Posen 4:0 gewonnen.** **Patrik Schick ist in Form (zwei Elfmetertreffer in Posen), Ibrahim Maza hat dort getroffen.** **Die Ausfallliste ist aber lang und seit gestern genauer: Martin Terrier fehlt mit Oberschenkelverletzung, dazu Ben Seghir, Doué, Eichhorn und Kofane.**

***Belastung: beide spielen Donnerstag in der Europa League, und beide haben drei Tage Pause.*** **Das ist die einzige Partie des Spieltags, in der sich die europäische Belastung exakt aufhebt** — *allerdings kenne ich bei keinem der beiden den Gegner und damit auch nicht die Reiseweite; das ist eine benannte Lücke.* **Bleibt der Qualitäts- und Formunterschied, und der ist deutlich.**

***Schwelle:*** *Wird Leverkusens Europapokalgegner als weite Auswärtsreise bekannt (außerhalb Mitteleuropas) **und** Hoffenheims als Heimspiel, gehe ich auf **1:1**. Wird Schicks Ausfall oder Schonung belegt, gehe ich ebenfalls auf **1:1**. Holt Hoffenheim am Sonntag gegen Gladbach einen Sieg, gehe ich auf **2:2** — **ein erster Dreier gegen den Letzten wäre bei sechs Niederlagen aus acht Spielen der erste belastbare Formumschwung.***

---

### 9. SC Freiburg – FC Bayern München
**Sonntag, 25.10.2026, 17:30 Uhr (MEZ), Europa-Park Stadion**
**Tipp: 1:2**
***neuer Spieltag — kein Vergleich möglich***

**Das Topspiel des Spieltags, und die Partie mit der besten Faktenlage auf beiden Seiten.** **Bayern hat Leipzig 6:1 geschlagen, steht bei 22:5 Toren und ist in sechs Spielen unbesiegt** — **Luis Díaz traf dreifach, dazu Pavlović, Olise und Kane.** **Jonas Urbig stand im Tor; Neuer hat zwei Pflichtspiele nicht gespielt, ohne dass eine Diagnose vorliegt. Musiala fehlt weiter (Muskelfaserriss, kein Datum).** **Belastung: Mittwoch 21:00 zu Hause gegen Arsenal — ein Spitzenspiel, aber im eigenen Stadion und mit vier Tagen Abstand.**

**Freiburg ist nach fünf Spielen unbesiegt (4 Siege, 1 Remis, 14:4) und Schuster hat neun Pflichtspiele in Folge ohne Niederlage.** **Freiburg spielt Donnerstag in der Conference League — drei Tage vor dem Anpfiff, Gegner und Reiseweite unbekannt.** **Yuito Suzukis Gelb-Rot-Sperre betrifft nur die Bundesliga und wird am Sonntag, 18.10., gegen Leverkusen abgesessen — für den 7. Spieltag ist er wieder spielberechtigt.** **Florent Muslija fehlt mit Kreuzbandriss.** *Zu Beste, der am 15.10. als „unbekannt" geführt war, finde ich ihn heute erstmals in einer veröffentlichten Prognoseelf — **das ist eine Prognose und damit nach meiner eigenen Regel kein Beleg**, aber es spricht gegen einen Ausfall.*

**Ich tippe Bayern mit einem Tor Unterschied.** **Begründung: der Qualitäts- und Formunterschied in der Offensive ist in Zahlen eindeutig (22:5 gegen 14:4 bei einem Spiel mehr), Freiburgs Heimstärke und die drei Tage nach dem Donnerstagsspiel sprechen gegen eine klare Angelegenheit.** ***Dieser Tipp hängt an einer Unbekannten, die ich benennen muss: Freiburg spielt am Sonntag, 18.10., gegen Leverkusen, und dieses Ergebnis steht noch aus. Bei einer Niederlage wäre Freiburgs Serie beendet, bei einem Sieg wäre Freiburg Tabellenführer.***

***Schwelle:*** *Verliert Freiburg am Sonntag gegen Leverkusen deutlich (zwei Tore oder mehr), gehe ich auf **1:3**. Gewinnt Freiburg und ist damit Tabellenführer, gehe ich auf **2:2**. Wird Neuers Rückkehr belegt (Vereinsmeldung oder Kaderaufgebot), bleibt es bei 1:2 — **ein Torwartwechsel auf Urbig hat Bayern sechs Spiele nicht geschadet.** Wird Kompanys Rotation nach dem Arsenal-Spiel belegt angekündigt, gehe ich auf **1:1**. Wird Musialas Rückkehr belegt gemeldet (Kaderaufgebot, nicht Prognose), gehe ich auf **1:3**.*

---

## Verteilung und Selbstkontrolle

| Partie | Anstoß | Tipp | Vergleich | Europapokal in der Woche (heim/auswärts, Tage Pause) |
|---|---|---|---|---|
| Stuttgart – Gladbach | **Fr 20:30** | **2:0** | neuer Spieltag | **Di CL heim (3)** / — |
| Augsburg – Union | Sa 15:30 | **2:1** | neuer Spieltag | — / — |
| Köln – Schalke | Sa 15:30 | **1:0** | neuer Spieltag | — / — |
| Leipzig – Elversberg | Sa 15:30 | **2:1** | neuer Spieltag | **Mi CL auswärts Madrid (3)** / — |
| Mainz – Werder | Sa 15:30 | **1:1** | neuer Spieltag | — / — |
| Paderborn – HSV | Sa 15:30 | **1:1** | neuer Spieltag | — / — |
| Dortmund – Frankfurt | **Sa 18:30** | **2:0** | neuer Spieltag | **Di CL auswärts Aserbaidschan (4)** / — |
| Hoffenheim – Leverkusen | **So 15:30** | **1:2** | neuer Spieltag | **Do EL (3)** / **Do EL (3)** |
| Freiburg – Bayern | **So 17:30** | **1:2** | neuer Spieltag | **Do CoL (3)** / **Mi CL heim (4)** |

**Verteilung: vier Heimsiege, zwei Remis, drei Auswärtssiege. 20 Tore in 9 Partien (2,2 pro Spiel).** *Zum Vergleich: der 6. Spieltag hat in sieben Partien 18 Tore gebracht (2,6), mein Tippsatz dafür lag bei 2,4. **Ich liege also etwas unter dem tatsächlichen Schnitt — bewusst, weil vier meiner Partien von Mannschaften mit ausgefallenen Stürmern bestritten werden.***

**Anstoßzeiten:** **Fr 23.10. 20:30 Stuttgart – Gladbach; Sa 24.10. 15:30 Augsburg – Union, Köln – Schalke, Leipzig – Elversberg, Mainz – Werder, Paderborn – HSV; Sa 24.10. 18:30 Dortmund – Frankfurt; So 25.10. 15:30 Hoffenheim – Leverkusen; So 25.10. 17:30 Freiburg – Bayern.** ***Das Raster ist in sich stimmig — ein Freitagsspiel, fünf Partien am Samstag um 15:30, ein Samstagabendspiel, zwei Sonntagsspiele —, und genau diese Stimmigkeit ist mein stärkstes Argument gegen die vier verworfenen Abweichungen oben.*** **Die beiden Sonntagsspiele finden nach der Zeitumstellung statt, also in MEZ.**

***Zur Selbstkontrolle: drei Dinge, bei denen ich diesen Lauf für angreifbar halte.***

1. ***Partie 4 (Leipzig – Elversberg) ist mein unsicherster Tipp.*** **Ich tippe eine Mannschaft, die gerade 1:6 verloren hat, deren Trainer öffentlich in Frage steht und die drei Tage vorher im Bernabéu spielt, gegen einen Aufsteiger, der in der Tabelle über ihr steht.** *Die Begründung (zweitbeste Offensive, Heimspiel, Reaktionserwartung) ist vertretbar, aber dünn. **Es ist derselbe Fehlertyp, der mich bei Elversberg – Augsburg schon einmal erwischt hat, nur mit vertauschten Rollen.***
2. ***Vier Tipps stehen auf Daten, die sich morgen ändern.*** **Freiburg, Leverkusen, Gladbach und Hoffenheim spielen am Sonntag noch ihre Partien des 6. Spieltags.** *Betroffen sind die Partien 1, 8 und 9 — und Partie 9 unmittelbar, weil Freiburg bei einem Sieg Tabellenführer wäre.* **Ich habe das in den Schwellen von Partie 8 und 9 ausdrücklich abgebildet, statt es zu überspielen.**
3. ***Für Mainz und Union habe ich heute keine neuen Belege gefunden.*** **Partie 2 und Partie 5 stehen damit teils auf Material vom 15.10.** *Bei Union hilft mir das 0:0 gegen Dortmund und Karetsas' Verletzung als frischer Befund; **bei Mainz ist die zentrale Annahme (Heimschwäche) zwei Tage alt und stammt aus PK-Berichten.*** **Das ist die schwächste Faktengrundlage der neun.**

***Was ich diesmal nicht getan habe und bewusst nicht:*** **Ich habe keinen Tipp auf direkte Vergleiche gestützt.** *Die Suchergebnisse dazu waren durchweg aus falschen Saisons — derselbe Fallentyp, der an jedem Vortag aufgetreten ist. **Ich halte es für ehrlicher, die Kategorie offen weglassen zu nennen, als sie mit undatierten Zahlen zu füllen.***

---

## Quellen

**Verwendet** (ausschließlich über `WebSearch`-Zusammenfassungen, kein Volltext — siehe Hinweis zur Quellenlage):

**Ansetzungen und Anstoßzeiten:** `datencenter.dfb.de` (Stuttgart – Gladbach Fr 20:30 MHPArena; Köln – Schalke Sa 15:30 RheinEnergieSTADION) · `vfb.de` (Spielplan, Fr 20:30) · `s-bahn-stuttgart.de` (Sonderverkehr zum Freitagsspiel, 20.30 Uhr) · `sportschau.de` (Audiostream-Seiten mit Anstoßzeiten zu Dortmund – Frankfurt, Augsburg – Union, Hoffenheim – Leverkusen, Köln – Schalke) · `bundesliga.com` (Liveticker-Seiten zum 7. Spieltag, Spielorte, UTC-Zeiten) · `tsg-hoffenheim.de` (Ticketcenter: So 25.10., 15:30, SNP Arena) · `hessenschau.de`, `fussballdaten.de` (Freiburg – Bayern So 17:30) · `schalke04.de` (Spielplan 7. Spieltag) · `profis.eintracht.de` (Spielplan) · `anstosszeiten.de` (Paarungen; Zeiten nur, wo durch andere gedeckt)

**Ergebnisse und Berichte zum 6. Spieltag:** `bundesliga.com` (Spielberichte Bayern – Leipzig, HSV – Stuttgart, Union – Dortmund, Elversberg – Augsburg, Werder – Paderborn, Schalke – Mainz, Frankfurt – Köln) · `sportschau.de` (Spielberichte Union – Dortmund, HSV – Stuttgart, Elversberg – Augsburg, Werder – Paderborn) · `t-online.de` (Bayern – Leipzig; Nwaneri-Karte) · `hsv.de` (Muheim-Tor, 25 Meter, 117 km/h) · `werder.de` (Füllkrug-Doppelpack) · `hessenschau.de`, `neunzigplus.de`, `sky.de` (Frankfurt – Köln) · `zdfheute.de` (Elversberg – Augsburg, vier Elfmeter) · `reviersport.de` (Schalke – Mainz, Karius; Tabelle 6. Spieltag) · `laola1.at` · `berliner-kurier.de`, `tagesspiegel.de`, `spox.com`, `footy.de` (Nwaneri-Karte und Rücknahme) · `goal.com` (Einzelkritiken Dortmund: Anton, Schlotterbeck) · `beinsports.com` · `weser-kurier.de` (Thioune-Reaktion) · `fussballnationalmannschaft.net` (Ergebnisübersicht 6. Spieltag)

**Personal und Vorberichte:** `gladbachlive.de` („Muskel-Seuche"), `fussballdaten.de` (Kleindienst-Rückschlag), `fohlen-hautnah.de`, `onefootball.com`, `sportsmole.co.uk` (Gladbach/Hoffenheim-Ausfälle, Bernardo-Sperre, Hajdari) · `koeln.t-online.de`, `geissblog.koeln`, `absolutfussball.com`, `ms-aktuell.de`, `fussball-news.de` (Kölner Ausfälle, Skhiri bis 2027, Dallinga-Kreuzbandriss, Schmied, keine Stürmerverpflichtung) · `sport1.de` (Demichelis-Kritik, Matthäus, Klostermann; HSV-Ausfälle Daka/Grönbaek) · `rblive.de`, `getfootballnewsgermany.com` (Leipziger Stimmen) · `media-sportservice.de` („Kettemann warnt vor Füllkrug", 16.10.), `sportschau.de`/WDR (Paderborns fehlende Torgefahr) · `magazin.comunio.de` (Remberg-Kreuzbandriss) · `fussballtransfers.com`, `sportschau.de`/rbb (Lustrinelli als Unions Trainer) · `tribuna.com`, `livescore.com`, `reviersport.de` (Kovač-Kritik, Torflaute)

**Europapokal:** `de.wikipedia.org` (UEFA Europa League 2026/27: 2. Spieltag 15.10., 3. Spieltag 22.10.) · `kicker.de`-Spielplanzeile (Leverkusen, Do 22.10., 3. Spieltag) · `absolutfussball.com`, `sport.sky.de` (CL-Spielpläne Bayern, Dortmund, Leipzig, Stuttgart: Sabah auswärts Di 18:45, Atlético heim Di 21:00, Arsenal heim Mi 21:00, Real Madrid auswärts Mi 21:00) · `sport1.de`, `t-online.de` (Lostöpfe Hoffenheim und Freiburg) · `zdfheute.de` (Freiburg – Jablonec)

**Verworfen oder nur mit Vorbehalt verwendet** (siehe eigener Abschnitt): `weltfussball.de` (Dortmund – Stuttgart Sa 15:30; Hoffenheim – Ararat-Armenia) · `anstosszeiten.de` (Hoffenheim – Leverkusen Fr 15:30; offene Zeitfenster, ~96 Tage alt) · `fussballnationalmannschaft.net` (Ansetzungen Stuttgart – Gladbach und Freiburg – Bayern am 24.10.) · `sofascore.com` (16:30 UTC Freiburg – Bayern; 10:00 UTC Hoffenheim – Leverkusen) · `fotmob.com` (Baumgart als Unions Trainer; undatierte Kader- und Verletztenseiten) · `goal.com`/ESPN (Zeitzonenangaben) · `kicker.de` (Tabelle mit drei Spielen, ~112 Tage alt) · `sport.de`/`sportschau.de` (Tabellen-Momentaufnahmen mit fünf Spielen) · `sport1.de` („erst zwei Saisontore", „nächstes Spiel bei Hoffenheim") · `whoscored.com` (Vorschau Mainz – Union 2025/26) · `sportschau.de`/rbb (Eta-Sieg in Mainz, 11.05.2026) · Union-Verletztenliste aus der Saisonvorbereitung (Rönnow u. a.) · `comunio.de`/Yahoo (Prognoseelfen Leverkusen – Freiburg)
