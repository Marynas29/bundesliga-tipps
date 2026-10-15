# Bundesliga-Tipps – 6. Spieltag 2026/27 (Stand: 15.10.2026)

**Ansetzung:** Freitag, 16.10. bis Sonntag, 18.10.2026.
**Vortagsstand:** 14.10.2026, **ebenfalls 6. Spieltag** — echter Vergleich für alle neun Partien möglich.

**Ergebnis dieses Laufs in einem Satz:** **Zwei Tipps geändert, sieben unverändert** — und beide Änderungen gehen auf Schwellen zurück, die ich vor Tagen schriftlich festgelegt habe und die heute **erstmals ausgelöst** haben: **Frankfurt – Köln 2:1 → 3:1** (Rondic fällt neu aus, Köln reist mit fünf Ausfällen plus Langzeitverletztem und Nachwuchsspielern auf der Bank) und **Leverkusen – Freiburg 2:2 → 3:2** (Maza ist belegt Starter und hat in Posen getroffen). **Dazu sind die drei Donnerstagsspiele gelaufen** — **Leverkusen 4:0 in Posen, Hoffenheim 2:3 zu Hause gegen Beşiktaş, Freiburg 3:2 gegen Jablonec** — **und vier alte Lücken sind geschlossen:** **Kölns beide unbenannte Ausfälle (van den Berg, Hübers), Leipzigs Trainer (Demichelis), Paderborns Trainer (Kettemann) und der Endstand in Bratislava (3:0).** **Damit sind erstmals alle 18 Trainer belegt.** **Die Quellensperre besteht zum fünften Tag, mit einem neuen Befund zum Abrufweg.**

---

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Der Befund der Vortage ist heute erneut geprüft, unverändert — und um einen Punkt genauer geworden.**

- **Der Proxy ist funktionsfähig.** `curl -sS "$HTTPS_PROXY/__agentproxy/status"` lief durch: `enabled: true`, `bundleCoversEveryHost: true`, `recentRelayFailures: []`.
- **Die Fußballquellen bleiben durch die Egress-Policy dieser Umgebung gesperrt.** Heute zwei Testabrufe, beide gescheitert: `www.kicker.de` und `www.bundesliga.com` enden mit `CONNECT tunnel failed, response 403`. ***Das ist eine Richtlinienablehnung, kein Quellenproblem*** — und `/root/.ccr/README.md` schreibt für 403 ausdrücklich vor, den gesperrten Host zu melden statt die Sperre zu umgehen.
- ***Neu und präziser als an den Vortagen:*** **auch der Abruf über das `WebFetch`-Werkzeug scheitert, aber mit einer anderen Fehlermeldung** — `getaddrinfo ENOTFOUND www.bundesliga.com`, also ein Fehlschlag bereits bei der Namensauflösung. **Beide Wege sind damit zu, auf zwei verschiedene Weisen.** *Das schließt die Vermutung aus, die Sperre betreffe nur `curl`.*
- ***Was der Nutzer tun kann, wenn er Volltexte will:*** **Im Menü der Cloud-Umgebung in der Titelzeile der Sitzung → „Edit" → Network access**: entweder eine breitere Zugriffsstufe wählen oder `kicker.de`, `bundesliga.com`, `weltfussball.de` und `transfermarkt.de` unter **Allowed domains** eintragen (Häkchen „Allow package managers" gesetzt lassen). Dokumentiert unter https://code.claude.com/docs/en/cloud-environments#network-access. **Solange das so bleibt, kann ich die vier im Routine-Prompt genannten Leitquellen dauerhaft nicht im Volltext lesen.**
- **`WebSearch` funktioniert und war wieder die tragende Quelle.** **Alles Folgende steht auf Suchergebnis-Zusammenfassungen und -Titeln, kein Volltext.**
- ***Qualitativer Befund des Tages:*** **Der Donnerstag ist der ergiebigste Tag dieses Spieltags gewesen.** **Fünf Spieltags-Pressekonferenzen sind ausgewertet** (Schalke, Mainz, Werder, Elversberg, Augsburg), **drei Europapokalspiele mit Aufstellungen und Torfolgen**, **zwei veröffentlichte voraussichtliche Aufstellungen** zu Frankfurt – Köln. *Zum Vergleich: gestern waren es zwei PKs und zwei Ergebnisse.*
- **Die Tabelle unten ist weiterhin selbst gerechnet** — **aber sie ist heute erstmals von außen gegenbestätigt** (siehe dort).

---

## Die Nachrichtenlage

**Der Donnerstagabend hat drei Pflichtspiele gebracht, und alle drei betreffen Partien dieses Spieltags.** **Bayer Leverkusen hat 4:0 bei Lech Posen gewonnen** — Patrik Schick traf in der 29. und 41. Minute je per Strafstoß, Malik Tillman in der 32., Ibrahim Maza in der 89.; zur Pause stand es 3:0. ***Entscheidend für meinen Tipp ist aber nicht das Ergebnis, sondern die Aufstellung:*** **Martínez Novell hatte mit Blick auf das Sonntagsspiel rotiert — Schick sollte pausieren, im Sturm begann Martin Terrier, Lucas Vázquez verteidigte rechts statt Quansah, Ezequiel Fernández spielte neben Aleix García, Andrich bekam eine Pause.** **Terrier verletzte sich früh, Schick kam in der 18. Minute und wurde vor der Schlussviertelstunde wieder ausgewechselt.** **Die TSG Hoffenheim hat 2:3 gegen Beşiktaş verloren** — Murillo (60.), Asllani (68.), Oh Hyeon-gyu (72. und 79.), Machida (87.); **es ist die vierte Pflichtspielniederlage in Folge**, und Kapitän Oliver Baumann sagt, die Mannschaft habe „zu wenig Punkte für die Leistung" geholt. **Der SC Freiburg hat 3:2 gegen Jablonec gewonnen** — Grifo (15., direkter Freistoß), Růsek (28./29., abgelenkt von Ginter), Eigentor Pavlović (53./58., nach Videobeweis), Eggestein (65.), Kuol (90.+3). ***Und hier ist die Aufstellung die eigentliche Nachricht:*** **Schuster hat Rotation angekündigt, aber nur auf einer Position rotiert** — Höler stürmte statt Matanović, ***Suzuki und Grifo begannen beide***, weil **Suzukis Gelb-Rote Karte gegen Schalke nur in der Bundesliga sperrt.** *Es war Schusters 100. Pflichtspiel, der neunte Erfolg in Folge ohne Niederlage.*

**Der zweite große Block sind fünf Spieltags-Pressekonferenzen — nach zwei am Mittwoch.** **Miron Muslić muss auf Moussa Sylla verzichten: der Stürmer hat sich im Spiel bei Freiburg am linken Bein verletzt, der Verein nennt weder Diagnose noch Dauer.** *Sylla hatte vier der fünf Ligaspiele begonnen und galt als erste Wahl vor Edin Džeko — **für die schwächste Offensive der Liga ist das der schwerste mögliche einzelne Ausfall.*** **Urs Fischer nennt Mainz' Problem beim Namen: zehn Gegentore in den letzten drei Bundesligaspielen, es fehle an Abständen und Kompaktheit** — *und dabei steht Mainz auswärts perfekt und zu Hause ohne Sieg.* **Daniel Thioune hat Amos Pieper für die Startelf zurück, Mitchell Weiser ist „wohl noch kein Startelf-Kandidat"** — *Thioune sieht „jetzt gerade keinen Grund, irgendwelche Wechsel vorzunehmen".* **Manuel Baum meldet Marius Wolf fit, Noahkai Banks fehlt mit Außenbandverletzung im Knie „zwei, drei, vier Wochen mindestens", Alexis Claude-Maurice mit Muskelverletzung.** **Vincent Wagner hat die Elversberger Linie mit einem Scherz zusammengefasst** („Wir versuchen, den Ball weiter wegzuschießen als Manuel Neuer").

**Drittens, und für Freitag entscheidend: Kölns Personallage ist heute zusammengebrochen.** **Imad Rondic hat sich am Donnerstag im Training eine Muskelverletzung im Oberschenkel zugezogen** (*eine genaue Diagnose wollte der Verein auf Nachfrage noch nicht bestätigen*), **und Rav van den Bergs Ausfall mit Muskelverletzung ist bestätigt.** **Damit fehlen neben dem langzeitverletzten Timo Hübers fünf Spieler: Skhiri, Dallinga, Ache, van den Berg, Rondic.** **Der Verteidiger Assad Kotya-Fofana steht erstmals im Spieltagskader, weitere Nachwuchsspieler reisen mit nach Frankfurt.** *Damit ist die Lücke von gestern geschlossen — ich kannte drei der fünf Namen.*

**Viertens die beiden Torwart- und Personalfragen, die zwei Topspiele betreffen.** **Manuel Neuer hat am Donnerstag im Mannschaftstraining gefehlt und stattdessen im Leistungszentrum gearbeitet; die Entscheidung über den Einsatz gegen Leipzig fällt nach dem Abschlusstraining am Freitag.** *Mehrere Berichte titeln „wohl nicht fit" — **eine Vereinsmeldung oder ein Kaderaufgebot liegt nicht vor.*** **Und zu Dortmund gibt es die stärkste Aussage bisher, aber nicht aus der Quelle, auf die meine Schwelle wartet: Sportdirektor Lars Ricken hat am Flughafen gesagt, Schlotterbeck werde „bei Union Berlin dann auch wieder dabei sein"; `bvb.de` selbst nennt als Grund für das Fehlen in Bodø ausdrücklich Belastungssteuerung, also keine Verletzung.**

**An der Spitze bleibt es bei Freiburg und Dortmund punktgleich mit 13 Zählern, Gladbach ist punktlos Letzter.** **Ein DFB-Pokalspiel liegt diese Woche nicht an, eine Länderspielpause läuft nicht.**

### Die Europapokalwoche — vollständig, alle sieben Spiele gelaufen

| Tag | Partie | Wettbewerb | Lage | Ergebnis |
|---|---|---|---|---|
| **Di 13.10.** | Viking Stavanger – **FC Bayern** | Champions League | auswärts | **3:3** — Kane (54. E, 60.), Díaz (71.); Gelb-Rot Olise (73.); Urbig im Tor für Neuer |
| **Di 13.10.** | **RB Leipzig** – PSV Eindhoven | Champions League | heim | **1:0** — Gruda (75.) |
| **Mi 14.10.** | Bodø/Glimt – **Bor. Dortmund** | Champions League | auswärts | **0:1** — Sjøvold (52.); erste Pflichtspielniederlage des BVB |
| **Mi 14.10.** | Slovan Bratislava – **VfB Stuttgart** | Champions League | auswärts | **0:3 (Endstand jetzt belegt)** — Undav (29.), Eigentor Cruz (64./65.), Demirović (90.); Camaras Tor (53.) nach VAR aberkannt |
| **Do 15.10.** | Lech Posen – **Bayer Leverkusen** | Europa League | auswärts (Polen) | **0:4** — Schick (29. E, 41. E), Tillman (32.), Maza (89.); **Terrier früh verletzt** |
| **Do 15.10.** | **TSG Hoffenheim** – Beşiktaş | Europa League | heim | **2:3** — Murillo (60.), Asllani (68.), Oh (72., 79.), Machida (87.) |
| **Do 15.10.** | **SC Freiburg** – FK Jablonec | Conference League | heim | **3:2** — Grifo (15.), Růsek (28./29.), Eigentor Pavlović (53./58.), Eggestein (65.), Kuol (90.+3) |

**Stand nach zwei Spielen:** **Leverkusen 6 Punkte, Stuttgart 6 Punkte, Leipzig sechs Punkte aus zwei Siegen nicht belegt, Hoffenheim 0 aus 2 mit 2:5.** *Für die Bundesligatipps zählt vor allem die Belastung: **Freiburg hat Donnerstag 21:00 mit fast der ersten Elf gespielt und tritt Sonntag 15:30 auswärts an. Hoffenheim hat Donnerstag 21:00 gespielt und tritt Sonntag 17:30 auswärts an. Leverkusen hat Donnerstag 18:45 in Polen rotiert gespielt und hat Sonntag Heimrecht.***

### Pressekonferenzen — der Donnerstag war der Haupttag

**Stattgefunden und ausgewertet:** **Frankfurt und Köln (Mi 14.10.)** · **Schalke, Mainz, Werder, Elversberg, Augsburg (Do 15.10.)** · **Stuttgart (Di 13.10., vor Bratislava, mit Aussagen zu Mittelstädt und zur Innenverteidigung für Samstag).** · **Angesetzt: Gladbach am Freitag, 16.10. — dort fällt laut Bericht die endgültige Einsatzprognose zu Kleindienst.** · **Zu Bayern, Leverkusen, Dortmund, Leipzig, HSV, Union, Hoffenheim, Freiburg und Paderborn ist mir kein Spieltags-PK-Bericht bekannt.** *Zu Union und Dortmund liegen stattdessen Vorberichte mit Trainer- bzw. Sportdirektorenzitaten vor, zu Bayern Berichte vom Donnerstagstraining.*

---

## Korrekturen am Vortagsstand

**Sechs Punkte. Zwei sind eigene Fehlurteile in Richtung Übervorsicht, vier sind Auflösungen offener Widersprüche.**

1. ***Mein Vorbehalt gegen den Bratislava-Endstand war unnötig.*** **Gestern schrieb ich: „Ich führe den Sieg als belegt, den Endstand nicht" und stellte die Sportschau-Fundstelle mit dem 3:0 unter Vorbehalt (verworfene Fundstelle 2).** **Richtig ist: Stuttgart hat 3:0 gewonnen** — Undav (29.), Eigentor Sandro Cruz (64./65.), Demirović (90.), übereinstimmend bei `bundesliga.com`, `sportschau.de`, `zdf.de`, `vfb.de`, `eurosport.de` und ESPN („S Bratislava 0-3 Stuttgart"). ***Die Fundstelle hatte recht, meine Einordnung war zu misstrauisch — derselbe Fehlertyp wie gestern bei Augsburgs Trainer.***
2. ***Osterhage steht nicht auf Freiburgs Ausfallliste, und das war schon gestern falsch.*** **Gestern führte ich „nach dem Stand vom 12.10. Beste, Osterhage und Yılmaz" als Freiburger Ausfälle.** **Osterhage hat am Donnerstag in der Startelf gegen Jablonec gespielt.** *Ich streiche ihn. **Zu Beste finde ich auch heute keinen Beleg und führe ihn deshalb nicht mehr als Ausfall, sondern als unbekannt.** Yılmaz fehlt — neu und mit Grund: **nach einer Zahnoperation.***
3. **Kölns zwei unbenannte Ausfälle sind aufgelöst.** **Gestern: „Kölns fünf Ausfälle sind nur zu drei Namen aufgelöst (Skhiri, Dallinga, Ache); die beiden übrigen kenne ich nicht."** **Es sind Rav van den Berg (Muskelverletzung, Ausfall heute bestätigt) und — als sechster, langzeitverletzt — Timo Hübers.** *Heute neu hinzugekommen ist Imad Rondic, sodass es nun **fünf Ausfälle plus Hübers** sind.*
4. **Freiburgs Torverhältnis ist nicht mehr strittig.** **Gestern: „13:3 gegen 14:4".** **Es ist 14:4** — `weltfussball.de`, `bulibox.de` und die deutsche Wikipedia führen Freiburg einheitlich mit 5 Spielen, 4 Siegen, 1 Remis, 14:4 und 13 Punkten. *Meine selbst gerechnete Tabellenzeile war richtig.*
5. **Leipzigs Trainer ist belegt: Martín Demichelis**, seit 22.06.2026 mit Zweijahresvertrag bis 2028, Nachfolger von Ole Werner, gekommen von RCD Mallorca — `sportschau.de`/MDR, `zdfheute.de`, `bundesliga.com`, `neunzigplus.de`. ***Einschränkung, die ich nicht verschweige: die Fundstellen datieren aus Juni und August 2026, eine Bestätigung aus dem Oktober habe ich nicht.*** *Eine Trennung ist in den Treffern nirgends berichtet.*
6. **Paderborns Trainer ist belegt: Ralf Kettemann**, Aufstiegstrainer (2:1 n.V. in der Relegation gegen Wolfsburg am 25.05.2026), Nachfolger von Lukas Kwasniok, erstes Cheftraineramt — `zdfheute.de`, `sportschau.de`, `bundesliga.com`. *Jüngste Fundstelle: Interview vom 30.08.2026.* ***Damit ist die vierte Lücke des Tages geschlossen und die Trainerliste erstmals vollständig.***

---

## Tabelle nach dem 5. Spieltag (vollständig)

**Unverändert gegenüber gestern — in der Bundesliga ist seit dem 5. Spieltag kein Spiel hinzugekommen.** ***Neu: die Spitze ist heute erstmals von außen bestätigt*** — `weltfussball.de`, `bulibox.de` und die deutsche Wikipedia nennen Freiburg (14:4, 13), Dortmund (11:4, 13), Bayern (16:4, 11) und Leverkusen (14:8, 10) **genau wie meine Zeilen.** *Eine `kicker.de`-Spieltagsseite zeigte alle Teams mit 0 Punkten (Platzhalteransicht), eine `sport.de`-Tabelle nur vier Spiele — beide verworfen.* **Form = 1. bis 5. Spieltag von links nach rechts.**

| # | Verein | Sp | S | U | N | Tore | Diff | Pkt | Form | Europapokal diese Woche |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | SC Freiburg | 5 | 4 | 1 | 0 | 14:4 | +10 | 13 | S S S U S | **Do, Conf. League, heim — 3:2** |
| 2 | Borussia Dortmund | 5 | 4 | 1 | 0 | 11:4 | +7 | 13 | S S S S U | **Mi, CL, auswärts — 0:1** |
| 3 | FC Bayern München | 5 | 3 | 2 | 0 | 16:4 | +12 | 11 | S U S S U | **Di, CL, auswärts — 3:3** |
| 4 | Bayer 04 Leverkusen | 5 | 3 | 1 | 1 | 14:8 | +6 | 10 | N S U S S | **Do, EL, auswärts — 4:0** |
| 5 | RB Leipzig | 5 | 3 | 0 | 2 | 15:5 | +10 | 9 | S N S N S | **Di, CL, heim — 1:0** |
| 6 | FC Augsburg | 5 | 2 | 2 | 1 | 13:8 | +5 | 8 | S S U N U | — |
| 7 | SV Werder Bremen | 5 | 2 | 2 | 1 | 10:10 | 0 | 8 | N S U S U | — |
| 8 | 1. FSV Mainz 05 | 5 | 2 | 1 | 2 | 13:10 | +3 | 7 | U S N S N | — |
| 9 | SV 07 Elversberg | 5 | 2 | 1 | 2 | 8:8 | 0 | 7 | S S N U N | — |
| 10 | 1. FC Köln | 5 | 2 | 1 | 2 | 8:10 | −2 | 7 | S N U N S | — |
| 11 | VfB Stuttgart | 5 | 2 | 0 | 3 | 8:9 | −1 | 6 | N S N N S | **Mi, CL, auswärts — 3:0** |
| 12 | Hamburger SV | 5 | 2 | 0 | 3 | 5:15 | −10 | 6 | N N N S S | — |
| 13 | FC Schalke 04 | 5 | 1 | 2 | 2 | 5:6 | −1 | 5 | N U S U N | — |
| 14 | Eintracht Frankfurt | 5 | 1 | 2 | 2 | 9:16 | −7 | 5 | U N S U N | — |
| 15 | SC Paderborn 07 | 5 | 1 | 1 | 3 | 3:7 | −4 | 4 | U N N S N | — |
| 16 | 1. FC Union Berlin | 5 | 1 | 1 | 3 | 5:17 | −12 | 4 | U N N N S | — |
| 17 | TSG Hoffenheim | 5 | 1 | 0 | 4 | 9:13 | −4 | 3 | N N S N N | **Do, EL, heim — 2:3** |
| 18 | Bor. Mönchengladbach | 5 | 0 | 0 | 5 | 7:18 | −11 | 0 | N N N N N | — |

**Heute gegenbestätigt:** **Elversberg steht laut dpa als Aufsteiger „bislang bei sieben Punkten"** — deckt sich mit Zeile 9. **Mainz gilt in den PK-Berichten als auswärts ungeschlagen und zu Hause sieglos** — passt zu 7 Punkten aus 2 Siegen, 1 Remis, 2 Niederlagen. **Schalkes „schwächste Offensive" (5 Tore) und Paderborns 3 Tore** sind in den Vorberichten unverändert.

---

## Trainer — erstmals 18 von 18 belegt

**Frankfurt** Adi Hütter · **Köln** René Wagner (Interim) · **Dortmund** Niko Kovač (Vertrag bis 2029) · **Werder** Daniel Thioune · **Gladbach** Alexander Blessin (bis 2028) · **Schalke** Miron Muslić · **Freiburg** Julian Schuster (heute 100. Pflichtspiel) · **Mainz** Urs Fischer · **Hoffenheim** Christian Ilzer · **Stuttgart** Sebastian Hoeneß · **Union** Mauro Lustrinelli · **Elversberg** Vincent Wagner · **Bayern** Vincent Kompany · **Leverkusen** Carles Martínez Novell (seit 01.07.2026, bis 2028) · **Augsburg** Manuel Baum (seit 01.12.2025, bis 2028) · **HSV** Merlin Polzin · **Leipzig** Martín Demichelis (**neu belegt**, seit 22.06.2026, bis 2028) · **Paderborn** Ralf Kettemann (**neu belegt**, Aufstiegstrainer 2026).

***Die Einschränkung gehört dazu:*** *zu Demichelis und Kettemann sind meine jüngsten Fundstellen vom Juni bzw. 30. August 2026. **Beide Namen tragen keinen meiner Tipps** — Leipzig betrifft Partie 7, deren Begründung auf Tabellen- und Formwerten steht, Paderborn Partie 4.*

---

## Heute geprüft und verworfen

1. **Eine erste Suchzusammenfassung, Freiburg habe „auf sieben Positionen rotiert".** **Verworfen und durch die Aufstellungsmeldung ersetzt:** *die offiziellen Aufstellungen zeigen **eine** Änderung gegenüber der erwarteten Elf (Höler für Matanović). Die sieben Wechsel waren **Einwechslungen** nach der Pause. **Das ist der folgenreichste verworfene Befund des Tages — er hätte Partie 8 in die falsche Richtung gedreht.***
2. **Ein `sport.de`-Liveticker zu Hoffenheim – Beşiktaş, der Kökçü und Vlahović als Torschützen der ersten Halbzeit führt.** **Verworfen:** *die erste Halbzeit endete 0:0; die Mehrheit der Berichte nennt Murillo und Oh, und Vlahović wird als nicht im Kader geführt.*
3. **Ein `t-online`-Treffer „Nullnummer gegen Bukarest: Hoffenheim tritt auf der Stelle — wieder kein Sieg unter Ilzer".** **Verworfen:** *passt zu keinem Spiel dieser Woche und stammt aus einer früheren Europapokalsaison.*
4. **Eine `bundesliga.com`-Vorschau mit Anstoß „Donnerstag 19:00" für Hoffenheim – Beşiktaş.** **Nicht verwendet:** *die Mehrheit und der Liveticker nennen 21:00. **Für den Tipp ohne Belang, aber ich schreibe die Abweichung hin.***
5. **Eine `hsv.de`-Pressekonferenz „Wir werden sehr viel verteidigen müssen" zu einem Spiel gegen Stuttgart.** **Verworfen:** *die Seite ist rund 188 Tage alt und betrifft ein Auswärtsspiel am 29. Spieltag der Vorsaison. **Derselbe Fallentyp wie an allen Vortagen: passender Titel, falsche Saison** — diesmal auf der offiziellen Vereinsseite.*
6. **Ein `nw.de`-Artikel „Paderborn muss gegen Werder auf ein Sextett verzichten".** **Verworfen:** *er betrifft ein DFB-Pokalspiel aus 2024.*
7. **`flashscore.de`-Übersicht „Bundesliga 6. Spieltag: Verletzungen und Sperren".** **Verworfen:** *die Seite stammt aus der Saison 2023/24.*
8. **`ligainsider.de`-Schlagzeilen „Widmer-Kaderplatz gegen Leverkusen noch offen" und „Vor Leverkusen: Fischer lässt Nebel-Comeback offen".** **Nicht als aktueller Stand verwendet:** *beide beziehen sich auf den **Leverkusen-Spieltag**, also den 5., nicht auf Schalke. **Deshalb bleibt meine Schwelle 1 zu Partie 2 heute unentschieden.***
9. **`kicker.de`-Spieltagsseite mit allen Teams bei 0 Punkten und eine `sport.de`-Tabelle über vier Spiele.** **Verworfen:** *Platzhalter bzw. veralteter Stand.*
10. **Eine Comunio-Prognoseelf für Gladbach, die Kleindienst in der Startelf führt.** **Nicht als Beleg verwendet:** *meine Schwelle 4 verlangt ausdrücklich „Startelf oder Kaderaufgebot, **nicht Prognose**". **Eine Medienprognose ist genau das, was dieser Zusatz ausschließt** — siehe Partie 9.*

---

## Offen benannte Restlücken

**Der Spieltag beginnt morgen.**

- **Keine offizielle Startelf und kein offizielles Kaderaufgebot zu einer der neun Bundesligapartien.** *Was vorliegt: fünf Spieltags-PKs, zwei veröffentlichte **voraussichtliche** Aufstellungen zu Frankfurt – Köln (`bundesliga.com`, Comunio), ein Kölner Reisekader in Zweitberichterstattung, Trainingsstandsberichte und drei Europapokal-Aufstellungen.*
- **Neuers Status für Samstag ist offen** — *keine Diagnose, keine Vereinsmeldung; die Entscheidung fällt nach dem Abschlusstraining am Freitag.*
- **Kleindiensts Einsatz am Sonntag ist offen** — *die endgültige Prognose kommt laut Bericht erst auf der Gladbacher PK am Freitag.*
- **Terriers Diagnose und Ausfalldauer sind unbekannt.** *Belegt ist nur die frühe Auswechslung in Posen.*
- **Rondics Diagnose ist nicht bestätigt** — *der Verein wollte sie auf Nachfrage nicht nennen.*
- **Musialas Rückkehr bleibt offen** (Muskelfaserriss, kein Datum).
- **Zu Werder – Paderborn existiert erstmals Material, aber keine Paderborner Verletztenliste aus dem Verein.** *Eine `ligainsider.de`-Seite nennt Hoffmeier, Klaas, Gayret und Awortwie-Grant im Aufbautraining — **undatiert, deshalb nur als Hinweis geführt, nicht als Stand.*** **Fünfter Tag ohne belastbare Paderborner Liste.**
- **Kein Spieltags-PK-Bericht zu Bayern, Leverkusen, Dortmund, Leipzig, HSV, Union, Hoffenheim, Freiburg, Paderborn.**
- **Kohrs Ausfalldauer bei Mainz bleibt strittig** (Ende Oktober gegen Anfang Januar 2027).
- **Widmers und Nebels Kaderstatus für Schalke ist unbekannt** (siehe verworfene Fundstelle 8).
- **Zu Beste (Freiburg) finde ich keinen Beleg in beide Richtungen.**
- **Keine Transfermeldung mit Spielrelevanz.**

---

## Die Tipps zum 6. Spieltag

**Die vier Regeln gelten unverändert weiter** und werden an jeder Partie geprüft:
**(1)** Eine Ausfallmeldung **ohne Angabe zur Ersatzlösung** verschiebt den Tipp nicht. **(2)** Die Tabellenposition der Heimmannschaft begründet keinen Auswärtstipp, solange keine partiebezogene Information dazukommt. **(3)** Kein einziger Zu-null-Tipp an diesem Spieltag. **(4)** Wenige, grob geschnittene Schwellen mit einander ausschließenden Zweigen.

### 1. Eintracht Frankfurt – 1. FC Köln
**Freitag, 16.10.2026, 20:30 Uhr**
**Tipp: 3:1**
***Änderung gegenüber gestern: 2:1 → 3:1, weil*** **Imad Rondic am Donnerstag im Training eine Muskelverletzung im Oberschenkel erlitten hat und damit ein dritter Kölner Angreifer ausfällt — Köln reist mit fünf Ausfällen plus dem langzeitverletzten Hübers, der Verteidiger Assad Kotya-Fofana steht erstmals im Kader, weitere Nachwuchsspieler reisen mit.** *Das ist der zweite Zweig meiner Schwelle 1, wörtlich: „neuer Kölner Ausfall mit genannter Ersatzlösung → 3:1". **Er ist heute erstmals ausgelöst, und zwar an genau der Stelle, an der ich ihn gestern ausdrücklich für nicht ausgelöst erklärt habe, weil die Ausfälle unbenannt waren.***

**Begründung:** **Frankfurt kommt vom 0:6 in Leipzig, hat mit 16 Gegentoren einen Vereinsnegativrekord und steht mit fünf Punkten auf Platz 14.** **Entscheidend ist die Kölner Personallage: neben Hübers (langzeitverletzt) fehlen Skhiri (Sprunggelenk, Wagner rechnet in diesem Kalenderjahr nicht mehr mit ihm), Dallinga, Ache, van den Berg (Muskelverletzung, heute bestätigt) und Rondic (heute).** **Damit fehlen drei Angreifer und zwei Innenverteidiger; die Bank ist nach den Berichten „extrem dünn".** **Die voraussichtliche Kölner Elf führt Simpson-Pusey und Lochoshvili als improvisiertes Innenverteidigerpaar, Krauß und Johannesson im Zentrum als Skhiri-Ersatz.**

**Auf Frankfurter Seite ist heute erstmals eine Elf veröffentlicht, und sie löst die Sturmfrage von gestern:** **`bundesliga.com` erwartet Atubolu im Tor, Collins, Koch, Brassier und Kosugi in der Abwehr und ***Burkardt und Ebnoutalib gemeinsam*** im Sturm.** *Gestern hatte Hütter die Doppelspitze nur als Option genannt — **heute ist sie die erwartete Variante, und das ist das dritte Frankfurter Tor.*** **Koch führt die Mannschaft als Kapitän auf den Platz** (zweiter Tag belegt). **Bei Frankfurt fehlen Ngankam und Pimpong.**

**Warum Köln trotzdem trifft:** **Köln hat in jedem der fünf Ligaspiele mindestens ein Tor erzielt, und Frankfurt lässt zwei pro Spiel zu.** *Regel 3 verbietet das Zu-null ohnehin.* ***Ehrlich: das ist mein aggressivster Tipp des Spieltags.*** *Frankfurt hat 9 Tore in fünf Spielen erzielt, also 1,8 pro Spiel — **drei Tore sind eine Aufrundung nach oben, die ich allein mit der Kölner Abwehrimprovisation und der Doppelspitze begründe.** Ich setze sie unten als Schwelle zur Rücknahme.* **Keine der beiden Mannschaften spielt international.**

### 2. FC Schalke 04 – 1. FSV Mainz 05
**Samstag, 17.10.2026, 15:30 Uhr** (Veltins-Arena)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Der Offensivunterschied bleibt der größte belegte Einzelwert: Mainz 13 Tore in fünf Spielen, Schalke 5 — die schwächste Offensive der Liga.** **Mainz ist auswärts ungeschlagen und zu Hause sieglos; Urs Fischer nennt zehn Gegentore in den letzten drei Bundesligaspielen und fehlende „Abstände und Kompaktheit".** **Der direkte Vergleich spricht für Schalke: 32 Bundesligaspiele, 19 Schalker Siege, 7 Remis, 6 Mainzer Siege, 48:26 Tore.**

***Die wichtigste neue Information des Tages dreht die Lage von gestern um — und zwar gegen Schalke:*** **Moussa Sylla fällt aus.** **Der Stürmer hat sich im Spiel bei Freiburg am linken Bein verletzt, der Verein nennt weder Diagnose noch Ausfalldauer.** **Sylla hatte vier der fünf Ligaspiele begonnen und galt als erste Wahl vor Edin Džeko** — *damit ist die Ersatzlösung in der Berichterstattung benannt, Regel 1 ist erfüllt.* **Dazu fehlen Højlund (nach Ferseneingriff) und Ljubičić (Knie, Kaderplatz offen).**

***Warum der Tipp trotzdem exakt gleich bleibt, und das ist diesmal eine Rechnung, keine Trägheit:*** *Gestern habe ich diese Partie als „die mit der größten unverarbeiteten Gegeninformation" benannt — **fünf bis sechs Mainzer Ausfälle, die für 1:1 sprachen.** Heute kommt auf der anderen Seite der Ausfall des Schalker Torjägers hinzu. **Die beiden Entwicklungen heben sich auf, und der Tipp steht nach meiner Einschätzung heute fester als gestern, nicht gleich fest.*** **Das Schalker Tor bleibt stehen, weil Mainz in drei Spielen zehn Gegentore kassiert hat und Muslić ausdrücklich an seiner Defensivanlage festhält.**

**Schwelle 1 geprüft — unentschieden, und ich sage warum:** *Sie verlangte ein **Mainzer** Kaderaufgebot ohne Widmer, Nebel und Kohr (→ 1:1) oder einen Beleg für Widmers oder Nebels Einsatz (→ 1:2 ohne weitere Prüfung). **Die beiden Fundstellen, die ich zu Widmer und Nebel finde, beziehen sich auf den Leverkusen-Spieltag, nicht auf Schalke** (verworfene Fundstelle 8). **Kein Zweig ausgelöst, weil die Information fehlt — nicht, weil sie gegen die Zweige spricht.*** **Als Starter im Tor wird Alexander Schwolow erwartet, der etatmäßige Zweite.** **Keine der beiden Mannschaften spielt international.**

### 3. SV 07 Elversberg – FC Augsburg
**Samstag, 17.10.2026, 15:30 Uhr** (Ursapharm-Arena)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Augsburg hat an allen fünf Spieltagen mindestens zwei Tore erzielt** und **dem Dritten Bayern einen Punkt abgenommen** (2:2). **Elversberg kommt von der 0:1-Niederlage in Berlin, hat 8 Tore in fünf Spielen und als Aufsteiger sieben Punkte.**

**Die Personallage ist heute auf beiden Seiten aus der PK belegt, und sie bestätigt den Tipp, ohne ihn zu bewegen:** **Manuel Baum meldet Marius Wolf fit und wieder dabei** — *gestern stand er „vor der Rückkehr ins Training", heute ist er für Elversberg eingeplant.* **Noahkai Banks fehlt mit Außenbandverletzung im Knie, Baum nennt „zwei, drei, vier Wochen mindestens"; Alexis Claude-Maurice fehlt mit Muskelverletzung.** *Beide Namen standen gestern schon auf meiner Liste, heute sind sie datiert und mit Diagnose belegt — **das ist Präzisierung, keine Torveränderung** (beide sind Defensivspieler, und für keinen ist eine Ersatzlösung benannt, Regel 1).*

**Vincent Wagner hat die Elversberger Linie selbst beschrieben** („Wir versuchen, den Ball weiter wegzuschießen als Manuel Neuer" — Anspielung auf Neuers Fehler vor dem schnellsten Tor der Bundesligageschichte, das Augsburg erzielte). *Auf die Frage, was Augsburg vergessen könne, sagte er, es wäre schön, wenn sie einen Punkt vergäßen.* **Elversbergs Lage im Übrigen unverändert: Gyamerah einsatzbereit, Startelfplatz offen, Sirch als Vertreter gelobt; Onyeka ohne Rückkehrdatum, Seifert länger, Zimmerschied einige Wochen.** **Keine der beiden Mannschaften spielt international.**

### 4. SV Werder Bremen – SC Paderborn 07
**Samstag, 17.10.2026, 15:30 Uhr** (Weserstadion, 100. Geburtstag)
**Tipp: 2:1**
***unverändert***

**Begründung:** **Der klarste Formunterschied des Spieltags: Niclas Füllkrug steht bei vier Saisontoren, ist der einzige Spieler der Saison mit zwei Kopfballtoren und hat in Dortmund in der 90.+2 per Kopf ausgeglichen.** **Paderborn hat mit 3 Toren in fünf Spielen die schwächste Offensive der Liga und verlor zu Hause 0:2 gegen Stuttgart.**

***Gestern war dies die Partie, zu der ich „nichts Neues überhaupt" gefunden habe. Heute ist sie die mit der längsten Ausfallliste:*** **acht Werder-Profis fehlen gegen Paderborn** — **Agu, Stage, Njinmah, Musah, Alvero (alle muskulär), Lynen (Beckenprobleme), Ndiaye (Leiste) und Topp (Kreuzbandriss).** ***Das deckt sich mit dem Stand von gestern („17 Feldspieler und vier Torhüter"), ist aber erstmals namentlich auflösbar — und es ist, anders als es aussieht, keine Verschlechterung: es sind weitgehend dieselben Ausfälle, unter denen Werder acht Punkte geholt hat.***

**Die beiden neuen Nachrichten gehen in verschiedene Richtungen und heben sich auf:** **Amos Pieper, in Dortmund früh ausgewechselt, ist zurück** — Thioune: „Aktuell gehe ich davon aus, dass er uns zur Verfügung stehen wird und dann auch sofort wieder ein Startelf-Kandidat ist." **Mitchell Weiser ist dagegen „wohl noch kein Startelf-Kandidat"**, Thioune sieht „jetzt gerade keinen Grund, irgendwelche Wechsel vorzunehmen". *Ein zurückkehrender Innenverteidiger und ein nicht startender Außenbahnspieler sind zusammen keine Torveränderung.*

**Warum nicht 2:0:** **Werder hat 10 Gegentore in fünf Spielen** — *gegen eine Abwehr, die zwei pro Spiel zulässt, überwiegt „ein Paderborner Tor", und Regel 3 verbietet das Zu-null ohnehin.* **Zu Paderborn selbst habe ich zum fünften Tag keine belastbare Verletztenliste; belegt ist heute nur der Trainer (Kettemann).** **Keine der beiden Mannschaften spielt international.**

### 5. 1. FC Union Berlin – Borussia Dortmund
**Samstag, 17.10.2026, 15:30 Uhr** (An der Alten Försterei)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Der größte Tabellenabstand des Spieltags: Dortmund 13 Punkte und 11:4, Union 4 Punkte und 5:17 — die schlechteste Tordifferenz der Liga nach Gladbach.** **Der direkte Vergleich: 16 Pflichtspiele, elf Dortmunder Siege, vier für Union, ein Remis.** **Die Rotation hat belegt in Bodø stattgefunden, nicht in Berlin; Julian Ryerson ist nach seinem Ausfall gegen Bremen wieder eine Option für die erste Elf.**

***Schwelle 2 geprüft — und das ist die schwierigste Entscheidung dieses Laufs, deshalb schreibe ich sie vollständig hin.*** *Die Schwelle verlangte für **1:3**, dass belegt wird, dass Schlotterbeck **in Berlin spielt** — „Startelf, Kaderaufgebot **oder Kovač-Aussage auf einer Spieltags-PK**" — **und** dass Unions Ausfallliste unverändert ist.
- **Was heute vorliegt:** **Sportdirektor Lars Ricken hat am Flughafen gesagt, Schlotterbeck werde „bei Union Berlin dann auch wieder dabei sein"**, und **`bvb.de` nennt als Grund für das Fehlen in Bodø ausdrücklich Belastungssteuerung, also keine Verletzung.** **Unions Liste ist unverändert** (Markgraf, Ilić, Juranović, Friedrich, N'Soki, Burke; keine neue Meldung).
- **Warum ich die Schwelle trotzdem als nicht ausgelöst führe:** *Ricken ist **keiner der drei genannten Kanäle**, und seine Aussage fiel **vor** dem Bodø-Spiel am Flughafen — sie ist damit eine **Erwartung**, nicht ein Vollzug. **Genau diese Art Aussage schließe ich in Partie 9 bei Kleindienst als „Prognose" aus. Wenn ich sie hier als Beleg nähme, wendete ich zwei Maßstäbe an zwei Partien an.***
- ***Was ich dazu offenlegen muss:*** *Das ist der **zweite Tag in Folge, an dem ich eine Schwelle am Wortlaut scheitern lasse, während die Sache in der Substanz näher dran ist** (gestern Neuer, heute Schlotterbeck). **Beim dritten Mal wäre es ein Formulierungsproblem und kein Befund** — deshalb fasse ich die Schwelle unten neu und benenne den Freitag (Dortmunder Spieltags-PK) als Entscheidungstag.
- **Der Gegenzweig (2:2) ist ebenfalls nicht ausgelöst, aber knapper als gestern:** **Kovač hat nach der Niederlage seine Startelf selbst für falsch erklärt** („Startelf auf dem Prüfstand") und warnt: „Bei Union erwartet uns ja ein ähnliches Spiel. Da können wir auch davon ausgehen, dass die Post abgeht." *Berichte erwarten Änderungen auf mehreren Positionen (Nmecha, Guirassy, Nwaneri, Ryerson). **Das ist aber das Gegenteil der Schonrotation, auf die der Zweig gebaut war: Kovač holt Stammspieler zurück, er stellt sie nicht frei.*** **Ein Innenverteidiger-Ausfall mit Ersatzlösung liegt nicht vor.*

**Unions Lage, heute mit Trainerzitat:** **Lustrinelli setzt auf Kontinuität — „Ich gehe davon aus, dass wir nicht viele Wechsel vornehmen werden"; als Innenverteidigerpaar werden Uduokhai und van den Bosch erwartet, Kemlein ist kein Stammspieler mehr.** **Union hat zuletzt 1:0 gegen Elversberg seinen ersten Saisonsieg geholt — zu Hause und ohne Gegentor** — *und an der Alten Försterei habe ich am 5. Spieltag genau einen Tipp verloren.* ***Deshalb bleibt es beim Union-Tor, und deshalb ist 1:3 auch sachlich nicht so naheliegend, wie die Tordifferenz aussieht.***

### 6. Hamburger SV – VfB Stuttgart
**Samstag, 17.10.2026, 15:30 Uhr** (Volksparkstadion)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Beide stehen bei 6 Punkten, der Unterschied liegt in der Abwehr: HSV 15 Gegentore in fünf Spielen, Stuttgart 9.** **Die Heimbilanz des HSV ist die schwächste Teilbilanz dieses Spieltags: drei Punkte und 2:6 Tore aus drei Heimspielen** — *zwei erzielte Tore in drei Heimspielen, und darauf steht das eine HSV-Tor.*

**Das Mittwochsergebnis ist jetzt vollständig belegt und spricht für Stuttgart: 3:0 in Bratislava, Undav (29.) hat seine Torflaute beendet, Demirović (90.) steht bei vier Toren in dieser Champions-League-Saison.** *Mein Vorbehalt von gestern gegen den Endstand ist aufgelöst (Korrektur 1).*

***Die Gegeninformation ist heute größer als gestern, und sie betrifft Stuttgarts Abwehr:*** **Hoeneß hat auf der PK gesagt, dem VfB gehen die fitten Innenverteidiger aus — Al-Dakhil ist noch nicht im Mannschaftstraining, Zagadou braucht Zeit; positive Signale gibt es bei Luca Jaquez.** **Mittelstädts Aussichten für Samstag sind „derzeit eher gering" (genähte Risswunde an der Ferse), Chabot steht nach den muskulären Beschwerden wieder zur Verfügung.** **Zwischen Bratislava und Hamburg liegen drei Tage.** *Ich lasse den Tipp stehen, weil der HSV die Lücke nicht nutzen kann: **Grønbæk fehlt belegt (Muskelfaserriss, Comeback frühestens 24.10.), Daka kommt das Duell „wohl zu früh", Jatta und Lokonga sind laut Vorbericht fraglich, Kapitän Remberg fehlt nach Kreuzbandriss über Monate.*** **Zu Nadir und El Ouahdi bleibt es bei „hängt vom Trainingsverlauf ab" — Meldungen vom Donnerstagstraining habe ich nicht gefunden, nach Regel 1 rechne ich sie deshalb nicht in ein Tor um.**

### 7. FC Bayern München – RB Leipzig
**Samstag, 17.10.2026, 18:30 Uhr**
**Tipp: 2:1**
***unverändert***

**Begründung:** **Bayern hat mit 16:4 die beste Offensive der Liga und ist in der Bundesliga ungeschlagen, hat aber zwei der fünf Spiele unentschieden gespielt.** **Leipzig kommt vom 6:0 gegen Frankfurt und vom 1:0 gegen PSV und hat mit 5 Gegentoren die zweitbeste Abwehr der Liga.** *Rechnerisch komme ich für Bayern auf etwa zwei, für Leipzig auf etwa ein Tor.* **Leipzigs Trainer ist Martín Demichelis** (neu belegt, Korrektur 5).

***Die Neuer-Lage hat sich verschärft, ohne die Schwelle zu erfüllen:*** **Neuer hat am Donnerstag im Mannschaftstraining gefehlt und im Leistungszentrum gearbeitet; mehrere Berichte titeln „wohl nicht fit" und „Leipzig-Spiel in Gefahr"; die Entscheidung fällt nach dem Abschlusstraining am Freitag.** **Urbig stünde bereit, es wäre sein vierter Saisoneinsatz.**

**Schwelle 3 geprüft — nicht ausgelöst, und zwar an der zweiten Bedingung:** *Die neue Fassung von gestern verlangte **Neuers Ausfall belegt** (Vereinsmeldung oder Kaderaufgebot) **und zusätzlich einen Feldspieler-Ausfall mit benannter Ersatzlösung** → 2:2. **Belegt ist Neuers Ausfall nicht — „wohl nicht fit" ist eine Einschätzung, und der Verein hat sich nicht geäußert.** **Und der Feldspieler-Teil fehlt ebenfalls: neu auf der Liste steht Tarek Buchmann (verletzt), aber ohne benannte Ersatzlösung und nicht als Stammspieler.** *Musiala fehlt weiter, ein Rückkehrdatum ist nicht genannt — der 3:1-Zweig ist nicht ausgelöst.* **Dass ein Torwartwechsel auf Urbig allein nichts auslöst, ist meine gestrige Festlegung nach der Schwolow-Logik, und ich halte sie.*

**Personalien im Übrigen:** **Bei Bayern fehlen Musiala und Buchmann verletzt, Laimer wegen Vaterfreuden.** **Olises Gelb-Rot aus Stavanger sperrt für das nächste Europapokalspiel, nicht für die Bundesliga** — *dritter Tag, weil es die naheliegende Fehlschlussquelle dieser Partie ist.* **Bei Leipzig fehlen Baumgartner, Ouédraogo, Guiu und Gebel; Sperren gibt es auf keiner Seite.** ***Zu dieser Partie gibt es auch heute keinen Spieltags-PK-Bericht.***

### 8. Bayer 04 Leverkusen – SC Freiburg
**Sonntag, 18.10.2026, 15:30 Uhr**
**Tipp: 3:2**
***Änderung gegenüber gestern: 2:2 → 3:2, weil*** **Ibrahim Maza in Posen in der Startelf stand und in der 89. Minute getroffen hat — damit ist er belegt Starter und nicht mehr „unsicher", wie er auf meiner Liste seit vier Tagen stand.** *Das ist wörtlich der zweite Zweig meiner Schwelle vom 11.10.: „Wird Maza belegt als Starter geführt, gehe ich auf 3:2." **Der erste Zweig (3:1) ist ausdrücklich nicht ausgelöst — er verlangte eine Freiburger Startelf, in der neben Suzuki mindestens zwei weitere der erwarteten Stammspieler fehlen, und die veröffentlichte Elf zeigt das Gegenteil.***

**Begründung:** **Das Spitzenspiel des Spieltags: Vierter gegen Ersten, 14:8 gegen 14:4.** **Patrik Schick führt die Torjägerliste an und hat in Posen zweimal getroffen; Leverkusen hat mit 4:0 den souveränsten deutschen Europapokalabend der Woche hingelegt.** **Freiburg ist ungeschlagen, steht bei einem Vereinsrekord von 13 Punkten und ist nun neun Pflichtspiele unbesiegt.**

***Die drei neuen Tatsachen, die das dritte Leverkusener Tor tragen:***
1. **Freiburg hat am Donnerstag 21:00 mit fast der ersten Elf gespielt** — Backhaus; Kübler, Ginter, Rosenfelder, Günter; Eggestein, Osterhage; Irié, Suzuki, Grifo; Höler. **Eine einzige Änderung gegenüber der erwarteten Elf (Höler für Matanović).** *Schuster hatte Rotation offengelassen und sie dann über Einwechslungen gelöst.* **Dazu acht Spiele in 25 Tagen bis zur Länderspielpause.**
2. **Leverkusen hat drei Stunden früher gespielt und vorher rotiert:** **Andrich und Quansah pausierten, Vázquez und Ezequiel Fernández begannen, Schick sollte geschont werden.**
3. **Suzuki hat am Donnerstag gespielt, fehlt aber am Sonntag:** **seine Gelb-Rote Karte gegen Schalke sperrt nur in der Bundesliga.** ***Freiburg verliert damit belegt einen Torschützen mit vier Saisontoren aus einer Mannschaft, die 90 Minuten in den Beinen hat.***

***Was gegen die Änderung spricht, und ich schreibe es hin, weil es ernst ist:*** *Leverkusens Rotationsplan ist aufgegangen und gleichzeitig zerbrochen — **Martin Terrier hat sich früh verletzt, Schick kam in der 18. Minute und spielte etwa 57 Minuten statt null.** **Zu Terriers Diagnose gibt es keine Meldung, zu seiner Ausfalldauer nichts.** *Dazu die Rückreise aus Polen.* **Leverkusens Ausfallliste ist ohnehin die längere: Kofane (Muskelfaserriss), Eichhorn, Ben Seghir (Muskelverletzung), Doué (Wade), Boniface und Culbreath (Trainingsrückstand) — plus nun Terrier.** ***Ich bleibe bei der Änderung, weil der Schick-Einsatz ein Vorteil in der Form und ein Nachteil in der Frische ist, der Suzuki-Ausfall aber ein reiner Verlust — und weil die Schwelle, an die ich mich gebunden habe, eindeutig ausgelöst ist.***

**Das zweite Freiburger Tor bleibt:** **Freiburg hat 14 Tore in fünf Spielen erzielt und am Donnerstag selbst zwei kassiert.** **Freiburgs Ausfälle: Muslija (Kreuzbandriss, langfristig) und Yılmaz (nach Zahnoperation); Osterhage ist entgegen meinem Vortagsstand einsatzfähig** (Korrektur 2).

### 9. Borussia Mönchengladbach – TSG Hoffenheim
**Sonntag, 18.10.2026, 17:30 Uhr**
**Tipp: 1:1**
***unverändert*** — *die Änderung vom 12.10. (2:1 → 1:1) hält den vierten Tag.*

**Begründung:** **Letzter gegen Siebzehnten, und beide stehen unter Druck.** **Für Gladbach ist es das erste Heimspiel unter Blessin nach der 1:2-Derbyniederlage in Köln.** **Hoffenheim hat nun vier Pflichtspielniederlagen in Folge.**

***Die halbe Schwelle ist heute erfüllt — und genau das ist der Grund, warum der Tipp steht:*** **Hoffenheim hat am Donnerstag 2:3 gegen Beşiktaş verloren** (Murillo 60., Asllani 68., Oh 72. und 79., Machida 87.), **vor mehr als 10.000 türkischen Gästefans in Sinsheim, nach 0:0 zur Pause.** **Kapitän Baumann: „zu wenig Punkte für die Leistung."** *Mein dritter Zweig verlangte: **Hoffenheim verliert am Donnerstag und Kleindienst steht belegt im Kader → 2:1.*** **Die erste Bedingung ist erfüllt, die zweite nicht:** **Kleindienst hat am Mittwoch nach rund 35 Minuten erneut abgebrochen (Verband am Oberschenkel), und die endgültige Einsatzprognose gibt Blessin erst auf der Pressekonferenz am Freitag.** **Eine Comunio-Prognoseelf führt ihn in der Startelf — das ist ausdrücklich das, was meine Schwelle als „nicht Prognose" ausschließt** (verworfene Fundstelle 10).

**Was heute neu und belegt ist, auf beiden Seiten:** **Nicolas Kühn hat die komplette Einheit absolviert; Blessin: „Wenn er gut durch die Woche kommt, wäre es möglich, dass er am Sonntag wieder im Kader steht" — eher als Joker denn in der Startelf.** *Das ist die erste gute Gladbacher Personalnachricht seit Tagen und der Grund, warum ich das Gladbacher Tor nicht streiche.* **Weiter fehlen Itakura und Honorat (muskulär) sowie die Langzeitverletzten Castrop und Enzo Leopold; Torwart Moritz bleibt laut Blessin die Nummer eins.** **Bei Hoffenheim fehlt Hajdari (Plantarfaszie) für „die nächsten Wochen", von Ilzer ausdrücklich mit Bezug auf dieses Spiel benannt.**

**Schwelle 4 geprüft — kein Zweig ausgelöst:** *Erster Zweig (**Kleindiensts Einsatz belegt bestätigt** → 2:1): nicht ausgelöst, es gibt nur eine Prognose. Zweiter Zweig (**sein Ausfall belegt bestätigt** → bleibt 1:1): ebenfalls nicht, „fraglich" ist nicht „bestätigt". Dritter Zweig: **zur Hälfte erfüllt.*** ***Der 0:1-Zweig, den ich „solange Hoffenheim Donnerstag spielt" nicht geprüft habe, ist jetzt prüfbar — und das Ergebnis spricht dagegen: eine Mannschaft, die Donnerstag um 21:00 zu Hause verloren hat, 2:5 in der Ligaphase steht und Sonntag um 17:30 reisen muss, ist kein Kandidat für einen Auswärtssieg zu null.***

**Was gegen meinen Tipp spricht:** ***Gladbach hat null Punkte aus fünf Spielen und mit 18 Gegentoren die schlechteste Abwehr der Liga*** — *gegen diese Abwehr ist ein Hoffenheimer Sieg jederzeit möglich, Belastung hin oder her, und Asllani und Machida haben am Donnerstag beide getroffen.* *Nach Regel 2 werte ich Gladbach nicht wegen der Tabellenposition ab; die Abwertung vom 12.10. beruhte auf der Personalinformation, und die gilt heute mit Kühns Rückkehr einen Hauch schwächer als gestern.*

---

## Verteilung und Selbstkontrolle

| Partie | Anstoß | Tipp | Vergleich | Europapokal in der Woche |
|---|---|---|---|---|
| Frankfurt – Köln | Fr 20:30 | **3:1** | **geändert von 2:1** | — / — |
| Schalke – Mainz | Sa 15:30 | **1:2** | unverändert | — / — |
| Elversberg – Augsburg | Sa 15:30 | **1:2** | unverändert | — / — |
| Werder – Paderborn | Sa 15:30 | **2:1** | unverändert | — / — |
| Union – Dortmund | Sa 15:30 | **1:2** | unverändert | — / **Mi auswärts 0:1** |
| HSV – Stuttgart | Sa 15:30 | **1:2** | unverändert | — / **Mi auswärts 0:3** |
| Bayern – Leipzig | Sa 18:30 | **2:1** | unverändert | **Di auswärts 3:3** / **Di heim 1:0** |
| Leverkusen – Freiburg | So 15:30 | **3:2** | **geändert von 2:2** | **Do auswärts 4:0** / **Do heim 3:2** |
| Gladbach – Hoffenheim | So 17:30 | **1:1** | unverändert | — / **Do heim 2:3** |

**Verteilung:** **4 Heimsiege, 4 Auswärtssiege, 1 Unentschieden** — *gestern 3/4/2.* **Kein Zu-null-Tipp** (Regel 3 eingehalten). **30 Tore in neun Partien, 3,33 pro Spiel** — *gestern 27 und 3,0.* ***Das ist die Nebenwirkung beider Änderungen: ich tippe heute offensiver als an jedem Tag dieser Woche, und beide Male geht das Plus auf das Konto der Heimmannschaft.***

**Anstoßzeiten:** **unverändert gegenüber dem mehrfach gegenbestätigten Stand von gestern.** *Zwei Abweichungen, beide verworfen: eine Fundstelle ordnet Union – Dortmund dem Sonntag 17:30 zu (das ist Gladbach – Hoffenheim), eine `bundesliga.com`-Seite nennt für Samstag „Mainz – Leverkusen" (das ist der 5. Spieltag).* **Ich bleibe bei: Fr 20:30 Frankfurt – Köln; Sa 15:30 Schalke – Mainz, Elversberg – Augsburg, Werder – Paderborn, Union – Dortmund, HSV – Stuttgart; Sa 18:30 Bayern – Leipzig; So 15:30 Leverkusen – Freiburg; So 17:30 Gladbach – Hoffenheim.**

***Zur Selbstkontrolle: nach zwei Tagen mit neunmal „unverändert" heute zwei Änderungen — woran liegt der Unterschied?*** **Mein Befund: an der Art der Information, nicht an ihrer Menge.** *An den Vortagen kamen Trainernamen, Diagnosen und Trainingsberichte — Dinge, die den Kontext schärfen. **Heute kamen drei gespielte Spiele mit Aufstellungen und ein veröffentlichter Reisekader. Das sind Belege der Art, auf die meine Schwellen ausdrücklich gebaut sind** („Startelf, Kaderaufgebot"), und entsprechend haben zwei von vier ausgelöst.* **Vier Stellen, an denen ich heute zusätzlich hätte ändern können, und warum ich es nicht getan habe:**

1. ***Union – Dortmund auf 1:3.*** **Rickens Zusage zu Schlotterbeck plus unveränderte Unionsliste.** *Nicht getan, weil Ricken keiner der drei von mir benannten Kanäle ist und seine Aussage vor dem Bodø-Spiel fiel — **und weil ich in Partie 9 am selben Tag eine Prognose aus genau diesem Grund ablehne.*** ***Das ist die wahrscheinlichste Fehlstelle dieses Laufs.***
2. ***Schalke – Mainz auf 1:1.*** **Sechs Mainzer Ausfälle.** *Nicht getan, weil heute der Ausfall des Schalker Torjägers Sylla dazukam und beide Seiten sich aufheben. **Gestern war das meine benannte Hauptfehlstelle — heute ist sie es nicht mehr, und das ist der Grund.***
3. ***Gladbach – Hoffenheim auf 2:1.*** **Hoffenheim hat Donnerstag verloren, reist Sonntag, Kühn ist zurück.** *Nicht getan, weil die zweite Hälfte meiner eigenen Bedingung (Kleindienst belegt im Kader) nicht erfüllt ist. **Die Gladbacher PK am Freitag entscheidet das.***
4. ***HSV – Stuttgart auf 2:2.*** **Stuttgart gehen die Innenverteidiger aus, drei Tage nach Bratislava.** *Nicht getan, weil der HSV mit Grønbæk, Daka, Remberg und wahrscheinlich Jatta und Lokonga keine Mannschaft ist, die diese Lücke bestraft.*

**Wenn dieser Lauf falsch ist, ist er mit hoher Wahrscheinlichkeit an Stelle 1 falsch — oder an der neuen 3:1-Aufrundung in Partie 1.**

**Die vier Schwellen für die nächsten Läufe — eine neu, eine neu gefasst, zwei fortgeführt:**

1. **Frankfurt – Köln (neu, zur Rücknahme der heutigen Änderung):** *Wird ein Frankfurter Kaderaufgebot oder eine Startelf veröffentlicht, in der **Burkardt und Ebnoutalib nicht gemeinsam** beginnen, gehe ich auf **2:1** zurück. Wird ein Kölner Aufgebot veröffentlicht, in dem **van den Berg oder Rondic doch dabei** sind, ebenfalls 2:1. **Die Partie beginnt Freitag 20:30 — das ist der letzte Lauf, der sie überhaupt erreicht.***
2. **Union – Dortmund (neu gefasst, weil die alte Fassung zum zweiten Mal am Kanal gescheitert ist):** *Wird Schlotterbecks Einsatz in Berlin durch **Startelf, Kaderaufgebot, Kovač auf der Spieltags-PK oder eine Meldung auf `bvb.de`** belegt — **vier Kanäle statt drei, und die Vereinsseite zählt jetzt mit** — **und** ist Unions Ausfallliste unverändert, gehe ich auf **1:3**. Wird ein Dortmunder Innenverteidiger-Ausfall **mit genannter Ersatzlösung** gemeldet, gehe ich auf 2:2. **Eine Rotationsankündigung allein löst nichts mehr aus: Kovač hat seine Startelf selbst für falsch erklärt, Änderungen sind also eher Rückkehr als Schonung.***
3. **Bayern – Leipzig (fortgeführt, unverändert im Wortlaut):** *Wird **Neuers Ausfall für Samstag belegt** (Vereinsmeldung oder Kaderaufgebot) **und** zusätzlich ein **Feldspieler**-Ausfall mit benannter Ersatzlösung gemeldet, gehe ich auf **2:2**. Allein ein Torwartwechsel auf Urbig löst nichts aus. Kündigt Kompany eine Rotation belegt an, gehe ich ebenfalls auf 2:2. Wird Musialas Rückkehr belegt gemeldet (Kaderaufgebot, nicht Prognose), gehe ich auf 3:1. **Das Abschlusstraining am Freitag ist die Gelegenheit.***
4. **Gladbach – Hoffenheim (fortgeführt):** *Wird Kleindiensts Einsatz belegt bestätigt (Startelf oder Kaderaufgebot, **nicht Prognose**), gehe ich auf **2:1**. **Die Gladbacher PK am Freitag ist dafür die benannte Gelegenheit** — und da Hoffenheims Donnerstagsniederlage jetzt feststeht, **genügt ab sofort der Kleindienst-Beleg allein, um den dritten Zweig vollständig zu machen.** Wird sein Ausfall bestätigt, bleibt 1:1. **0:1 ist nach der Donnerstagsniederlage und der Sonntagsreise vom Tisch.***

**Was dieser Lauf geleistet hat:** **zwei Tipps aus pre-committed Schwellen heraus geändert, nicht aus dem Bauch** · **vier offene Lücken geschlossen** (Kölns zwei unbenannte Ausfälle, Leipzigs und Paderborns Trainer, Bratislava-Endstand) · **die Trainerliste erstmals auf 18 von 18 gebracht** · **Freiburgs strittiges Torverhältnis aufgelöst und die eigene Tabelle erstmals von außen gegenbestätigt** · **alle drei Donnerstagsspiele mit Torfolge und Aufstellung erfasst und für die Partien 8 und 9 ausgewertet** · **fünf Spieltags-PKs ausgewertet (nach zwei gestern)** · **einen eigenen Übervorsichtsfehler korrigiert (Bratislava-Endstand) und einen Listenfehler (Osterhage)** · **Syllas Ausfall gefunden und gegen die Mainzer Ausfallliste gerechnet, wodurch die gestrige Hauptfehlstelle entfallen ist** · **die Schlotterbeck-Entscheidung vollständig offengelegt statt sie in einem Halbsatz zu entsorgen, und die Schwelle daraufhin um einen Kanal erweitert** · **zehn Fundstellen geprüft und verworfen**, darunter eine 188 Tage alte Pressekonferenz auf einer offiziellen Vereinsseite und eine Rotationsangabe, die Partie 8 in die falsche Richtung gedreht hätte.

**Was dieser Lauf nicht geleistet hat:** **kein Volltext einer einzigen Quelle — die Hosts sind durch die Netzwerk-Policy gesperrt, fünfter Tag, und `WebFetch` scheitert zusätzlich an der Namensauflösung; das ändert sich nur durch den Nutzer** · **keine offizielle Startelf und kein offizielles Kaderaufgebot zu einer der neun Partien** · **keine belastbare Paderborner Verletztenliste, fünfter Tag** · **kein Spieltags-PK-Bericht zu neun der achtzehn Vereine** · **Neuers Status, Kleindiensts Status, Terriers Diagnose und Rondics Diagnose alle offen** · **Widmers und Nebels Kaderstatus unbekannt** · **Kohrs Ausfalldauer widersprüchlich** · **zu Beste (Freiburg) kein Beleg in beide Richtungen** · **Demichelis und Kettemann nur aus Quellen vom Juni bzw. August 2026 belegt.**

---

## Quellen

**Alle Fundstellen stammen aus Suchergebnis-Zusammenfassungen und -Titeln. Kein Volltext — siehe Hinweis zur Quellenlage.**

**Donnerstagsspiele (neu):** `t-online.de` („Bayer Leverkusen siegt, doch Terrier verletzt sich"; Liveticker Posen) · `oldenburger-onlinezeitung.de`, `nachrichten-heute.net`, `ad-hoc-news.de` („Leverkusen schlägt Lech Posen mit 4:0") · `fussballnationalmannschaft.net` (Ergebnis- und Aufstellungsseiten Posen, Hoffenheim, Freiburg) · `baykusen.de` (Aufstellung Posen) · `tagesspiegel.de` und `kurier.de` (dpa, „Beşiktaş übertönt und besiegt Hoffenheim") · `sportschau.de`/SWR („Nächste Pleite"; „Freiburg auch international im Flow") · `nau.ch` und `wz.de` (Hoffenheim 2:3) · `skysportaustria.at` (Baumann-Stimmen) · `zdfheute.de` („Freiburg löst Pflichtaufgabe souverän") · `schwarzwaelder-bote.de` (Schusters 100. Spiel) · `breisgau.live` · `bulinews.com` („Confirmed Lineups: SC Freiburg vs. FK Jablonec") · `allfootballapp.com`

**Bratislava-Endstand (Lücke geschlossen):** `bundesliga.com` (Spielbericht Spieltag 2) · `sportschau.de` („Kurs K.o.-Runde") · `zdf.de` (Zusammenfassung) · `vfb.de` · `eurosport.de` (Liveticker, „Undav trifft") · `espn.com` (401915405, „S Bratislava 0-3 Stuttgart") · `sportinglife.com` (Kommentar zum Demirović-Tor) · `ad-hoc-news.de` („Undav beendet Torflaute")

**Pressekonferenzen (neu):** `recklinghaeuser-zeitung.de` („Schalke-PK vor Mainz in voller Länge") und `reviersport.de` („Die werden sich fetzen") sowie `absolutfussball.com` („Muslić bleibt trotz Ladehemmung stur") · `rhein-zeitung.de` und `nw.de` („Zu jung oder zu alt? Fischer schmunzelt") · `sport1.de` („Fischer über Gegentore: Ist mir zu negativ") · `deichstube.de` („Werder hofft auf Weserstadion-Party"; „Acht Profis fallen aus") und `weser-kurier.de` (Weiser, Pieper) und `aol.de` (Highlights der Werder-PK) · `wochenblatt-reporter.de` („Neuer-Seitenhieb bei Elversberg") und `schwaebische.de`/`lokalo.de`/`frankenpost.de` (dpa, Wagner) · `sport1.de` (Baum nach dem Bayern-Spiel) und `tv-mittelrhein.de` (dpa, „Augsburg in Elversberg wieder mit Wolf") · `vfb.de` und `ligainsider.de` (Hoeneß zu Mittelstädt, „von Tag zu Tag") und `tipico.de` (Chabot, Innenverteidigung)

**Köln und Frankfurt (Lücke geschlossen):** `koeln.t-online.de` („Ausfall bestätigt: Verteidiger verpasst Frankfurt-Spiel", van den Berg) · `geissblog.koeln` („Nächste Muskelverletzung: Stürmer fällt aus, Talent mit Kader-Debüt", Rondic/Kotya-Fofana) · `come-on-fc.com` („Mit diesem Kader geht es nach Frankfurt"; „Alle Infos zum 6. Spieltag") · `hessenschau.de` (News-Ticker, „Köln mit Personalsorgen") · `bundesliga.com` („Voraussichtliche Aufstellungen am 6. Spieltag") · `magazin.comunio.de` (voraussichtliche Aufstellungen Frankfurt – Köln) · `wochenblatt-reporter.de` („Gegner mit Umschaltstärke")

**Bayern, Dortmund, Union (neu):** `t-online.de` („Leipzig-Spiel in Gefahr: Neuer wohl nicht fit") · `absolutfussball.com` („Bayern muss wohl auch gegen Leipzig auf Neuer verzichten") · `fussballtransfers.com` und `90min.de` (Bayern-Sorgen um Neuer) · `rhein-zeitung.de`/`tagesspiegel.de`/`volksstimme.de` (dpa, Kompany „Selbst in den Fuß geschossen") · `magazin.comunio.de` (Bayern – Leipzig, Buchmann/Musiala; Union – Dortmund) · `sport.de` („BVB ohne Schlotterbeck: Kovač packt aus") · `footy.de` und `bvbwld.de` („Macht keinen Sinn") · `dortmund.t-online.de` (Belastungssteuerung, Ricken am Flughafen) · `ligainsider.de` („Startelf auf dem Prüfstand: Kovač selbstkritisch") · `wz.de` („Nach Premierensieg: Union setzt gegen BVB auf Kontinuität") · `getfootballnewsgermany.com` (Lustrinelli)

**Schalke, Gladbach, HSV (neu):** `t-online.de` und `aachener-zeitung.de` („Schalke muss auf Torjäger Sylla verzichten") · `absolutfussball.com` („Schalke verkündet Verletzung von Sylla") · `sport.de` („Verletzungs-Schock beim FC Schalke 04") · `wochenblatt-reporter.de` („Sylla-Ausfall vor Mainz 05") · `gladbachtotal.de` („Kleindienst bricht auch Training vor Hoffenheim ab") · `bmg-news.de` („Kleindienst erneut verletzt, Kühn macht Hoffnung") · `rotowire.com` (Kühn, „could return against Hoffenheim") · `ms-aktuell.de` (Gladbachs Ausfälle) · `borussia.de` („Fohlen wollen die Abläufe festigen") · `90min.de` („Lazarett lichtet sich: HSV-Trio vor schnellem Comeback") · `nurdieraute.de` · `moinvolkspark.de` (Vorbericht, Jatta und Lokonga fraglich)

**Trainer und Tabelle (Lücken geschlossen):** `sportschau.de`/MDR („Bestätigt! Ole Werner kein Trainer mehr bei RB Leipzig"; „Mit Cheftrainer Martin Demichelis beginnt neue Zeitrechnung") · `zdfheute.de` („Nachfolger von Werner: Demichelis neuer Trainer von RB Leipzig"; „Paderborns Trainer Ralf Kettemann: Mit Selbstreflexion zum Erfolg") · `bundesliga.com` („Die neuen Trainer der Bundesliga"; „Ralf Kettemann: Who is the man who led Paderborn back to the Bundesliga?") · `sportschau.de`/SWR (Kettemann-Porträts) · `neunzigplus.de` („Bundesliga-Trainer 2026/27") · `weltfussball.de`, `bulibox.de`, `de.wikipedia.org` (Tabelle nach dem 5. Spieltag)

**Vorberichte:** `bundesliga.com` („Surprise leaders Freiburg face toughest test yet at Bayer Leverkusen"; „Mit Rückenwind in die EL-Woche") · `scfreiburg.com` („Getting going against Jablonec") · `90min.de` (Übertragung Posen) · `sportsmole.co.uk` (Vorberichte, teils mit abweichenden Aufstellungserwartungen)

**Verworfen oder nur mit Vorbehalt verwendet** (siehe eigener Abschnitt): `sport.de` (Liveticker Hoffenheim mit falschen Torschützen) · `t-online.de` („Nullnummer gegen Bukarest", falsche Saison) · `hsv.de` („Wir werden sehr viel verteidigen müssen", 188 Tage alt) · `nw.de` (Paderborn-Sextett, Pokal 2024) · `flashscore.de` (Verletzungsübersicht 2023/24) · `ligainsider.de` (Widmer/Nebel „vor Leverkusen"; Paderborner Verletzte undatiert) · `kicker.de` (Spieltagsseite mit 0 Punkten) · `sport.de` (Tabelle über vier Spiele) · `magazin.comunio.de` (Kleindienst in der Prognoseelf) · `bundesliga.com` (Anstoß 19:00 für Hoffenheim – Beşiktaş) · `fotmob.com` (undatierte Kaderseiten)
