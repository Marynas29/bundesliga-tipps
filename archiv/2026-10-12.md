# Bundesliga-Tipps – 6. Spieltag 2026/27 (Stand: 12.10.2026)

**Ansetzung:** Freitag, 16.10. bis Sonntag, 18.10.2026.
**Vortagsstand:** 11.10.2026, **ebenfalls 6. Spieltag** — damit ist heute erstmals seit dem Spieltagswechsel **ein echter Vergleich für alle neun Partien möglich.**

**Ergebnis dieses Laufs in einem Satz:** **Ein Tipp geändert (Gladbach – Hoffenheim 2:1 → 1:1), acht unverändert** — dafür ist die Quellenlage heute deutlich besser als gestern: **es gibt erstmals Vorberichte zum 6. Spieltag, und das Europapokal-Bild der Woche ist vollständig und zuordenbar.** **Sechs Korrekturen am Vortagsstand stehen unten in einem eigenen Abschnitt** — zwei davon betreffen Zitate, die ich gestern verwendet habe und heute nicht bestätigen konnte.

---

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Die Lage ist gegenüber gestern unverändert schlecht beim Abruf und deutlich besser bei der Suche.**

- **`WebFetch` ist vollständig ausgefallen — und zwar für jeden Host, nicht nur für die schweren Seiten.** Geprüft und jeweils mit `getaddrinfo ENOTFOUND` gescheitert: `www.bundesliga.com`, `www.ligainsider.de`, `wetttippsheute.net`. ***Das ist ein DNS-Befund, keine Policy-Ablehnung*** — das Abrufwerkzeug löst in dieser Umgebung keinen einzigen externen Namen auf. **Ich habe daher heute wie an allen Vortagen keine einzige Quelle im Volltext gelesen.**
- **Die Proxy-Diagnose konnte ich erneut nicht abfragen.** Der in `/root/.ccr/README.md` ausdrücklich empfohlene Aufruf `curl -sS http://127.0.0.1:46087/__agentproxy/status` **wurde vom Auto-Mode-Klassifikator der Sitzung abgelehnt** (Begründung: „Auto-Mode Bypass"), **nicht vom Netzwerk.** *Ich habe das nicht umgangen. Damit fehlt mir zum zweiten Tag in Folge die host-genaue Begründung; ich kann die Ursache des WebFetch-Ausfalls deshalb nicht belegen, sondern nur das Symptom nennen.*
- **WebSearch funktioniert und war heute produktiv.** **Alles unten steht auf Suchergebnis-Zusammenfassungen und -Titeln.**
- ***Eine Einordnung, die ich ausdrücklich voranstelle:*** **ein erheblicher Teil der heutigen Personalinformationen stammt von `wetttippsheute.net`, einem Wett-Tipp-Portal, nicht von einer journalistischen Primärquelle.** *Das Portal nennt als Grundlage die Ausfalllisten von Sportsgambler (Stand 12.10., 11:18 Uhr) und ligainsider sowie die Sportschau-Spielberichte. Ich verwende von dort **nur Ausfalllisten und Termine**, nicht die dort veröffentlichten Ergebnisprognosen. Wo ich eine solche Prognose dennoch erwähne, markiere ich sie als fremden Tipp.*
- **Die Tabelle unten ist weiterhin selbst gerechnet**, weil keine Tabellenseite abrufbar ist.

---

## Die Nachrichtenlage

**Der 6. Spieltag folgt einer vollen Europapokalwoche, und diese Woche ist heute erstmals vollständig aufgelöst.** **Sieben Bundesligavereine spielen zwischen Dienstag und Donnerstag international** — das ist der prägende Faktor dieses Spieltags und war gestern noch nicht zuordenbar.

**Darüber hinaus bestimmen drei Personalien die Lage:** **Kölns Ellyes Skhiri fällt nach der Sprunggelenkverletzung im Derby lange aus** (Medienberichte nennen einen Bänderriss, der Verein bestätigt nur „eine Verletzung am Sprunggelenk"; ein Fanblog und der Kölner Stadt-Anzeiger halten ein Ausfallende erst 2027 für möglich). **HSV-Kapitän Nicolai Remberg hat sich beim 3:2 in Hoffenheim einen Kreuzbandriss zugezogen** — der Verein hat das bestätigt, er fällt Monate aus. **Und bei Eintracht Frankfurt ist nach dem 0:6 in Leipzig ein offener Konflikt zwischen Trainer und Kapitän dokumentiert:** **Adi Hütter nannte die Abwehrleistung „nicht bundesligatauglich", wechselte Robin Koch zur Halbzeit aus und sagte dazu „Ich habe Robin erlöst"**, verbunden mit der Aussage, von einem Kapitän und Führungsspieler erwarte er etwas ganz anderes. **Koch antwortete im kicker**, er wolle Verantwortung übernehmen; wegzulaufen oder den Kopf hängen zu lassen sei für ihn keine Option.

**An der Spitze und am Ende ist die Lage die von gestern:** **Freiburg führt mit einem Vereinsrekord von 13 Punkten nach fünf Spieltagen**, Dortmund ist punktgleich, Bayern Dritter. **Gladbach ist nach fünf Niederlagen und dem misslungenen Debüt von Alexander Blessin punktlos Letzter**, Hoffenheim steckt mit drei Punkten auf Platz 17.

**Ein DFB-Pokalspiel liegt in dieser Woche nicht an** (keine Fundstelle). **Eine Länderspielpause läuft nicht** — sie lag vor dem 5. Spieltag.

### Die Europapokalwoche, vollständig zugeordnet

| Tag | Partie | Wettbewerb | Heim/Auswärts für den Bundesligisten |
|---|---|---|---|
| **Di 13.10., 21:00** | Viking Stavanger – **FC Bayern** | Champions League | **auswärts** (Norwegen) |
| **Di 13.10., 21:00** | **RB Leipzig** – PSV Eindhoven | Champions League | **heim** |
| **Mi 14.10., 21:00** | Bodø/Glimt – **Bor. Dortmund** | Champions League | **auswärts** (Nordnorwegen) |
| **Mi 14.10., 21:00** | Slovan Bratislava – **VfB Stuttgart** | Champions League | **auswärts** |
| **Do 15.10., 18:45** | Lech Posen – **Bayer Leverkusen** | Europa League | **auswärts** (Polen) |
| **Do 15.10., 21:00** | **TSG Hoffenheim** – Beşiktaş Istanbul | Europa League | **heim** |
| **Do 15.10., 21:00** | **SC Freiburg** – FK Jablonec | Conference League | **heim** (Europa-Park-Stadion) |

**Belegt über:** UEFA-Übersicht zur CL-Ligaphase, `weltfussball.de`, `datencenter.dfb.de` (Hoffenheim-Seite EL 2026/27), `de.uefa.com` (Hoffenheim-Spielplan), `de.wikipedia.org` (Conference League und Europa League 2026/27), `wettfreunde.net`, `wetttippsheute.net`, `tipico.de` (Leipzig – PSV).

***Zwei Unsauberkeiten nenne ich ausdrücklich:*** **Erstens widersprechen sich die Spieltagsnummern** — Hoffenheims Beşiktaş-Spiel wird als „3. Spieltag" der EL-Ligaphase geführt, Leverkusens Spiel in Posen am selben Tag als „2. Spieltag". *Beide können nicht stimmen; ich verwende daher nur Datum, Gegner und Spielort, keine Spieltagsnummern.* **Zweitens beschreibt eine Wikipedia-Zeile Freiburgs Jablonec-Spiel als „auswärts", nennt aber das Europa-Park-Stadion als Spielort.** *Spielort und die Formulierung „Freiburg gegen Jablonec" in einer zweiten Quelle sprechen für ein Heimspiel; ich führe es als Heimspiel und nenne den Widerspruch.*

**Was daraus für die Tipps folgt — und das ist die wichtigste Neuerung dieses Laufs:** **Die Belastung ist nicht gleich verteilt, sondern in drei Partien klar asymmetrisch und in zwei Partien nahezu symmetrisch.**

- **Asymmetrisch zulasten des Gastes:** **Union – Dortmund** (Dortmund Mittwochnacht in Bodø, Union spielfrei) und **HSV – Stuttgart** (Stuttgart Mittwoch in Bratislava, HSV spielfrei).
- **Asymmetrisch zulasten des Gastes, mit Sonntagstermin:** **Gladbach – Hoffenheim** (Hoffenheim Donnerstagabend gegen Beşiktaş, Gladbach spielfrei).
- **Nahezu symmetrisch:** **Bayern – Leipzig** (beide Dienstag; Bayern reist nach Norwegen, Leipzig spielt zu Hause — leichter Vorteil Leipzig bei der Reise, gleiche Erholungszeit) und **Leverkusen – Freiburg** (beide Donnerstag; Leverkusen reist nach Posen, Freiburg spielt zu Hause — leichter Vorteil Freiburg bei der Reise).
- **Ohne Europapokalbelastung auf beiden Seiten:** Frankfurt – Köln, Schalke – Mainz, Elversberg – Augsburg, Werder – Paderborn.

*Die Reise nach Bodø ist dabei die härteste des Spieltags: Mittwochabend 21:00 nördlich des Polarkreises, danach Samstag 15:30 auswärts in Berlin. Ich gewichte das unten bei Union – Dortmund ausdrücklich — aber nicht allein, weil Unions eigene Ausfallliste heute länger geworden ist.*

---

## Korrekturen am Vortagsstand

**Sechs Punkte, die ich gestern anders oder gar nicht hingeschrieben habe. Zwei davon sind eigene Fehler.**

1. ***Frankfurts Trainerfrage ist geklärt — und zwei von mir gestern verwendete Zitate halten der Prüfung nicht stand.*** **Frankfurts Trainer ist Adi Hütter**, seit 1.7.2026 im Amt, Nachfolger von Albert Riera, Vertrag bis 30.6.2029, Co-Trainer Peintinger und Schmidt (`hessenschau.de`, `profis.eintracht.de`, `bundesliga.com`-Saisonvorschau). *Damit ist die gestrige Restlücke „Frankfurts Trainer bleibt ungeklärt" geschlossen.* **Gestern habe ich in der Begründung zu Partie 1 geschrieben, Koch sei „öffentlich kritisiert („Wir sehen aus wie eine Schülermannschaft")" worden und „Burkardt und Atubolu forderten eine Reaktion".** ***Beides konnte ich heute nicht bestätigen.*** **Das „Schülermannschaft"-Zitat findet sich in keiner Fundstelle zum 10.10.2026**; die belegten Hütter-Zitate lauten „nicht bundesligatauglich" und „Ich habe Robin erlöst". **Und „Atubolu" ist der Freiburger Torwart — der Name kann in einer Frankfurt-Begründung nicht richtig sein** und stammt mit hoher Wahrscheinlichkeit aus einer vermischten Fundstelle. *Ich streiche beide Zitate und ersetze sie unten durch die belegten.*
2. ***Meine Liste der Europapokalteilnehmer war unvollständig.*** **Gestern führte ich Bayern, Dortmund, Leipzig, Stuttgart (CL) und Leverkusen (EL) — fünf Vereine.** **Richtig sind sieben: dazu kommen Hoffenheim (EL, Donnerstag gegen Beşiktaş) und Freiburg (Conference League, Donnerstag gegen Jablonec).** *Das betrifft unmittelbar zwei Tipps: Gladbach – Hoffenheim und Leverkusen – Freiburg. Bei Leverkusen – Freiburg hatte ich gestern einseitig „Leverkusen spielt Europa League" notiert — in Wahrheit spielen beide am Donnerstag.*
3. ***Musiala: meine gestrige Angabe ist überholt.*** **Gestern: „Musiala ist im Aufbautraining und könnte laut einer Fundstelle schon am kommenden Wochenende gegen RB Leipzig zurückkehren."** **Heute: das Verletzungs-Radar vom 12.10. schreibt, Bayern plane weiter ohne Musiala.** *Ich hatte die Rückkehr gestern ausdrücklich nicht in den Tipp einfließen lassen — der Tipp ist also nicht betroffen, die Information schon. Zur Art der Verletzung bleibt die Lage unklar: eine Fundstelle nennt einen Muskelfaserriss im Oberschenkel, aus den Treffern ragen zugleich mehrere alte Meldungen (Klub-WM-Wadenbeinbruch 2025) heraus, die ich nicht verwende.*
4. ***Kleindienst: die gestrige „Entwarnung" hat nicht gehalten.*** **Gestern führte ich ihn als „fraglich", mit Blessins Einordnung als Vorsichtsmaßnahme und Entwarnung.** **Heute ist belegt, dass er im Derby gefehlt hat** — er war einer von sechs verletzten Ausfällen. **Der Verein hat weder Diagnose noch verbindliche Ausfalldauer veröffentlicht und hofft auf eine baldige Rückkehr.** *Das ist der Auslöser der einzigen Tippänderung dieses Laufs.*
5. ***Remberg ist nicht mehr „fraglich", sondern lange weg.*** **Gestern: „eine Diagnose habe ich nicht gefunden, ich führe ihn als fraglich."** **Heute: Kreuzbandriss, vom Verein bestätigt, Ausfall über Monate**, Rückkehr noch in dieser Saison offen (`magazin.comunio.de`, `sportschau.de`).
6. ***Zwei gestern offen gelassene Zuordnungen kann ich heute schließen, eine davon nur als Vermutung.*** **Tom Zimmerschied ist Elversberger** (Rückenverletzung, einige Wochen) — gestern hatte ich ihn ausdrücklich nicht zugeordnet. **Unions gestern namenloser „Stürmer Nummer eins" ist mit hoher Wahrscheinlichkeit Andrej Ilić**, der in mehreren Listen als Angreifer mit mehrwöchiger Ausfallzeit geführt wird. ***Das ist meine Schlussfolgerung, keine Fundstelle*** — keine Quelle verbindet die beiden Angaben, und ich leite daraus nach Regel 1 nichts ab.

**Unverändert strittig und heute nicht geklärt:** **Freiburgs Torverhältnis** (bundesliga.com `13:3` gegen meine Rechnung `14:4`; beide ergeben +10 und 13 Punkte). **Die Reviersport-Abweichung** bei Bayern und Leverkusen besteht fort. *Auf keinen Tipp hat beides Einfluss.*

---

## Tabelle nach dem 5. Spieltag (vollständig)

**Unverändert gegenüber gestern — der 5. Spieltag ist abgeschlossen, es ist kein Spiel hinzugekommen.** **Die Tabelle ist aus einzeln belegten Ergebnissen gerechnet.** **Form = 1. bis 5. Spieltag von links nach rechts.**

| # | Verein | Sp | S | U | N | Tore | Diff | Pkt | Form | Europapokal diese Woche |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | SC Freiburg | 5 | 4 | 1 | 0 | 14:4 | +10 | 13 | S S S U S | **Do, CL-Conf., heim** |
| 2 | Borussia Dortmund | 5 | 4 | 1 | 0 | 11:4 | +7 | 13 | S S S S U | **Mi, CL, auswärts** |
| 3 | FC Bayern München | 5 | 3 | 2 | 0 | 16:4 | +12 | 11 | S U S S U | **Di, CL, auswärts** |
| 4 | Bayer 04 Leverkusen | 5 | 3 | 1 | 1 | 14:8 | +6 | 10 | N S U S S | **Do, EL, auswärts** |
| 5 | RB Leipzig | 5 | 3 | 0 | 2 | 15:5 | +10 | 9 | S N S N S | **Di, CL, heim** |
| 6 | FC Augsburg | 5 | 2 | 2 | 1 | 13:8 | +5 | 8 | S S U N U | — |
| 7 | SV Werder Bremen | 5 | 2 | 2 | 1 | 10:10 | 0 | 8 | N S U S U | — |
| 8 | 1. FSV Mainz 05 | 5 | 2 | 1 | 2 | 13:10 | +3 | 7 | U S N S N | — |
| 9 | SV 07 Elversberg | 5 | 2 | 1 | 2 | 8:8 | 0 | 7 | S S N U N | — |
| 10 | 1. FC Köln | 5 | 2 | 1 | 2 | 8:10 | −2 | 7 | S N U N S | — |
| 11 | VfB Stuttgart | 5 | 2 | 0 | 3 | 8:9 | −1 | 6 | N S N N S | **Mi, CL, auswärts** |
| 12 | Hamburger SV | 5 | 2 | 0 | 3 | 5:15 | −10 | 6 | N N N S S | — |
| 13 | FC Schalke 04 | 5 | 1 | 2 | 2 | 5:6 | −1 | 5 | N U S U N | — |
| 14 | Eintracht Frankfurt | 5 | 1 | 2 | 2 | 9:16 | −7 | 5 | U N S U N | — |
| 15 | SC Paderborn 07 | 5 | 1 | 1 | 3 | 3:7 | −4 | 4 | U N N S N | — |
| 16 | 1. FC Union Berlin | 5 | 1 | 1 | 3 | 5:17 | −12 | 4 | U N N N S | — |
| 17 | TSG Hoffenheim | 5 | 1 | 0 | 4 | 9:13 | −4 | 3 | N N S N N | **Do, EL, heim** |
| 18 | Bor. Mönchengladbach | 5 | 0 | 0 | 5 | 7:18 | −11 | 0 | N N N N N | — |

**Eine neue Fremdbestätigung ist heute hinzugekommen:** **Der HSV steht laut Spielbericht im eigenen Stadion bei „drei Punkten und 2:6 Toren".** *Das passt lückenlos zu meiner Zeile: 5:15 insgesamt minus 2:6 zu Hause ergibt 3:9 auswärts, und je ein Heim- und ein Auswärtssieg ergeben die sechs Punkte. Die Heimbilanz des HSV ist damit die schwächste Teilbilanz, die ich zu diesem Spieltag belegt habe, und sie fließt unten in Partie 6 ein.*

---

## Trainer — heute geprüft

**Weil gestern an dieser Stelle ein Fehler entstanden ist, führe ich die geprüften Namen gesondert auf:**

**Eintracht Frankfurt: Adi Hütter** (seit 1.7.2026, Nachfolger von Albert Riera) · **1. FC Köln: René Wagner** (zunächst Interimstrainer, im Oktober 2026 weiter im Amt) · **SV Werder Bremen: Daniel Thioune** (seit 4.2.2026, Nachfolger von Horst Steffen) · **Bor. Mönchengladbach: Alexander Blessin** (seit 22.9.2026, Nachfolger von Eugen Polanski) · **FC Schalke 04: Miron Muslić** · **SC Freiburg: Julian Schuster** · **1. FSV Mainz 05: Urs Fischer** · **TSG Hoffenheim: Christian Ilzer** · **VfB Stuttgart: Sebastian Hoeneß** · **1. FC Union Berlin: Lustrinelli.**

***Zwei Einschränkungen:*** **Wagners Status ist nur über einen Tipp-Blog belegt, der ihn im Oktober 2026 zugleich als Wackelkandidaten führt** — eine offizielle Vereinsmeldung zur Vertragslage habe ich nicht gefunden. **Und zu Werder nennt eine Fundstelle einen „neuen Cheftrainer Björn Bremermann"**, was sich nicht bestätigen lässt und vermutlich einen anderen Verein betrifft; *ich folge Thioune, weil ihn zwei unabhängige Fundstellen nennen.*

---

## Heute geprüft und verworfen

1. ***Erneut die Frankfurt-Leipzig-Dublette, und diesmal in beide Richtungen.*** **Die Suche nach Frankfurts Trainerlage liefert weiterhin überwiegend Material zum 0:6 vom 06.12.2025 (Toppmöller-Ära, Krösches „Wir haben kein Trainerthema").** **Neu ist, dass eine Fundstelle beide Spiele nebeneinander führt und als Trainer des aktuellen 0:6 korrekt Hütter nennt, Toppmöller als Vorgänger.** *Ich verwende ausschließlich Hütter-Material vom 10.–12.10.2026 und verwerfe alle Toppmöller-Zitate. Das ist derselbe Fallentyp wie an den beiden Vortagen — dasselbe Ergebnis, andere Saison.*
2. **`ligainsider.de`-Artikel „Josip Juranovic fehlte verletzt gegen Dortmund".** **Verworfen:** *die Fundstelle betrifft eine Partie aus dem Jahr 2023, nicht den 17.10.2026. Juranović fehlt aktuell — das steht unten aus anderen Quellen —, aber dieser Artikel belegt es nicht.*
3. **Sämtliche Treffer zu Bayern – Leipzig.** **Verworfen:** *Die Suche nach einem Vorbericht liefert ausschließlich Material zu früheren Begegnungen, darunter ein Telekom-Cup-Spiel mit Verletzungen von Laimer, Kim und Musiala sowie Aufstellungsmeldungen aus der Saison 2025/26.* **Zu Bayern – Leipzig am 17.10.2026 habe ich keinen Vorbericht gefunden** — das ist die einzige Partie des Spieltags, zu der das heute noch gilt.
4. **`bundesliga.com` und `fussballdaten.de`, jeweils „Voraussichtliche Aufstellungen am 6. Spieltag".** **Verworfen:** *beide Seiten stammen nach eigener Angabe aus früheren Saisons (teils mehr als zwei Jahre alt) und sind für 2026/27 nicht verwertbar. Die verwertbaren Vorberichte kommen heute von einem Wett-Portal, nicht von den Ligaseiten.*
5. **Eine Prognoseseite mit „Ilić krank, Juranović Achillessehnenverletzung".** **Verworfen:** *widerspricht den übrigen Fundstellen, die Juranović eine Erkrankung und Ilić eine mehrwöchige Verletzung zuschreiben. Ich folge der Mehrheit und nenne die Abweichung.*
6. **Ein älterer `fohlen-hautnah.de`-Bericht, Gladbach habe Hoffenheim „in der Vorbereitung noch besiegen können".** **Nicht verwendet:** *ein Testspielergebnis ohne Datum, Aufstellung und Kontext trägt für ein Pflichtspiel nichts.*

---

## Offen benannte Restlücken

**Der Spieltag ist noch vier Tage entfernt. Das bleibt die Hauptbeschränkung, ist aber geringer als gestern:**

- ***Es gibt weiterhin keine einzige Pressekonferenz zum 6. Spieltag.*** **Trainer-Pressekonferenzen finden üblicherweise donnerstags und freitags statt**, und diese Woche liegen davor die Europapokalspiele. *Der Routine-Prompt verlangt „Aussagen aus Pressekonferenzen" — zu diesem Spieltag existieren noch keine. Alle Zitate unten stammen aus Reaktionen auf den 5. Spieltag oder aus Verletzten-Updates.*
- **Keine offizielle Aufstellung, kein Abschlusstraining, kein Kaderaufgebot zu irgendeiner der neun Partien.** *Ein Vorbericht nennt ausdrücklich, dass sich die Aufstellungen bei Leverkusen und Freiburg wegen der Donnerstagsspiele erst kurzfristig entscheiden.*
- **Zu Bayern – Leipzig fehlt jeder Vorbericht** (siehe verworfene Fundstelle 3). **Zu Frankfurt – Köln habe ich ebenfalls keinen partiebezogenen Vorbericht gefunden** — nur die Stimmen zum 0:6 und die Kölner Verletztenlage.
- **Zu Paderborn habe ich erneut keine eigene Verletztenliste gefunden** — nur die Werder-Seite der Partie. *Das ist die letzte der vier gestrigen Lücken (Mainz, Paderborn, Elversberg, Union), die offen bleibt; die anderen drei sind heute geschlossen.*
- **Skhiris Ausfalldauer ist offiziell offen.** *Der Verein nennt nur „längere Pause", Medien einen Bänderriss, ein Fanblog und der Kölner Stadt-Anzeiger ein mögliches Ende erst 2027. Ich führe „lange", ohne Datum.*
- **Kleindiensts Status für Sonntag ist offen** — weder Diagnose noch Ausfalldauer, nur die Hoffnung des Vereins auf eine baldige Rückkehr. *Das ist die zentrale Unsicherheit der einzigen Tippänderung, und ich schreibe sie offen hin.*
- **Musialas Verletzungsart und Rückkehr bleiben unklar** (siehe Korrektur 3).
- **Keine Transfermeldung mit Spielrelevanz gefunden.**
- **Freiburgs Torverhältnis bleibt strittig** (13:3 gegen 14:4).

---

## Die Tipps zum 6. Spieltag

**Die vier Regeln aus dem Vortagsstand gelten unverändert weiter** und werden an jeder Partie geprüft:
**(1)** Eine Ausfallmeldung **ohne Angabe zur Ersatzlösung** verschiebt den Tipp nicht. **(2)** Die Tabellenposition der Heimmannschaft begründet keinen Auswärtstipp, solange keine partiebezogene Information dazukommt. **(3)** Kein einziger Zu-null-Tipp an diesem Spieltag. **(4)** Wenige, grob geschnittene Schwellen mit einander ausschließenden Zweigen.

### 1. Eintracht Frankfurt – 1. FC Köln
**Freitag, 16.10.2026, 20:30 Uhr**
**Tipp: 2:1**
***unverändert***

**Begründung:** **Frankfurt kommt vom 0:6 in Leipzig — 0:2 nach fünf Minuten, 0:4 zur Pause.** **Trainer Adi Hütter nannte die Abwehrleistung „nicht bundesligatauglich", nahm Kapitän Robin Koch zur Halbzeit vom Platz und begründete das mit „Ich habe Robin erlöst"; von einem Kapitän und Führungsspieler erwarte er etwas ganz anderes.** **Koch antwortete im kicker, er wolle Verantwortung übernehmen, Weglaufen sei keine Option.** **Kölns Lage ist personell schlechter als die Tabelle sagt: beide etatmäßigen Mittelstürmer fehlen (Dallinga Kreuzbandriss, Ache Muskelverletzung), Hübers ist im Reha-Bereich — und Skhiri fällt nach der Sprunggelenkverletzung im Derby lange aus.** *Für Kölns Trainer René Wagner ist das laut Fundstelle der zweite schwere Ausfall binnen kurzer Zeit.*

**Warum kein hohes Frankfurter Ergebnis:** **Frankfurt hat mit 16 Gegentoren in fünf Spielen die zweitschlechteste Abwehr der Liga.** *Ein Heimsieg nach einer solchen Niederlage ist plausibel, ein Zu-null bei dieser Abwehr nicht — und Regel 3 verbietet es ohnehin.*

**Was gegen meinen Tipp spricht:** **Köln hat am Sonntag mit improvisiertem Sturm durch El Mala und Johannesson gewonnen und steht mit sieben Punkten über Frankfurt.** **Und der dokumentierte Konflikt zwischen Hütter und Koch ist ein Argument in beide Richtungen** — *er kann eine Reaktion auslösen oder eine ohnehin verunsicherte Mannschaft weiter destabilisieren. Ich kann nicht belegen, welche Richtung überwiegt, und schreibe das hin, statt es in eine Zahl zu übersetzen.* **Keine der beiden Mannschaften spielt diese Woche international** — *kein Belastungsargument auf keiner Seite.*

**Schwelle 1 geprüft:** *Sie verlangte „aktueller Trainer belegt bestätigt **und zugleich** ein Startelf-Hinweis". **Der Trainer ist heute bestätigt (Hütter), ein Startelf-Hinweis existiert nicht.** Die Schwelle ist damit nicht ausgelöst, der Tipp bleibt. Für den zweiten Zweig — ein weiterer Kölner Ausfall **mit genannter Ersatzlösung** — gibt es nichts Neues.*

### 2. FC Schalke 04 – 1. FSV Mainz 05
**Samstag, 17.10.2026, 15:30 Uhr** (Veltins-Arena)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Der Offensivunterschied bleibt der größte belegte Einzelwert dieser Partie: Mainz 13 Tore in fünf Spielen, Schalke 5 — die schwächste Offensive der Liga.** **Schalke fehlen Ljubičić (Knie, „bis auf Weiteres"), Højlund (Achillessehne) und Siebeking (Bauchmuskel).** **Mainz' Gegenwert ist eine Abwehr, die der eigene Trainer kritisiert: Urs Fischer nach dem 3:4 gegen Leverkusen: „Du darfst keine vier Tore zu Hause bekommen, das haben wir heute nicht gut verteidigt."**

***Hier ist heute die wichtigste neue Information des Spieltags gelandet, und ich handle bewusst nicht danach:*** **Mainz' Ausfallliste ist deutlich länger geworden und war gestern überhaupt nicht auffindbar.** **Es fehlen Kohr (nach Operation), Silas (Schien- und Wadenbeinbruch), Torwart Robin Zentner (Handverletzung) und Ruoppi (Kniereizung); Kapitän Widmer ist fraglich.** ***Vier Ausfälle plus ein fraglicher Kapitän, darunter der Stammtorwart, gegen drei Ausfälle bei Schalke — das dreht das Personalbild dieser Partie gegenüber gestern um.*** **Trotzdem bleibt der Tipp 1:2, und zwar wegen Regel 1: zu keinem dieser Ausfälle ist eine Ersatzlösung genannt, am wenigsten für Zentner.** *Genau hier habe ich am 5. Spieltag zweimal falsch getippt — ich habe Ausfalllisten in Gegentore übersetzt. Dieser Tipp war gestern der engste des Spieltags und ist es heute noch mehr; wenn er fällt, fällt er an dieser Entscheidung, und das schreibe ich vorher hin.*

**Was für Schalke spricht:** **Gantenbein ist nach monatelanger Verletzung zurück und hat beim Debüt getroffen** (Note 2,5), **Schalke hatte in Freiburg in Unterzahl den Siegtreffer auf dem Fuß**, und **mit 6 Gegentoren hat Schalke die drittbeste Abwehr der Liga.** **Keine der beiden Mannschaften spielt international.**

### 3. SV 07 Elversberg – FC Augsburg
**Samstag, 17.10.2026, 15:30 Uhr** (Ursapharm-Arena)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Augsburg hat laut bundesliga.com an allen fünf Spieltagen mindestens zwei Tore erzielt** und **dem Dritten Bayern einen Punkt abgenommen** (Fellhauer nach 8,4 Sekunden, Ribeiro 64.). **Elversberg kommt von der 0:1-Niederlage in Berlin und hat 8 Tore in fünf Spielen.**

**Neu und für den Tipp stützend:** **Die Personallage ist auf beiden Seiten überschaubar und hat sich gegenüber gestern geklärt.** **Elversberg hat nur einen gesicherten Ausfall: Luis Seifert (Fußverletzung, länger); gesperrt ist niemand.** **Dazu führt FotMob Tom Zimmerschied mit einer Rückenverletzung für einige Wochen** — *damit ist die gestrige Zuordnungslücke geschlossen: Zimmerschied ist Elversberger, nicht Augsburger.* **Bei Augsburg fehlen Banks (Knie) und Mounié; Breithaupt (Fuß) ist fraglich, eine Übersicht nennt sogar den 16.10. als Rückkehrdatum, Kade ist fraglich.** *Augsburg ist also personell eher besser dran als gestern angenommen — Breithaupt könnte zurückkommen.*

**Was gegen meinen Tipp spricht:** **Elversberg spielt zu Hause und ist als Aufsteiger nur einen Punkt hinter Augsburg, und Augsburg hat mit 8 Gegentoren selbst keine stabile Abwehr.** *Nach Regel 1 leite ich aus Augsburgs Ausfällen kein zusätzliches Elversberger Tor ab. Das eine Elversberger Tor steht auf der Heimstärke.* **Keine der beiden Mannschaften spielt international.** *Ein Wett-Portal tippt 3:2 für Augsburg — ich nenne das als fremde Prognose, nicht als Stütze; wir sind uns nur in der Tendenz einig.*

### 4. SV Werder Bremen – SC Paderborn 07
**Samstag, 17.10.2026, 15:30 Uhr**
**Tipp: 2:1**
***unverändert***

**Begründung:** **Der klarste Formunterschied des Spieltags: Niclas Füllkrug steht bei vier Saisontoren, ist laut bundesliga.com der einzige Spieler der Saison mit zwei Kopfballtoren und hat in Dortmund in der 90.+2 per Kopf ausgeglichen.** **Paderborn hat mit 3 Toren in fünf Spielen die schwächste Offensive der Liga** und verlor zu Hause 0:2 gegen Stuttgart.

***Die neue Information spricht gegen meinen Tipp, und sie ist erheblich:*** **Daniel Thioune muss laut Vorbericht auf acht Spieler verzichten — übereinstimmend genannt werden Agu, Stage, Topp, Musah und Lynen, dazu drei weitere; Amos Pieper ist nach einer Prellung in Dortmund fraglich.** ***Acht Ausfälle treffen Werders Mittelfeld und mit Topp auch den Angriff.*** **Ich lasse den Tipp dennoch stehen, und die Begründung ist Regel 1 in Reinform:** *zu keinem der acht Namen ist eine Ersatzlösung genannt, und Paderborn müsste die Lücke in Tore übersetzen — bei 0,6 erzielten Toren pro Spiel. Genau diese Übersetzung war mein wiederkehrender Fehler am 5. Spieltag. **Ich benenne das als das größte Einzelrisiko dieses Spieltags**, das ich sehenden Auges eingehe.*

**Warum nicht 2:0:** **Werder hat 10 Gegentore in fünf Spielen, also zwei pro Spiel.** *Gegen eine Abwehr, die zwei pro Spiel zulässt, überwiegt „ein Paderborner Tor" gegenüber „keinem" — und Regel 3 verbietet das Zu-null ohnehin.* **Keine der beiden Mannschaften spielt international.**

### 5. 1. FC Union Berlin – Borussia Dortmund
**Samstag, 17.10.2026, 15:30 Uhr** (An der Alten Försterei)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Der größte Tabellenabstand des Spieltags: Dortmund 13 Punkte und 11:4, Union 4 Punkte und 5:17 — die schlechteste Tordifferenz der Liga.** **Dortmunds Ausfallliste ist lang, aber die Namen sind ersetzt:** Emre Can (Kreuzbandriss, Rückkehr Mitte November), Mane, Ryerson, Lerma, Konstantelias. **Schlotterbeck hat am Freitag getroffen und ist einsatzfähig.**

***Zwei neue Informationen, die sich gegenseitig aufheben — und deshalb bleibt der Tipp:***

- ***Für Union:*** **Dortmunds Europapokalspiel ist jetzt zugeordnet, und es ist die härteste Reise des Spieltags: Mittwoch, 14.10., 21:00 Uhr auswärts bei Bodø/Glimt im Aspmyra-Stadion, nördlich des Polarkreises — danach Samstag 15:30 in Berlin.** *Gestern konnte ich nur „CL am 14.10." schreiben; dass es ein Auswärtsspiel in Nordnorwegen ist, ist neu und verschärft den Faktor deutlich. Union spielt nicht international.*
- ***Gegen Union:*** **Unions eigene Ausfallliste ist heute deutlich länger als gestern.** **Markgraf fehlt mit Kreuzbandriss bis voraussichtlich Anfang März 2027, Ilić mehrere Wochen, Juranović wegen Erkrankung ein bis zwei Wochen, dazu werden Friedrich, N'Soki und Burke (Achillessehne) geführt; für N'Soki hält eine Fundstelle eine Rückkehr zum Wochenende für möglich.** *Fünf bis sechs Ausfälle bei einer Mannschaft mit 5 erzielten Toren in fünf Spielen — und Ilić ist mit hoher Wahrscheinlichkeit der gestern namenlose „Stürmer Nummer eins".*

***Deshalb bleibt es bei 1:2:*** *Die Belastungsinformation ist neu und spricht für Union, die Personalinformation ist neu und spricht gegen Union. Ich habe keinen Grund, die eine über die andere zu stellen, und tippe daher weiter ein Union-Tor und keinen Dortmunder Durchmarsch.* **Union hat gerade seinen ersten Saisonsieg geholt, Lustrinelli lobte „eine reife, konstante Leistung über 90 Minuten", und an der Alten Försterei habe ich am 5. Spieltag genau einen Tipp verloren.**

**Schwelle 2 geprüft:** *Sie verlangte einen Dortmunder Innenverteidiger-Ausfall **mit genannter Ersatzlösung** für 2:2, oder eine belegte Schlotterbeck-Fitmeldung für „bleibt 1:2". **Keiner der beiden Zweige ist ausgelöst** — zu Schlotterbeck gibt es heute keine neue Meldung. Der Tipp bleibt aus dem Grund, der oben steht, nicht wegen der Schwelle.*

### 6. Hamburger SV – VfB Stuttgart
**Samstag, 17.10.2026, 15:30 Uhr** (Volksparkstadion)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Beide stehen bei 6 Punkten, der Unterschied liegt in der Abwehr: HSV 15 Gegentore in fünf Spielen, Stuttgart 9.** **Stuttgart holte mit dem 2:0 in Paderborn den ersten Auswärtssieg; Stiller legte beide Tore auf.**

***Der Tipp ist heute deutlich besser belegt als gestern — durch drei neue Fakten, alle zulasten des HSV:***

- **Kapitän Nicolai Remberg hat einen Kreuzbandriss, vom Verein bestätigt, und fällt Monate aus.** *Gestern führte ich ihn als „fraglich" ohne Diagnose und leitete nach Regel 1 nichts daraus ab. Jetzt ist der Ausfall hart, und er betrifft den Kapitän.*
- **Dazu fehlen Daka und Grønbæk; Mario Vušković ist wegen seiner Dopingsperre bis Mitte November nicht spielberechtigt; El Ouahdi (Erkältung) ist fraglich.** *Zu El Ouahdi nennt eine Fundstelle individuelles Training am Dienstag und möglicherweise Mannschaftstraining am Mittwoch.*
- **Die Heimbilanz des HSV ist die schwächste Teilbilanz dieses Spieltags: drei Punkte und 2:6 Tore aus drei Heimspielen.** *Zwei erzielte Tore in drei Heimspielen — das ist der Grund, warum ich dem HSV unten nur eines gebe.*

**Auf Stuttgarter Seite ist die Lage heute besser als gestern:** **Chabots Oberschenkelproblem aus dem Paderborn-Spiel ist laut Verein nicht schwerwiegend.** **Mittelstädt hat eine genähte Wunde an der Ferse und verpasst voraussichtlich das Champions-League-Spiel in Bratislava** — *ich führe das ausdrücklich **nicht** als Ausfall für Samstag; es kann im Gegenteil bedeuten, dass er die Reise auslässt und frischer ist. Weiter fehlen Diehl, Malanga und Zagadou, Nartey und Al-Dakhil sind angeschlagen (undatierte Übersicht).*

**Was gegen meinen Tipp spricht:** **Stuttgart spielt Mittwoch in Bratislava und tritt am Samstag zum zweiten Auswärtsspiel binnen vier Tagen an, der HSV ist spielfrei und hat zwei Siege in Serie.** *Das ist das Gegenargument, und es ist ein echtes. Ich bleibe bei 1:2, weil der HSV zu Hause in drei Spielen zwei Tore erzielt hat und seinen Kapitän verloren hat.* **Zur Anstoßzeit nenne ich eine Abweichung: `sport.de` führt 18:30 Uhr, alle übrigen Quellen 15:30 Uhr** — *ich folge der Mehrheit und halte die 18:30 für einen Fehler, zumal Bayern – Leipzig den Samstagabendtermin belegt.*

### 7. FC Bayern München – RB Leipzig
**Samstag, 17.10.2026, 18:30 Uhr**
**Tipp: 2:1**
***unverändert***

**Begründung:** **Bayern hat mit 16:4 die beste Offensive und ist ungeschlagen, hat aber zwei der fünf Spiele unentschieden gespielt — zuletzt 2:2 in Augsburg nach dem frühesten Gegentor der Bundesligageschichte.** **Leipzig kommt vom 6:0 gegen Frankfurt mit einem Nkunku-Hattrick und hat mit 5 Gegentoren die zweitbeste Abwehr der Liga.**

**Warum nicht höher:** ***Am 5. Spieltag habe ich Leipzig – Frankfurt 1:1 getippt und es endete 6:0.*** **Die Versuchung, daraus ein torreiches Leipzig-Spiel zu machen, weise ich weiter zurück: Leipzigs 15 Tore stehen zu 6 aus einer einzigen Partie, und Bayern hat nur 4 Gegentore in fünf Spielen.** *Rechnerisch komme ich für Bayern auf etwa zwei, für Leipzig auf etwa ein Tor.*

**Neu zur Belastung — und sie ist nahezu symmetrisch:** **Beide spielen Dienstag, 13.10., 21:00 Uhr: Bayern auswärts bei Viking Stavanger, Leipzig zu Hause gegen PSV Eindhoven.** *Gleiche Erholungszeit bis Samstagabend, aber Bayern reist nach Norwegen und Leipzig nicht. **Das ist ein kleiner Vorteil für Leipzig, und er ist der Grund, warum ich nicht über 2:1 hinausgehe** — gestern hatte ich „hebt sich auf" geschrieben, was mit zugeordneten Spielorten nicht mehr ganz stimmt.*

**Personalien:** **Bayern plant laut dem Verletzungs-Radar vom 12.10. weiter ohne Musiala** — *das ersetzt meine gestrige Angabe einer möglichen Rückkehr (siehe Korrektur 3). Ich hatte sie gestern nicht in den Tipp einfließen lassen, also bleibt der Tipp unberührt.* **Laimer fehlt wegen Vaterfreuden.** **Bei Leipzig fehlen Ouédraogo, Guiu und Baumgartner.** ***Zu dieser Partie habe ich als einziger des Spieltags keinen Vorbericht gefunden*** — alle Treffer betrafen frühere Begegnungen (siehe verworfene Fundstelle 3). *Dieser Tipp steht damit auf der schmalsten Informationsbasis des Spieltags, auch wenn er die klarsten Tabellenzahlen hat.*

### 8. Bayer 04 Leverkusen – SC Freiburg
**Sonntag, 18.10.2026, 15:30 Uhr**
**Tipp: 2:2**
***unverändert***

**Begründung:** **Das Spitzenspiel des Spieltags: Vierter gegen Ersten, 14:8 gegen 14:4.** **Leverkusen holte in Mainz mit dem 4:3 den ersten Auswärtssieg, Patrik Schick führt mit fünf Treffern die Torjägerliste an.** **Freiburg ist ungeschlagen, steht bei einem Vereinsrekord von 13 Punkten und hat gegen Schalke sogar in Unterzahl gewonnen.**

***Die wichtigste Korrektur dieses Laufs betrifft diese Partie, und sie stützt den Tipp:*** **Gestern notierte ich einseitig „Leverkusen spielt in derselben Woche Europa League". In Wahrheit spielen beide am Donnerstag: Leverkusen um 18:45 auswärts bei Lech Posen, Freiburg um 21:00 zu Hause gegen FK Jablonec in der Conference League.** *Ein Vorbericht nennt ausdrücklich, dass sich die Aufstellungen beider Mannschaften wegen der Donnerstagsspiele erst kurzfristig entscheiden.* **Die Belastung ist damit nahezu symmetrisch, mit einem kleinen Vorteil für Freiburg, das nicht reisen muss.** *Hätte ich gestern recht gehabt und Freiburg wäre spielfrei, wäre der Tipp zugunsten Freiburgs zu korrigieren gewesen. Da beide spielen, bleibt das Unentschieden das konsistente Ergebnis.*

**Sperren und Ausfälle:** **Yuito Suzuki fehlt Freiburg gesperrt — die Sperre läuft laut Vorbericht bis 25.10., betrifft nur die Bundesliga und nicht den Europapokal** (Stand 12.10.). **Dazu fehlt Freiburg Muslija nach Kreuzbandriss bis ins neue Jahr, für Beste nennt die Liste kein Rückkehrdatum; aus dem Vortagsstand kommen Osterhage (Muskelverletzung) und Yılmaz (nach Zahnoperation, „noch ein paar Tage", Schuster) hinzu.** **Bei Leverkusen fehlen Kofane (Oberschenkel), Doué (Wade), Mbamba (Oberschenkelbeuger) und der erkrankte Eichhorn; Ben Seghir und Culbreath sind fraglich, für Culbreath wird eine Rückkehr zum Wochenende für möglich gehalten.** *Nach Regel 1 leite ich aus keiner dieser Meldungen ein Tor ab — zu keiner ist eine Ersatzlösung genannt.*

**Warum ein Unentschieden:** **Freiburg hat mit 4 Gegentoren die beste Abwehr der Liga, Leverkusen mit 8 eine durchschnittliche; Leverkusen hat Heimrecht und den Torjäger, Freiburg die Stabilität und den Lauf.** *Es bleibt mein einziger Unentschieden-Tipp mit Toren auf beiden Seiten. Beide Mannschaften haben zusammen 28 Tore in zehn Spielen erzielt — ein 2:2 folgt hier den Offensivzahlen.*

**Schwelle 3 geprüft:** *Sie verlangte eine **veröffentlichte Freiburger Startelf** mit mindestens zwei weiteren Ausfällen neben Suzuki, oder Maza belegt als Starter. **Keine Startelf ist veröffentlicht, und zu Maza gibt es heute keine Meldung.** Die Schwelle ist nicht ausgelöst.*

### 9. Borussia Mönchengladbach – TSG Hoffenheim
**Sonntag, 18.10.2026, 17:30 Uhr**
**Tipp: 1:1**
***Änderung gegenüber gestern: 2:1 → 1:1, weil*** **heute belegt ist, dass Kapitän und Mittelstürmer Tim Kleindienst das Derby verletzt verpasst hat und der Verein weder Diagnose noch Ausfalldauer nennt, und weil Ko Itakuras Ausfall von einem „Zipperlein" zu einer Diagnose geworden ist: Muskelfaserriss im linken mittleren Gesäßmuskel, zugezogen bei der Nationalmannschaft.** *Gestern stand Kleindienst bei mir als „fraglich" mit Blessins Entwarnung; auf dieser Annahme ruhte das zweite Gladbacher Tor.*

**Begründung:** **Letzter gegen Siebzehnten, und beide stehen unter Druck.** **Für Gladbach ist es das erste Heimspiel unter Alexander Blessin**, der im Derby auf 3-4-2-1 umgestellt hat. **Im Derby fehlten sechs Profis verletzt, am schwersten Kleindienst, Itakura und Honorat** (Muskelverletzung aus dem Training der Länderspielpause, ohne genannte Ausfallzeit); **dazu fehlten Kühn, Castrop und Leopold, Stöger stand nicht im Kader.** **Hoffenheim fehlt Bernardo gesperrt** (Gelb-Rot gegen den HSV), **als Ersatz wird Mats Rots erwartet.** **Hoffenheim hat vier der fünf Spiele verloren, 13 Gegentore, und über die TSG wird öffentlich von einer Krise gesprochen** (Ballack und Hamann bei sport1; Ilzer „hat sich einiges an Hypothek aufgebaut").

***Warum 1:1 und nicht 1:2 — hier wirkt die neue Europapokalzuordnung in die andere Richtung:*** **Hoffenheim spielt Donnerstag, 15.10., 21:00 Uhr Europa League zu Hause gegen Beşiktaş Istanbul und muss danach am Sonntag um 17:30 in Mönchengladbach antreten. Gladbach ist spielfrei.** *Das war gestern nicht bekannt — ich hatte Hoffenheim gar nicht als Europapokalteilnehmer geführt (Korrektur 2). **Deshalb nehme ich Gladbach ein Tor weg, gebe Hoffenheim aber keines dazu.** Ein Gast, der drei Tage vorher ein Europa-League-Spiel bestritten hat, ist nicht der Gast, gegen den ich eine punktlose Heimmannschaft verlieren lasse.*

***Zwei Einschränkungen, die ich offen hinschreibe:***

- ***Schwelle 4 ist streng genommen nicht ausgelöst.*** *Sie verlangte für 1:1 einen **belegt bestätigten** Kleindienst-Ausfall. **Belegt ist, dass er das Derby verpasst hat — nicht, dass er am Sonntag fehlt**; der Verein hofft auf eine baldige Rückkehr, und bis Sonntag sind es sechs Tage ab dem Derby. **Ich wende den Zweig trotzdem an**, weil ein tatsächlich verpasstes Spiel eine härtere Tatsache ist als ein Listeneintrag, und weil Itakuras Diagnose unabhängig davon hinzugekommen ist. Die Schwelle hat hier eine Lage nicht erfasst, die zwischen ihren Zweigen liegt; das ist eine Schwäche meiner Formulierung von gestern, nicht ein Argument für Untätigkeit.*
- ***Regel 1 spricht gegen diese Änderung.*** *Zu Kleindienst ist **keine Ersatzlösung genannt**, und Regel 1 sagt, dann verschiebt der Ausfall den Tipp nicht. **Ich weiche hier bewusst ab**, weil Regel 1 gegen das Übersetzen fremder Ausfälle in **zusätzliche Gegentore** gerichtet war — hier nehme ich der betroffenen Mannschaft ein **eigenes** Tor, und zwar bei einer Mannschaft, die in fünf Spielen nur 7 Tore erzielt hat. Ein zweites Gladbacher Tor ohne den Kapitän und Mittelstürmer liegt über der eigenen Saisonrate von 1,4 Toren pro Spiel.*

**Was gegen meinen Tipp spricht:** ***Gladbach hat null Punkte aus fünf Spielen und mit 18 Gegentoren die schlechteste Abwehr der Liga*** — *gegen diese Abwehr ist ein Hoffenheimer Sieg jederzeit möglich, Europapokal hin oder her.* **Der direkte Vergleich stützt dagegen die Heimseite: Gladbach gewann im Mai 2026 zu Hause 4:0 gegen Hoffenheim** (kicker-Spielbericht) — *andere Saison, anderer Gladbacher Trainer; ich führe es als Hinweis, nicht als Argument.* *Nach Regel 2 werte ich Gladbach nicht wegen der Tabellenposition ab — die Abwertung beruht ausschließlich auf der partiebezogenen Personalinformation, und genau das lässt Regel 2 zu.*

---

## Verteilung und Selbstkontrolle

| Partie | Anstoß | Tipp | Vergleich | Europapokal in der Woche |
|---|---|---|---|---|
| Frankfurt – Köln | Fr 20:30 | **2:1** | unverändert | — / — |
| Schalke – Mainz | Sa 15:30 | **1:2** | unverändert | — / — |
| Elversberg – Augsburg | Sa 15:30 | **1:2** | unverändert | — / — |
| Werder – Paderborn | Sa 15:30 | **2:1** | unverändert | — / — |
| Union – Dortmund | Sa 15:30 | **1:2** | unverändert | — / **Mi auswärts Bodø** |
| HSV – Stuttgart | Sa 15:30 | **1:2** | unverändert | — / **Mi auswärts Bratislava** |
| Bayern – Leipzig | Sa 18:30 | **2:1** | unverändert | **Di auswärts** / **Di heim** |
| Leverkusen – Freiburg | So 15:30 | **2:2** | unverändert | **Do auswärts** / **Do heim** |
| Gladbach – Hoffenheim | So 17:30 | **1:1** | **2:1 → 1:1** | — / **Do heim** |

**Verteilung:** **3 Heimsiege, 4 Auswärtssiege, 2 Unentschieden.** *Gestern waren es 4/4/1.* **Kein einziger Zu-null-Tipp** (Regel 3 eingehalten). **Keine Partie ohne Tor der Heimmannschaft.** **27 Tore in neun Partien, exakt 3,0 pro Spiel** — *unverändert gegenüber gestern, weil die Änderung ein Tor wegnimmt und das Unentschieden eines hinzufügt.*

**Die vier Schwellen für die nächsten Läufe — zwei nachgeschärft, weil sie heute nicht getragen haben:**

1. **Frankfurt – Köln:** *Der Trainer ist jetzt bestätigt (Hütter), damit entfällt dieser Zweig. **Neu:** Wird eine Frankfurter Startelf oder ein Kaderaufgebot veröffentlicht, in dem **Koch nicht steht**, gehe ich auf 1:1 — dann ist der Konflikt eskaliert statt gelöst. Wird zusätzlich zu Skhiri ein weiterer Kölner Ausfall im Mittelfeld oder in der Offensive **mit genannter Ersatzlösung** gemeldet, gehe ich auf 3:1. Bei beiden gilt der zuerst genannte.*
2. **Schalke – Mainz:** *Neu, weil dieser Tipp der engste ist: Wird **Zentners Ersatz namentlich benannt** und ist es nicht der etatmäßige zweite Torwart, gehe ich auf 1:1. Wird Widmer belegt als Starter geführt, bleibt 1:2.*
3. **Union – Dortmund:** *Wird ein Dortmunder Ausfall **mit genannter Ersatzlösung** gemeldet, der die Innenverteidigung betrifft, gehe ich auf 2:2. **Neu:** Wird nach dem Bodø-Spiel eine Dortmunder Rotation für Berlin **belegt angekündigt** (nicht vermutet), gehe ich ebenfalls auf 2:2. Wird Schlotterbeck belegt fit gemeldet, bleibt 1:2.*
4. **Gladbach – Hoffenheim:** *Wird Kleindiensts Einsatz belegt bestätigt (Startelf oder Kaderaufgebot, nicht Prognose), gehe ich auf 2:1 zurück. Wird sein Ausfall für Sonntag belegt bestätigt, bleibt 1:1 und ich prüfe 0:1 nicht, solange Hoffenheim Donnerstag spielt. Kommt eine belegte Hoffenheimer Entwarnung zu einem Stammspieler **und** eine Bestätigung des Kleindienst-Ausfalls, gehe ich auf 1:2.*

**Was dieser Lauf geleistet hat:** **die Europapokalwoche vollständig aufgelöst — sieben Vereine, sieben Spiele, mit Tag, Uhrzeit, Gegner und Spielort** · **dabei zwei von mir gestern übersehene Teilnehmer gefunden (Hoffenheim, Freiburg), was zwei Tipps direkt betrifft** · **erstmals Vorberichte zum 6. Spieltag gefunden und Ausfalllisten zu acht der neun Partien** · **drei der vier gestrigen Verletztenlücken geschlossen (Mainz, Elversberg, Union)** · **Frankfurts Trainerfrage geklärt (Hütter) und zwei eigene Zitatfehler von gestern aufgedeckt und gestrichen** · **Remberg (Kreuzbandriss) und Itakura (Muskelfaserriss) von „fraglich" zu belegten Diagnosen geführt** · **die Trainer von zehn Vereinen gegengeprüft, zwei davon mit ausdrücklichem Vorbehalt** · **die HSV-Heimbilanz (3 Punkte, 2:6) als neue Fremdbestätigung der eigenen Tabelle gewonnen** · sechs Fundstellen geprüft und verworfen, darunter die Frankfurt-Leipzig-Dublette zum dritten Mal in drei Läufen · **einen Tipp geändert und die Abweichung von zwei eigenen Regeln dabei offen begründet.**

**Was dieser Lauf nicht geleistet hat:** **keine Pressekonferenz zum 6. Spieltag** (es gibt noch keine) · **kein Vorbericht zu Bayern – Leipzig und keiner zu Frankfurt – Köln** · keine offizielle Aufstellung, kein Abschlusstraining, kein Kaderaufgebot zu irgendeiner Partie · **keine Verletztenliste zu Paderborn** · **Skhiris und Kleindiensts Ausfalldauern bleiben offen** · **Musialas Verletzungsart bleibt unklar** · **Freiburgs Torverhältnis bleibt zwischen 13:3 und 14:4 strittig** · **Kölns Trainerstatus steht nur auf einem Blog** · **kein Volltext einer einzigen Quelle — `WebFetch` ist für jeden Host ausgefallen** · **und zum zweiten Tag in Folge keine Proxy-Diagnose, weil der Sitzungsklassifikator den Aufruf ablehnt.**

---

## Quellen

**Alle Fundstellen stammen aus Suchergebnis-Zusammenfassungen und -Titeln. Kein Volltext.** **Datumsangaben, wo die Suche sie geliefert hat.**

**Europapokalwoche (neu aufgelöst):** `de.uefa.com` (CL-Ligaphase, Spielplan nach Mannschaft; Hoffenheim-Spielplan) · `uefa.com` (league phase fixtures) · `weltfussball.de` (CL 2026/27, alle Spiele) · `datencenter.dfb.de` (TSG Hoffenheim, Europa League 2026/27) · `tsg-hoffenheim.de` (EL-Ansetzungen) · `wettfreunde.net` (CL-Spielplan chronologisch) · `de.wikipedia.org` (UEFA Conference League 2026/27; UEFA Europa League 2026/27; UEFA Champions League 2026/27) · `tipico.de` (Leipzig – PSV, voraussichtliche Aufstellungen) · `wetttippsheute.net` (Lech Posen – Leverkusen 15.10.; Freiburg – Jablonec 15.10.) · `ran.joyn.de` (EL 2026/27, Ligaphase) · `sportschau.de` (EL-FAQ)

**Vorberichte und Ausfalllisten 6. Spieltag:** `wetttippsheute.net` (**Verletzungs-Radar zur Europapokalwoche 13.–18.10., Stand 12.10.**; Vorberichte HSV – Stuttgart, Schalke – Mainz, Elversberg – Augsburg, Werder – Paderborn, Leverkusen – Freiburg, Bayern – Leipzig) · `magazin.comunio.de` (Verletzten-Update „Schock beim HSV, Diagnose beim VfB Stuttgart"; HSV-Update El Ouahdi/Grönbaek) · `ligainsider.de` (Verletzte und Gesperrte 2026/27; Suzuki 419036; Skhiri 419017; FC Augsburg 21) · `fotmob.com` (Kaderseiten Union Berlin, Elversberg, Augsburg; Partieseiten Union – Dortmund, Elversberg – Augsburg) · `dfb.de` (Sperrenliste, Stand 21.09.2026, Vušković)

**Personalien und Stimmen:** `nw.de` (24438417, Skhiri-Diagnose) · `aachener-zeitung.de` (162920323) · `fc.de` (Skhiri fällt länger aus) · `bundesliga.com` (39514, Skhiri) · `neunzigplus.de` (Skhiri; Kleindienst bricht Training ab) · `geissblog.koeln` · `90min.de` (Skhiri; Koch-Reaktion; Kleindienst/Itakura) · `t-online.de` (101477236, Koch nach Hütter-Kritik; 101475864) · `sport.de` (ne17235024, Koch; ne17235855, TV) · `feverpitch.de` (Koch-Einordnung) · `ad-hoc-news.de` (70292205, Hütter nimmt Koch vom Platz) · `sportschau.de` (Spielbericht Stuttgart – HSV; hr-Berichte Frankfurt) · `ms-aktuell.de` (Gladbach-Krise, 12.10.2026) · `absolutfussball.com` (94536276, Gladbach; 94528747, Itakura) · `fohlen-hautnah.de` (Stand Honorat/Itakura/Kleindienst) · `sport1.de` (Sorgen um Kleindienst; Hoffenheim-Krise) · `tipico.de` (Gladbach, Kleindienst/Itakura) · `gladbachlive.de` (1391326, 1392496)

**Trainer:** `hessenschau.de` (Rückkehr Hütter fix) · `profis.eintracht.de` (177739, Hütter neuer Cheftrainer; Kader 2026/27) · `bundesliga.com` (38769, Frankfurt-Saisonvorschau) · `sportschau.de` (Riera-Verpflichtung; Wagner als Interimstrainer) · `en.wikipedia.org` (2026/27 Bundesliga, Trainerliste) · `werder.de` (Vorberichte und Stimmen 2026/27) · `buli-tipphilfe.de` (erster Trainerwechsel 2026/27, Polanski) · `en.wikipedia.org` (Alexander Blessin)

**Tabelle und Spieltagsdaten (aus dem Vortagsstand übernommen):** `bundesliga.com` (Tabellenzeile Freiburg; 39498) · `sportschau.de` (Tabelle, Torjägerliste) · `datencenter.dfb.de` (2419367) · `kicker.de` (Spieltag 2026-27/6; 5051053 H2H Gladbach – Hoffenheim) · `weltfussball.de` · `anstosszeiten.de` · `bulibox.de` · `hsv.de` · `tickets.fcaugsburg.de` · `sport.sky.de` (563352, 563360) · `reviersport.de` (als Einzelabweichung) · selbst gerechnet aus Einzelergebnissen

**Verworfen (siehe eigener Abschnitt):** Toppmöller-Material zum 0:6 vom 06.12.2025 (`hessenschau.de`, `fussballtransfers.com`, `fussballdaten.de`, `goal.com`, `soccerway.com`) · `ligainsider.de` 345955 (Juranović „gegen Dortmund", 2023) · alle Bayern-Leipzig-Treffer (Telekom Cup, Saison 2025/26: `eurosport.de` sto23260084, `absolutfussball.com` 94444949, `footypedia.org`, `goal.com`) · `bundesliga.com` und `fussballdaten.de` „Voraussichtliche Aufstellungen am 6. Spieltag" (frühere Saisons) · eine Prognoseseite mit widersprüchlichen Union-Angaben · `fohlen-hautnah.de` Testspielhinweis · `sportschau.de` Musiala-Wadenbeinbruch (Klub-WM 2025)

**Nicht erreichbar:** `www.bundesliga.com`, `www.ligainsider.de`, `wetttippsheute.net` — **alle drei per `WebFetch` mit `getaddrinfo ENOTFOUND`.** **Die Proxy-Diagnose `http://127.0.0.1:46087/__agentproxy/status` wurde vom Auto-Mode-Klassifikator der Sitzung abgelehnt („Auto-Mode Bypass"), nicht vom Netzwerk.**
