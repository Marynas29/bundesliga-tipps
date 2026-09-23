# Bundesliga-Tipps – 5. Spieltag 2026/27 (Stand: 22.09.2026)

**Ansetzung:** Freitag, 09.10. bis Sonntag, 11.10.2026. Der Vortagsstand (21.09.) betraf denselben Spieltag – **alle neun Tipps sind vergleichbar.**

**Zweiter Tag der Länderspielpause (21.09.–06.10.2026).** Bis zum Anpfiff sind es 17 Tage.

**Ein Tipp ändert sich heute, acht bleiben.** Die Änderung betrifft **Köln – Gladbach** und ist eine **Rücknahme der gestrigen Änderung**. Das schreibe ich so deutlich hin, weil ein Tipp, der an zwei Tagen hin- und herspringt, eine Erklärung schuldet: Die gestrige Änderung stützte sich auf eine Annahme, die heute widerlegt ist (siehe dort).

## Hinweis zur Quellenlage (bitte zuerst lesen)

Die vorgesehenen Fachquellen sind aus dieser Umgebung **weiterhin nicht abrufbar** – heute der **sechzehnte Lauf in Folge** mit demselben Befund. `kicker.de`, `bundesliga.com`, `weltfussball.de`, `transfermarkt.de` und `sportschau.de` wurden um 21:12 UTC einzeln per curl geprüft und liefern alle den Rückgabewert `000` (kein Verbindungsaufbau). Die Proxy-Statusabfrage nennt für exakt diese fünf Hosts und exakt diesen Zeitpunkt `connect_rejected / gateway answered 403 to CONNECT (policy denial or upstream failure)`.

**Auch das Fetch-Werkzeug ist heute an allen fünf Versuchen gescheitert** (`EGRESS_BLOCKED`): `datencenter.dfb.de`, `anstosszeiten.de`, `vfb.de`, `ligainsider.de`, `diebewertung.de`.

Besonders ärgerlich sind die ersten beiden: In den Suchtreffern tauchte heute **erstmals das DFB-Datencenter** auf – das wäre die Primärquelle zum Spielplan gewesen, die ich seit zwei Wochen suche. Sie ist blockiert wie alle anderen. Dasselbe gilt für `ligainsider.de`, die einzige gefundene fortlaufende Verletztenliste.

Verfügbar ist damit **ausschließlich die Websuche**, also Suchergebnis-Zusammenfassungen statt Primärseiten. Es handelt sich um eine **Richtlinienentscheidung des Netzwerk-Proxys**, nicht um einen Fehler auf Seiten der Quellen.

### Der Spielplan ist jetzt so gut belegt, wie er ohne Primärseiten werden kann

Zwei Dinge haben sich heute zum Besseren geändert:

- **Zwei Vereinsmitteilungen stützen die Terminierung.** In den Suchtreffern stehen `vfb.de` mit „Bundesliga-Ansetzungen Spieltag fünf bis elf" und `scfreiburg.com` mit „Dates and kick-off times confirmed for matchdays 5 to 11". Beide Seiten sind **nicht abrufbar**, aber es sind Vereinsmeldungen zur Terminierung genau dieses Blocks – damit stehen hinter den Anstoßzeiten erstmals offizielle Absender und nicht nur Aggregatoren.
- **Vier Anstoßzeiten sind heute zusätzlich einzeln bestätigt worden:** Dortmund – Werder Fr 20:30, Augsburg – Bayern Sa 15:30, Köln – Gladbach So 15:30, Freiburg – Schalke So 17:30.

### Zwei Widersprüche aufgetaucht, beide aufgelöst

1. **„VfB Stuttgart – FC Paderborn" war falsch herum.** Eine Suchzusammenfassung zum TV-Plan führte die Partie mit Stuttgarter Heimrecht. **Es bleibt bei Paderborn zu Hause:** Eine kicker-Spielinfo-Seite trägt den Titel „SC Paderborn 07 – VfB Stuttgart, 5. Spieltag", die bundesliga.com-Matchday-URL lautet `.../5/sc-paderborn-07-vs-vfb-stuttgart/...`, und der Spielort ist die Home Deluxe Arena in Paderborn. Drei unabhängige Belege gegen eine schlecht zusammengefasste TV-Tabelle.
2. **„Freiburg – Schalke um 17:00" war ebenfalls falsch.** Eine erste Zusammenfassung behauptete, „die meisten Quellen" nennten 17:00 CEST. Die Nachfrage ergab: **17:30 Uhr, Sonntag, DAZN** – und die Standard-Anstoßzeiten am Sonntag sind in dieser Saison unverändert **15:30 und 17:30**; ein 17:00-Slot existiert im Bundesliga-Raster gar nicht. Mein bisheriger Wert war richtig.

**Was offen bleibt:** Zwei Ticketportale führen **Köln – Gladbach unter dem 10.10.** statt dem 11.10. Dagegen stehen soccerway, fussballdaten (5. Spieltag), zdfheute und – am gewichtigsten – ein Bericht aus dem Köln-Umfeld, wonach für den FC „am 11. Oktober mit dem Derby gegen Gladbach" weitergeht. Ich halte **Sonntag, 11.10., 15:30** für richtig und werte die Ticketdaten als Platzhalter.

## Korrekturen und Klärungen am Vortagsstand

1. **Blessins Vertrag läuft bis 2028, nicht bis 2029.** Gestern hatte ich „Vertrag bis 2029" aus einer Bild-Vorabmeldung übernommen. Heute liegt die **Vereinsbestätigung vom Dienstag** vor: Vertrag **bis Sommer 2028**. Sky, sportschau und bundesliga.com stimmen darin überein. Die 2029 war falsch.
2. **Die Verpflichtung ist offiziell, nicht mehr nur gemeldet.** Gestern stand hier „Meldungslage konkret statt spekulativ, aber keine Vereinsbestätigung". Die liegt jetzt vor. Die **offizielle Vorstellung** mit Sportdirektor Rouven Schröder ist für **Mittwoch, 23.09., 13:30 Uhr im ista-Borussia-Park** angesetzt. **Jan-Moritz Lichte** bleibt auch unter Blessin Assistent. Ablöse an St. Pauli fällt laut Hamburger Morgenpost keine an.
3. **Mein gestriger Satz „erstes Training Dienstag, 9:00 Uhr" ist unbestätigt geblieben.** Ich habe ihn heute nicht wiedergefunden und trage ihn nicht mehr mit.
4. **Grudas Diagnose liegt vor und ist milder als befürchtet:** **Zerrung der seitlichen Bauchmuskulatur.** Er hat die **DFB-Reise abgesagt** und fehlt gegen Serbien und Griechenland – laut Bild braucht er aber nur **wenige Tage Pause**. Für den 10.10. spricht damit mehr für als gegen ihn. Nebeneffekt: Er reist nicht, sondern regeneriert in Leipzig. Aus dem gestrigen „zusätzlichen Risiko" ist ein leichter Vorteil geworden.
5. **Der Mainzer Trainer ist geklärt: Urs Fischer**, im Amt seit dem **07.12.2025** (nach Bo Henriksen und einer Interimswoche von Benjamin Hoffmann). Danach hatte ich bisher nicht gesucht – die Lücke war mir gar nicht aufgefallen.
6. **Die Højlund-Frage bleibt offen.** Kein neuer Befund. Sie steht seit vier Tagen unbeantwortet; ich lasse sie stehen, statt sie stillschweigend zu streichen.

## Nachrichtenlage in Kürze

**Gladbach hat einen Trainer – aber in der ersten Woche keine Innenverteidiger.** Das ist die wichtigste Meldung des Tages, und sie steht quer zu dem, was ich gestern geschrieben habe. Die Mannschaft ist **ohne sechs Nationalspieler** in die erste Trainingswoche gestartet, darunter **alle vier etatmäßigen Innenverteidiger: Kevin Diks, Jan Leszczynski, Ko Itakura und Fabio Chiarodia.** Ein Trainer, dessen Handschrift die geordnete Fünferkette ist, kann sie in Woche eins mit niemandem einstudieren, der sie später spielen soll. Ein **Testspiel beim FC St. Pauli am 3. Oktober** ist angesetzt – auch das noch im Abstellungszeitraum, der erst am 06.10. endet.

**Köln bekommt zwei Spieler zurück und verliert neun an die Nationalteams.** **Luca Waldschmidt** steht kurz vor der Rückkehr ins Mannschaftstraining. **Sebastian Sebulonsen** (Muskelverletzung, Rechtsverteidiger) ist „noch nicht nah dran", käme aber laut Bericht „im Oktober für das Derby gegen Gladbach" wieder infrage – ausdrücklich ohne Zusage. **Timo Hübers** fällt weiter langfristig aus. Trainer **René Wagner** lässt bis Dienstag trainieren, gibt dann einige Tage frei und schickt die Mannschaft mit individuellen Laufplänen in die Pause; ein Testspiel ist geplant. **Neun FC-Profis sind bei Auswahlmannschaften unterwegs.**

**Leipzig: Gruda bleibt da, Guiu bleibt offen.** Zu Guiu ist die Lage unverändert und ausdrücklich unentschieden: Muskelverletzung im linken hinteren Oberschenkel, Rückkehr im Oktober möglich, **ob es für den 10.10. gegen Frankfurt reicht, ist laut den zugänglichen Berichten offen.** Demichelis führt die Häufung von Muskelverletzungen auf den sprintlastigen Spielstil zurück: Mannschaften, die nicht aggressiv pressen, hätten „im modernen Fußball keine Chance".

**Mainz verliert einen Spieler für die Saison.** **Mathias Pereira Lage** fällt nach einer Knieverletzung (Kreuzbandriss) **für die Saison** aus.

**Werder reist mit Lücken im Mittelfeld.** Auf der Ausfallliste stehen **Jens Stage** (Oberschenkel) und **Senne Lynen** (Leiste). Die Angabe stammt aus der Vorschau zum Spiel gegen Augsburg (4. Spieltag), ist also rund drei Tage alt.

**Die Länderspielpause ist dieses Jahr länger als gewohnt.** Statt drei Unterbrechungen im Herbst gibt es nur zwei; der FIFA-Abstellungszeitraum läuft als Block vom **21.09. bis 06.10.**, die zweite Pause folgt vom 09. bis 17.11. Für den 5. Spieltag heißt das: **kein Europapokal davor**, dafür bei allen Klubs die Reisebelastung der Nationalspieler.

### Offen benannte Restlücken und Unsicherheiten

- **Zu Bayern, Dortmund, Augsburg und Freiburg habe ich für den 5. Spieltag weiterhin keine belastbare Personalmeldung.** Das sind vier von achtzehn Mannschaften – gestern waren es sechs; Werder und Mainz sind heute dazugekommen. Eine gezielte Suche zu Bayern und Dortmund lieferte ausschließlich Saison- und Rahmentermine, keine Personalien.
- **Zu Mainz kursieren drei weitere Namen, die ich nicht mittrage:** Eine Zusammenfassung nennt **James Sands** (Sprunggelenk) und **Manolis Saliakas** (Muskelverletzung) neben Pereira Lage. Die Herkunft dieser Angabe ließ sich nicht auf die laufende Saison zurückführen, und die Nachfrage brachte nur Treffer zur Saison 2025/26. **Nur Pereira Lage trage ich als belegt ein.**
- **Eine Suche nach aktuellen Verletzungen lieferte erneut Material aus der Saison 2025/26** (u. a. Davies). Das ist **nicht** der aktuelle Stand und fließt in keinen Tipp ein – wie gestern nenne ich es, weil es zeigt, wie leicht die Suchzusammenfassungen ohne Primärseiten die Saison verwechseln.
- **Zu Angelo Stiller (Stuttgart) bleibt der letzte Stand vom 13.09.** (Knieprellung/Hämatom, keine schwere Verletzung). Ich nehme ihn für den 09.10. als verfügbar an – **das ist eine Annahme, keine Meldung**, und sie steht jetzt seit neun Tagen ungeprüft.
- **Die Tabelle ist weiterhin aus den einzeln belegten Ergebnissen gerechnet**, weil keine Tabellenseite abrufbar ist. Eine heutige Zusammenfassung führt **Union nach dem 20.09. auf Rang 17 mit 0 Siegen, 1 Remis, 3 Niederlagen** – das deckt sich exakt mit meiner Rechnung. Fünfter unabhängiger Kontrollpunkt.
- **Randnotiz zu Lustrinelli:** Seine Trainerbilanz wird mit **5 Spielen (1 S, 1 U, 3 N)** geführt, die Union-Bilanz in der Liga mit 0 S, 1 U, 3 N. Der eine Sieg stammt also aus dem DFB-Pokal. Das ist konsistent, nicht widersprüchlich.

### Tabelle nach dem 4. Spieltag (alle 36 Partien)

Aus den einzeln belegten Ergebnissen gerechnet. Form = letzte bis erste Partie von links nach rechts.

| # | Verein | Sp | S | U | N | Tore | Diff | Pkt | Form |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Borussia Dortmund | 4 | 4 | 0 | 0 | 9:2 | +7 | 12 | S S S S |
| 2 | FC Bayern München | 4 | 3 | 1 | 0 | 14:2 | +12 | 10 | S U S S |
| 3 | SC Freiburg | 4 | 3 | 1 | 0 | 12:3 | +9 | 10 | S S S U |
| 4 | FC Augsburg | 4 | 2 | 1 | 1 | 11:6 | +5 | 7 | S S U N |
| 5 | Bayer 04 Leverkusen | 4 | 2 | 1 | 1 | 10:5 | +5 | 7 | N S U S |
| 6 | 1. FSV Mainz 05 | 4 | 2 | 1 | 1 | 10:6 | +4 | 7 | U S N S |
| 7 | SV 07 Elversberg | 4 | 2 | 1 | 1 | 8:7 | +1 | 7 | S S N U |
| 8 | SV Werder Bremen | 4 | 2 | 1 | 1 | 8:8 | 0 | 7 | N S U S |
| 9 | RB Leipzig | 4 | 2 | 0 | 2 | 9:5 | +4 | 6 | S N S N |
| 10 | Eintracht Frankfurt | 4 | 1 | 2 | 1 | 9:10 | −1 | 5 | U N S U |
| 11 | FC Schalke 04 | 4 | 1 | 2 | 1 | 3:4 | −1 | 5 | N U S U |
| 12 | SC Paderborn 07 | 4 | 1 | 1 | 2 | 3:5 | −2 | 4 | U N N S |
| 13 | 1. FC Köln | 4 | 1 | 1 | 2 | 6:9 | −3 | 4 | S N U N |
| 14 | TSG Hoffenheim | 4 | 1 | 0 | 3 | 7:10 | −3 | 3 | N N S N |
| 15 | VfB Stuttgart | 4 | 1 | 0 | 3 | 6:9 | −3 | 3 | N S N N |
| 16 | Hamburger SV | 4 | 1 | 0 | 3 | 2:13 | −11 | 3 | N N N S |
| 17 | 1. FC Union Berlin | 4 | 0 | 1 | 3 | 4:17 | −13 | 1 | U N N N |
| 18 | Bor. Mönchengladbach | 4 | 0 | 0 | 4 | 6:16 | −10 | 0 | N N N N |

**1. Spieltag (28.–30.08.):** Bayern 5:1 Stuttgart · Dortmund 2:0 HSV · Augsburg 3:0 Schalke · Union 3:3 Frankfurt · Köln 3:2 Hoffenheim · Freiburg 4:1 Werder · Leipzig 3:0 Gladbach · Paderborn 0:0 Mainz · Elversberg 3:2 Leverkusen
**2. Spieltag (04.–06.09.):** Stuttgart 4:1 Köln · Hoffenheim 2:3 Dortmund · Leverkusen 4:0 Union · Schalke 0:0 Bayern · Gladbach 3:4 Elversberg · Paderborn 0:1 Freiburg · Werder 3:1 Leipzig · HSV 0:5 Mainz · Frankfurt 1:4 Augsburg
**3. Spieltag (11.–13.09.):** Union 1:3 Schalke · Dortmund 3:0 Paderborn · Hoffenheim 2:1 Stuttgart · Freiburg 5:0 Gladbach · Augsburg 2:2 Leverkusen · Mainz 1:3 Frankfurt · Köln 1:1 Werder · Leipzig 5:0 HSV · Elversberg 1:2 Bayern
**4. Spieltag (18.–20.09.):** Bayern 7:0 Union · Frankfurt 2:2 Freiburg · Gladbach 3:4 Mainz · HSV 2:1 Köln · Werder 3:2 Augsburg · Stuttgart 0:1 Dortmund · Leverkusen 2:0 Leipzig · Schalke 0:0 Elversberg · Paderborn 3:1 Hoffenheim

### Gegenprobe zur Heimschwäche-Neigung

Fünf meiner sechs Fehltipps am 4. Spieltag gingen gegen die Heimmannschaft. Nach der heutigen Rücknahme stehen die neun Tipps wieder bei **fünf Heimsiegen, zwei Auswärtssiegen, zwei Remis**. Dass die Korrektur diesmal in die von der Fehleranalyse nahegelegte Richtung zeigt, ist ein angenehmer Nebeneffekt – **das Argument dafür ist es nicht.** Der Grund ist allein, dass die gestrige Begründung an ihrer eigenen Voraussetzung gescheitert ist. Hätte die neue Meldung in die andere Richtung gezeigt, stünde hier ein Auswärtssieg mehr.

---

## Die Tipps zum 5. Spieltag

### Borussia Dortmund – SV Werder Bremen
**Freitag, 09.10.2026, 20:30 Uhr**
**Tipp: 2:0**
Dortmund ist die einzige Mannschaft ohne Punktverlust (12 Punkte, 9:2) und hat in vier Spielen **zwei Gegentore** kassiert; **Schlotterbeck** ist seit dem 3. Spieltag zurück, **Beier** traf als Spieler des Spiels in Stuttgart. Werder hat am Samstag zwar ein 0:2 gegen Augsburg in ein 3:2 gedreht (Grüll, Füllkrug, Weiser), steht auswärts aber bei **zwei Punkten aus zwei Spielen mit 2:5 Toren** (1:4 in Freiburg, 1:1 in Köln).
*unverändert*
***Neu belegt, und es stützt den Tipp:** Werder fehlen im Mittelfeld **Jens Stage** (Oberschenkel) und **Senne Lynen** (Leiste) – die erste Personalmeldung zu Bremen, die ich für diesen Spieltag überhaupt habe. **Einschränkend:** Die Angabe stammt aus der Vorschau zum 4. Spieltag, ist also nicht auf den 09.10. datiert, und Werders Stärke bleibt genau die späte Phase, in der ich die Null ansetze – dreimal getroffen ab der 66. Minute. **Zu Dortmund habe ich weiterhin keine Personalmeldung.***

### FC Augsburg – FC Bayern München
**Samstag, 10.10.2026, 15:30 Uhr**
**Tipp: 1:3**
Bayern hat 14:2 Tore und kommt vom 7:0 gegen Union, bei dem **Olise** einen Dreierpack erzielte und **Kane** im 98. Spiel sein 100. Bundesligator machte. Augsburg ist zu Hause unbesiegt (3:0 gegen Schalke, 2:2 gegen Leverkusen) und war bis Samstag ungeschlagen – das trägt das Augsburger Tor. Gegen die Münchner Offensive hat nach vier Spieltagen aber noch niemand bestanden.
*unverändert*
***Einschränkend:** Bayerns Auswärtsspiele waren die engsten der Saison – **0:0 auf Schalke** und 2:1 in Elversberg, zusammen zwei Tore in zwei Spielen. Die 3 im Tipp stützt sich auf die Gesamtbilanz, nicht auf die Auswärtsbilanz; das bleibt die Schwachstelle. **Zu beiden Kadern habe ich auch nach gezielter Suche keine Meldung für Oktober** – das ist die größte Lücke dieses Tipps und heute der zweite vergebliche Anlauf.*

### TSG Hoffenheim – Hamburger SV
**Samstag, 10.10.2026, 15:30 Uhr**
**Tipp: 2:1**
Beide kommen mit drei Punkten, aber unter umgekehrten Vorzeichen: Hoffenheim nach **vier Niederlagen in fünf Pflichtspielen** (1:3 in Paderborn, 0:2 auf Kreta) in offener Krise, der HSV nach dem ersten Saisonsieg und der Vertragsverlängerung für **Polzin** bis 2029. Den Ausschlag gibt die Auswärtsbilanz: Hamburg hat seine beiden Auswärtsspiele **0:2 in Dortmund und 0:5 in Leipzig** verloren und dabei **kein Tor** erzielt, während Hoffenheim zu Hause Stuttgart 2:1 geschlagen hat.
*unverändert*
***Einschränkend:** Das ist ein Heimtipp für die Mannschaft in der schlechteren Verfassung – ich setze die Auswärtsschwäche des Gastes über die Form des Gastgebers. Hoffenheims einziger bekannter Verletzungsfall war zuletzt **Bernardo** (Achillessehne), **Machida** ist zurück – Stand vor der Pause. **Eine gezielte Suche zu beiden Kadern blieb heute ohne Ergebnis.***

### 1. FSV Mainz 05 – Bayer 04 Leverkusen
**Samstag, 10.10.2026, 15:30 Uhr**
**Tipp: 1:2**
Beide stehen bei sieben Punkten, aber Mainz holt seine Punkte fast ausschließlich auswärts: **0:0 in Paderborn, 5:0 beim HSV, 4:3 in Gladbach** – das einzige Heimspiel ging **1:3 gegen Frankfurt** verloren. Leverkusen kommt vom 2:0 gegen Leipzig mit einem treffenden **Schick** und einem **Miguel Gutiérrez**, der an beiden Toren beteiligt war, und hat in den letzten drei Spielen nur zwei Gegentore kassiert.
*unverändert*
***Neu belegt:** Mainz verliert **Mathias Pereira Lage** nach einer Knieverletzung **für die Saison**. Trainer ist **Urs Fischer**, seit Dezember 2025 im Amt – eine Lücke, die mir bis heute nicht aufgefallen war. **Was gegen meinen eigenen Tipp spricht, ausdrücklich:** Ein einziges Heimspiel ist eine dünne Grundlage für eine Heimschwäche-These, und Mainz hat in den letzten beiden Partien **neun Tore** erzielt. Leverkusen wiederum hat auswärts erst in Elversberg verloren (2:3) und in Augsburg nur remisiert. Das bleibt der am knappsten begründete der neun Tipps; ein Remis wäre genauso vertretbar.*

### 1. FC Union Berlin – SV 07 Elversberg
**Samstag, 10.10.2026, 15:30 Uhr**
**Tipp: 1:2**
Union steht bei einem Punkt und **4:17 Toren** – so viele Gegentore nach vier Spielen gab es zuletzt **1983**. Auch zu Hause fehlt die Stabilität: 3:3 gegen Frankfurt, **1:3 gegen Schalke**. Elversberg hat als Aufsteiger sieben Punkte, hat in **jedem** Spiel getroffen und auswärts in Gladbach 4:3 gewonnen sowie auf Schalke ein 0:0 geholt.
*unverändert*
***Was gegen meinen eigenen Tipp spricht, ausdrücklich:** Union bekommt gut zwei Wochen, um genau das zu reparieren, was Lustrinelli benannt hat, und ein Heimspiel gegen einen Aufsteiger ist die realistischste Gelegenheit auf den ersten Sieg. Ich tippe trotzdem gegen den Gastgeber, weil 17 Gegentore in vier Spielen kein Formproblem mehr beschreiben. **Zur Trainerfrage:** Eine gezielte Suche nach einer Entlassungsdebatte um Lustrinelli brachte **nichts** – kein Hinweis auf Druck von Vereinsseite. Elversberg fehlt weiterhin **Seifert** (Syndesmoseriss); ob das im Oktober noch gilt, weiß ich nicht.*

### SC Paderborn 07 – VfB Stuttgart
**Samstag, 10.10.2026, 15:30 Uhr**
**Tipp: 1:1**
Paderborn hat am Sonntag mit dem 3:1 gegen Hoffenheim den ersten Saisonsieg geholt und dabei so viele Tore erzielt wie in den drei Spielen davor zusammen (**Castaneda**, **Marino**, **Tigges**); zu Hause stand die Mannschaft vorher bei 0:1 Toren aus zwei Spielen. Stuttgart hat **aus zwei Auswärtsspielen null Punkte bei 2:7 Toren** geholt, dürfte aber von der langen Pause am meisten profitieren.
*unverändert*
***Warum ein Remis und kein Sieger:** Beide Argumente sind gleich stark und zeigen in entgegengesetzte Richtungen. **Heute geklärt:** Das Heimrecht liegt bei **Paderborn** – eine Suchzusammenfassung hatte die Partie andersherum geführt, drei unabhängige Belege sprechen dagegen (siehe oben). Die Paderborner Ausfallliste bleibt lang: **Awortwie-Grant** (Knie), **Eickel** (individuelles Training), **Gayret** (Kreuzbandriss); alle drei fehlten schon beim 3:1. **Stillers Verfügbarkeit bleibt eine Annahme von mir, inzwischen neun Tage alt.***

### RB Leipzig – Eintracht Frankfurt
**Samstag, 10.10.2026, 18:30 Uhr**
**Tipp: 2:1**
Leipzigs Saison zerfällt sauber in zwei Hälften: zu Hause **3:0 gegen Gladbach und 5:0 gegen den HSV** (8:0), auswärts **kein einziger Punkt** (1:3 in Bremen, 0:2 in Leverkusen). Frankfurt ist mit 9:10 Toren die unberechenbarste Mannschaft des oberen Mittelfelds – 3:1 in Mainz gewonnen, 1:4 gegen Augsburg verloren, zuletzt 2:2 gegen Freiburg mit zweimaliger Führung. Der Frankfurter Torgefahr traue ich auch in Leipzig einen Treffer zu, den Auswärtssieg nicht.
*unverändert*
***Die Leipziger Personallage hat sich heute leicht zum Besseren geklärt, ohne den Tipp zu bewegen:* Grudas** Diagnose lautet **Zerrung der seitlichen Bauchmuskulatur**; er hat die **DFB-Reise abgesagt** und fehlt gegen Serbien und Griechenland, braucht laut Bild aber **nur wenige Tage Pause**. Er bleibt also in Leipzig, statt zu reisen – aus dem gestrigen Risiko ist ein kleiner Vorteil geworden. Unverändert: **Assan Ouédraogo** fällt nach Schulter-OP für den Rest des Jahres aus; **Marc Guiu** (linker hinterer Oberschenkel) könnte im Oktober zurückkehren, **ob es für den 10.10. reicht, ist ausdrücklich offen.** **Zu Frankfurt habe ich weiterhin keine Personalmeldung** – die Højlund-Frage bleibt seit vier Tagen unbeantwortet.*

### 1. FC Köln – Borussia Mönchengladbach
**Sonntag, 11.10.2026, 15:30 Uhr**
**Tipp: 2:1**
**Änderung gegenüber gestern: 1:1 → 2:1, weil die Voraussetzung der gestrigen Änderung heute widerlegt ist.** Gestern hatte ich von 2:1 auf 1:1 geändert – mit der Begründung, Blessin bekomme „die komplette Länderspielpause" zur Einarbeitung und könne damit genau den Defekt beheben, der Gladbach ruiniert (16 Gegentore in vier Spielen). Heute ist bekannt: Borussia ist **ohne sechs Nationalspieler** in die erste Trainingswoche gegangen, darunter **alle vier etatmäßigen Innenverteidiger – Diks, Leszczynski, Itakura und Chiarodia.** Der Abstellungszeitraum endet erst am **06.10.**; auch das **Testspiel bei St. Pauli am 3. Oktober** liegt noch darin.

Damit bricht die Begründung weg, nicht nur die Gewichtung: Ein Trainer, dessen dokumentierte Stärke die geordnete Fünferkette ist, hat für deren Einstudierung nicht zweieinhalb Wochen, sondern die wenigen Tage zwischen Rückkehr der Innenverteidiger und Derby. Dazu kommt auf Kölner Seite eine Meldung in die Gegenrichtung: **Luca Waldschmidt** steht kurz vor der Rückkehr ins Mannschaftstraining, und **Sebastian Sebulonsen** käme laut Bericht „im Oktober für das Derby" wieder infrage.
***Was gegen die Rücknahme spricht, ausdrücklich:** Ein Tipp, der an zwei aufeinanderfolgenden Tagen hin- und herspringt, ist an sich ein schlechtes Zeichen – er verrät, dass ich gestern aus einer Meldung mehr gemacht habe, als sie hergab. Die ehrliche Lesart ist: **Die gestrige Änderung war voreilig.** Die Trainerverpflichtung als solche stimmte, meine Annahme über die Trainingsbedingungen nicht. Zweitens bleibt Blessins Verpflichtung ein echter Faktor – er hat die Mannschaft immerhin gut zwei Wochen, wenn auch ohne die entscheidenden vier Spieler, und ein Derby ist der Wettbewerb, in dem ein neuer Trainer am ehesten einen Effekt erzielt. **Ein 1:1 bleibt gut vertretbar; ich halte 2:1 nach dem heutigen Stand für das wahrscheinlichere Ergebnis, nicht für das einzig mögliche.** Drittens fehlen auch Köln **neun Profis** an Auswahlmannschaften – die Abstellungslast trifft beide, nur trifft sie Gladbach an der einen Stelle, an der es weh tut. Belegt und unstrittig: Blessin hat **bis 2028** unterschrieben, wird am **Mittwoch um 13:30 Uhr** vorgestellt, **Lichte** bleibt Assistent; Kölns Trainer ist **René Wagner**, **Hübers** fällt langfristig aus.*

### SC Freiburg – FC Schalke 04
**Sonntag, 11.10.2026, 17:30 Uhr**
**Tipp: 2:0**
Freiburg ist als Dritter mit 12:3 Toren unbesiegt und zu Hause besonders deutlich: **4:1 gegen Werder, 5:0 gegen Gladbach** (9:1). Schalke hat in vier Spielen **drei Tore** erzielt – die wenigsten der Liga – und kam zuletzt zu Hause nicht über ein 0:0 gegen Elversberg hinaus. Der Europapokal belastet Freiburg an diesem Wochenende nicht, weil die europäischen Wettbewerbe in der Länderspielpause ruhen.
*unverändert*
***Die Anstoßzeit ist heute gegen einen Widerspruch verteidigt worden:** Eine Zusammenfassung behauptete 17:00 Uhr; die Nachfrage ergab **17:30 Uhr, Sonntag, DAZN**, und im Bundesliga-Sonntagsraster (15:30 / 17:30) gibt es keinen 17:00-Slot. **Unverändert belegt:** Schalke fehlen **Emil Højlund** (Achillessehnen-Reha), **Dejan Ljubičić** (linkes Knie, „bis auf Weiteres") und **Johannes Siebeking** (Bauchmuskel). **Einschränkend bleibt:** Schalke hat erst **vier** Gegentore kassiert, weniger als alle außer Bayern und Dortmund – ein 1:0 wäre ebenso plausibel. **Freiburgs Kaderlage für Oktober kenne ich nicht**; die heutige gezielte Suche blieb ergebnislos.*

---

## Quellen

Ausschließlich Websuche; Primärseiten sind aus dieser Umgebung nicht abrufbar. Heute erneut einzeln per curl geprüft (kicker.de, bundesliga.com, weltfussball.de, transfermarkt.de, sportschau.de – jeweils Rückgabewert `000`); die Proxy-Statusabfrage weist `connect_rejected / 403 to CONNECT` aus. Am Fetch-Werkzeug mit `EGRESS_BLOCKED` gescheitert: datencenter.dfb.de, anstosszeiten.de, vfb.de, ligainsider.de, diebewertung.de.

**Spielplan und Anstoßzeiten 5. Spieltag**
- [DFB Datencenter – Bundesliga 2026/27, 5. Spieltag](https://datencenter.dfb.de/datencenter/bundesliga/2026-2027/5) — Fetch blockiert, nur als Treffer nachgewiesen
- [SC Freiburg – Dates and kick-off times confirmed for matchdays 5 to 11](https://www.scfreiburg.com/en/latest/first-team/news/2026-27/dates-and-kick-off-times-confirmed-for-matchdays-5-to-11/) — nur über Suchzusammenfassung
- [VfB Stuttgart – Bundesliga-Ansetzungen Spieltag fünf bis elf](https://www.vfb.de/de/vfb/aktuell/neues/profis/2627/bundesliga-ansetzungen-spieltag-fuenf-bis-elf/) — Fetch blockiert
- [kicker – Spielinfo SC Paderborn 07 – VfB Stuttgart, 5. Spieltag](https://www.kicker.de/paderborn-gegen-stuttgart-2026-bundesliga-5226853/spielinfo) — nur über Suchzusammenfassung
- [bundesliga.com – Paderborn vs VfB Stuttgart, Matchday 5](https://www.bundesliga.com/en/bundesliga/matchday/2026-2027/5/sc-paderborn-07-vs-vfb-stuttgart/lineup) — nur über Suchzusammenfassung
- [bundesliga.com – Freiburg vs Schalke 04, Matchday 5](https://www.bundesliga.com/en/bundesliga/matchday/2026-2027/5/sport-club-freiburg-vs-fc-schalke-04/lineup) — nur über Suchzusammenfassung
- [anstosszeiten.de – Sonntagsspiele 2026/27](https://anstosszeiten.de/bundesliga/sonntagsspiele/) — Fetch blockiert
- [fussballdaten.de – 1. FC Köln – Borussia Mönchengladbach, 5. Spieltag](https://www.fussballdaten.de/bundesliga/2027/5/koeln-mgladbach/)

**Gladbach / Blessin**
- [sportschau.de – Soll Borussia retten: Blessin ist neuer Trainer in Mönchengladbach](https://www.sportschau.de/regional/wdr/wdr-blessin-neuer-trainer-in-gladbach-100.html)
- [Sky Sport – Alexander Blessin wird neuer Trainer von Borussia Mönchengladbach](https://sport.sky.de/fussball/artikel/alexander-blessin-wird-neuer-trainer-von-borussia-moenchengladbach/13590672/34252)
- [bundesliga.com – Borussia Mönchengladbach: Polanski-Nachfolger gefunden](https://www.bundesliga.com/de/bundesliga/news/alexander-blessin-gladbach-trainer-fix-nachfolger-eugen-polanski-39297)
- [absolutfussball.com – Vertrag bis 2028: Blessin wird neuer Trainer in Gladbach](https://www.absolutfussball.com/deutschland/borussia-moenchengladbach/vertrag-bis-2028-blessin-wird-neuer-trainer-in-gladbach-94504800.html)
- [sport.de – Keine Ablöse fällig? Gladbach stellt Polanski-Nachfolger vor](https://www.sport.de/news/ne17176543/keine-abloese-faellig-gladbach-stellt-polanski-nachfolger-vor/)
- [borussia.de – Start in die Testspielwoche](https://www.borussia.de/news/start-in-die-testspielwoche)
- [t-online.de – Schweres Auftaktprogramm für Alexander Blessin](https://www.t-online.de/sport/fussball/bundesliga/id_101446692/borussia-moenchengladbach-schweres-auftaktprogramm-fuer-alexander-blessin.html)
- [tagesspiegel.de – Alexander Blessin übernimmt als Trainer in Mönchengladbach](https://www.tagesspiegel.de/sport/dpa-fussball-bundesliga-alexander-blessin-ubernimmt-als-trainer-in-monchengladbach-16084165.html)

**Köln**
- [geissblog.koeln – „Nichts aufbrechen": Wagner erklärt Stürmer-Pause, spielt Sebulonsen erst im Oktober?](https://geissblog.koeln/2026/08/nichts-aufbrechen-wagner-erklaert-stuermer-pause-spielt-sebulonsen-erst-im-oktober)
- [absolutfussball.com – FC Kölns Plan für die Pause: Training, Erholung und Testspiel](https://www.absolutfussball.com/deutschland/1-fc-koeln/fc-koelns-plan-fuer-die-pause-training-erholung-und-testspiel-zr-94504258.html)
- [come-on-fc.com – Waldschmidt zurück, Van den Berg fehlt erneut: Mit diesem Kader reist der 1. FC Köln nach Hamburg](https://come-on-fc.com/profis/kader-des-fc-koeln-fuer-hamburg/)
- [headtopics.de – „Zeit für Themen": Wagners Plan für XXL-Pause – neun FC-Profis unterwegs](https://de.headtopics.com/news/zeit-fur-themen-wagners-plan-fur-xxl-pause-neun-87964237)

**Leipzig**
- [ligainsider.de – Diagnose da: Gruda sagt DFB-Reise ab](https://www.ligainsider.de/brajan-gruda_35733/diagnose-da-gruda-sagt-dfb-reise-ab-418389/)
- [Sky Sport – Brajan Gruda verletzt: RB-Leipzig-Profi verpasst DFB-Länderspiele unter Jürgen Klopp](https://sport.sky.de/fussball/artikel/brajan-gruda-verletzt-rb-leipzig-profi-verpasst-dfb-laenderspiele-unter-juergen-klopp/13590465/34130)
- [sportschau.de – Brajan Gruda verletzt: Länderspielaus für Gruda](https://www.sportschau.de/audio/laenderspielaus-fuer-gruda,brajan-gruda-rb-leipzig-100.html)
- [rbleipzig.com – Marc Guiu: Verletzung und Comeback](https://rbleipzig.com/de/news/marc-guiu-verletzung-rb-leipzig-comeback)
- [rblive.de – Mit Marc Guiu fällt der nächste Profi länger aus](https://rblive.de/news/rb-leipzig-vor-leverkusen-mit-marc-guiu-faellt-der-naechste-profi-laenger-aus-4322264)
- [bundesliga.com – RB Leipzig striker Marc Guiu suffers injury setback](https://www.bundesliga.com/en/bundesliga/news/marc-guiu-rb-leipzig-injury-spain-chelsea-39243)

**Mainz / Werder**
- [ligainsider.de – 1. FSV Mainz 05: Voraussichtliche Aufstellung 2026/27](https://www.ligainsider.de/1-fsv-mainz-05/17/) — Fetch blockiert
- [Sports Mole – Preview: Werder Bremen vs Augsburg, team news](https://www.sportsmole.co.uk/football/werder-bremen/preview/werder-bremen-vs-augsburg-prediction-team-news-lineups_605365.html)

**Union Berlin**
- [fc-union-berlin.de – Mauro Lustrinelli wird neuer Cheftrainer](https://www.fc-union-berlin.de/de/meldungen/meisterlicher-taktgeber-fuer-unions-maenner-mauro-lustrinelli-wird-neuer-cheftrainer-tCyufa)
- [sportschau.de – Union Berlins neuer Coach: Lustrinelli operiert am offenen Herzen](https://www.sportschau.de/regional/rbb/rbb-union-berlin-neuer-coach-lustrinelli-operiert-am-offenen-herzen-100.html)
