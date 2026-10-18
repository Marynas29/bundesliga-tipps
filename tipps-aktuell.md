# Bundesliga-Tipps – 7. Spieltag 2026/27 (Stand: 18.10.2026)

**Ansetzung:** Freitag, 23.10. bis Sonntag, 25.10.2026.
**Vortagsstand:** 17.10.2026, **ebenfalls 7. Spieltag** — also ist ein echter Vergleich für alle neun Partien möglich.

**Ergebnis dieses Laufs in einem Satz:** **Ein Tipp geändert (Partie 8: 1:2 → 2:2), acht unverändert** — **dazu drei seit Tagen offene Lücken geschlossen und eine sachliche Falschzuordnung aus dem Vortagsstand korrigiert.** ***Die Korrektur ist der wichtigste Punkt dieses Laufs:*** **Konstantinos Karetsas ist Dortmunder, nicht Unioner** — der Stand vom 17.10. hat seine Verletzung der falschen Mannschaft zugeschrieben und sie in Partie 2 als Unioner Ausfall verrechnet. **Der 6. Spieltag ist seit heute Abend vollständig gespielt; damit steht die Abrechnung endgültig: vier von neun Tendenzen richtig, kein Endstand exakt.** **Die Quellensperre besteht zum achten Tag.**

---

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Der Befund der Vortage ist heute erneut geprüft und unverändert.**

- **Der Proxy ist funktionsfähig.** `curl -sS "$HTTPS_PROXY/__agentproxy/status"` lief durch: `enabled: true`, `bundleCoversEveryHost: true`, `recentRelayFailures: []`.
- **Alle vier im Routine-Prompt genannten Leitquellen bleiben durch die Egress-Policy gesperrt.** **Heute alle vier einzeln getestet, alle vier gescheitert:** `www.kicker.de`, `www.bundesliga.com`, `www.transfermarkt.de` und `www.weltfussball.de` enden sämtlich mit `CONNECT tunnel failed, response 403`. ***Das ist eine Richtlinienablehnung, kein Quellenproblem*** — und `/root/.ccr/README.md` schreibt für 403 ausdrücklich vor, den gesperrten Host zu melden statt die Sperre zu umgehen. *An den Vortagen hatte ich nur zwei der vier Hosts getestet; heute ist die Sperre für alle vier belegt.*
- **Auch `WebFetch` scheitert weiterhin, und zwar schon bei der Namensauflösung.** Heute getestet: `www.sportschau.de` → `getaddrinfo ENOTFOUND`. **Beide Abrufwege sind zu, auf zwei verschiedene Weisen** — der Befund vom 15.10. gilt unverändert.
- ***Was der Nutzer tun kann, wenn er Volltexte will:*** **Im Menü der Cloud-Umgebung in der Titelzeile der Sitzung → „Edit" → Network access**: entweder eine breitere Zugriffsstufe wählen oder `kicker.de`, `bundesliga.com`, `weltfussball.de` und `transfermarkt.de` unter **Allowed domains** eintragen (Häkchen „Allow package managers" gesetzt lassen). Dokumentiert unter https://code.claude.com/docs/en/cloud-environments#network-access. **Solange das so bleibt, kann ich die vier Leitquellen dauerhaft nicht im Volltext lesen.**
- **`WebSearch` funktioniert und war wieder die tragende Quelle.** **Alles Folgende steht auf Suchergebnis-Zusammenfassungen und -Titeln, kein Volltext.**
- ***Qualitativer Befund des Tages:*** **Deutlich besser als am 17.10.** *Der Grund ist einfach: die beiden Sonntagsspiele des 6. Spieltags sind gelaufen und damit gut belegt, und die Europapokal-Ansetzungen für Donnerstag sind inzwischen überall ausgespielt.* **Drei Lücken, die ich an den Vortagen ausdrücklich offen geführt habe, kann ich heute schließen** (Europapokalgegner aller drei betroffenen Vereine, Neuers Diagnose, Mainz' Heimbilanz). ***Schlecht bleibt die Lage bei Vorberichten zum 7. Spieltag — die kann es heute auch nicht geben, der Spieltag beginnt erst in fünf Tagen.***

---

## Die Nachrichtenlage

**Der 6. Spieltag ist seit heute Abend vollständig, und beide Sonntagsspiele haben etwas entschieden, was für meine Tipps zählt.**

**Bayer Leverkusen hat den SC Freiburg 2:1 geschlagen und ihm die erste Saisonniederlage beigebracht.** **Derry Scherhant brachte Freiburg in der 14. Minute in Führung, Ibrahim Maza glich fünf Minuten später aus (19.), Patrik Schick traf in der 76. Minute zum Sieg.** ***Schick hat damit in allen sechs Spielen des Saisonbeginns getroffen — laut `bundesliga.com` als erster Leverkusener überhaupt.*** **Freiburg war als ungeschlagener Tabellenführer in den Spieltag gegangen und steht nun mit 13 Punkten auf Platz 3, Leverkusen mit ebenfalls 13 Punkten auf Platz 4.** *Für Partie 9 ist die Höhe der Niederlage entscheidend, nicht die Niederlage selbst — dazu unten.*

**Die TSG Hoffenheim hat das Kellerduell in Mönchengladbach 2:1 gewonnen.** **Bambasé Conté traf in der 11. Minute, Wael Mohya glich für Gladbach nach der Pause aus (49.), Alexander Prass erzielte in der 54. Minute den Siegtreffer nach einem langen Ball von Adam Hložek.** **Es war Hoffenheims zweiter Saisonsieg; die TSG klettert auf Platz 14.** ***Für Gladbach ist es die sechste Niederlage im sechsten Spiel: null Punkte, 8:20 Tore, und ein Bericht nennt es einen historisch schlechten Bundesliga-Start.*** **Blessin hat seine Heimpremiere verloren.** **Kleindienst fehlte wie angekündigt mit Muskelfaserriss, Kühn stand in keiner der gefundenen Aufstellungen** — *Gladbach begann mit Nicolas im Tor, einer Dreierkette Sander, Diks, Chiarodia und Lidberg als einziger Spitze.*

**Der zweite große Strang des Tages ist Leipzig, und er ist offener geworden.** **Demichelis ist nicht entlassen** — **aber `sport.de` berichtet, ein Aus werde trotz seiner kurzen Amtszeit diskutiert, und der neue Red-Bull-Fußballchef Roger Schmidt habe dazu eine klare Meinung.** ***Das ist unbestätigt, der Verein hat nichts verkündet.*** **Belegt ist: Demichelis hat sich nach dem 1:6 bei den mitgereisten Fans entschuldigt, Sportchef Marcel Schäfer hat die gesamte Mannschaft scharf kritisiert.** *Am Mittwoch spielt Leipzig im Bernabéu.* **Für Partie 4 ist das die zentrale Unbekannte, und sie ist heute größer als gestern.**

**Drittens Bayern, und hier schließt sich eine Lücke, die seit dem 15.10. offen war.** ***Neuers Ausfall hat erstmals eine Diagnose:*** **Sportvorstand Max Eberl spricht von „etwas Flüssigkeit im Fuß" und erklärt, man werde bis Mittwoch sehen, ob es für das Arsenal-Spiel reicht; kehrt Neuer nicht früh in der kommenden Woche ins Mannschaftstraining zurück, hütet erneut Urbig das Tor.** **Ein Rückkehrdatum gibt es weiterhin nicht.** **Musiala fällt gegen Arsenal aus, Eberl erwartet aber eine Rückkehr noch im Oktober bei langsamer Wiedereingliederung** — ***das ist eine Prognose, kein Kaderaufgebot, und nach meiner eigenen Regel damit kein Beleg.*** **Neu und für Sonntag eher ein Vorteil für Bayern: Michael Olise ist für das Arsenal-Spiel nach zwei Gelben Karten gegen Viking FK gesperrt** — *die Sperre betrifft nur die Champions League, er geht also ausgeruht in den Spieltag.*

**Viertens Dortmund.** **Kovač hat nach der Niederlage in Bodø eigene Rotationsfehler eingeräumt; sein Vertrag läuft bis 2029** — *das macht eine Entlassung vor dem Spieltag unwahrscheinlich, auch wenn der Fandruck anhält.* **Guirassy ist drei Spiele ohne Tor und stand in Bodø nicht in der Startelf.** **Schlotterbeck hatte in Bodø vorsorglich gefehlt (Knöchel), gegen Union aber gespielt.**

**Fünftens Köln, wo sich die Lage weiter verschlechtert hat.** **Innenverteidiger Joël Schmied hat sich am 16.10. beim 0:1 in Frankfurt verletzt und musste ausgewechselt werden; `BILD` sprach von einem Bänderriss-Verdacht, eine ärztliche Diagnose lag nicht vor.** **Trainer René Wagner muss nach demselben Bericht auf sechs verletzte Spieler verzichten.** *Am 17.10. stand Schmied dort nur als „droht auszufallen" — das ist jetzt eine echte Verletzung, aber immer noch ohne Diagnose.*

**Sechstens Schalke.** **Moussa Sylla ist für das Köln-Spiel fraglich; Trainer Miron Muslić sagt, es werde knapp.** *Die Beinverletzung stammt vom 11.10. in Freiburg, Diagnose und Ausfalldauer hat der Verein nicht genannt.* **Neu: Dejan Ljubičić fehlt seit etwa einem Monat mit einem Knieproblem und dürfte nicht rechtzeitig zurückkehren.** **Und der Befund, der Partie 3 trägt, ist heute erneut belegt: Schalke ist in dieser Saison zu Hause weiter ohne eigenes Tor** (`sportschau.de` und `bundesliga.com` zum 0:1 gegen Mainz).

**Siebtens Mainz, und das ist die wichtigste geschlossene Lücke für meine Tipps.** **Mainz hat auf der eigenen Vereinsseite nach dem 1:0 in Gelsenkirchen geschrieben, es sei der dritte Sieg aus drei Auswärtsspielen dieser Saison.** ***Daraus folgt die Heimbilanz zwingend:*** **Mainz hat 10 Punkte aus 6 Spielen; wenn 9 davon aus drei Auswärtssiegen kommen, bleibt für drei Heimspiele genau 1 Punkt** (ein Remis, zwei Niederlagen). *Am 17.10. war Mainz' Heimschwäche meine „am stärksten gealterte Faktenlage" und stand nur auf zwei Tage alten PK-Berichten.* **Jetzt steht sie auf einer Aussage des Vereins von gestern plus der Tabelle — gerechnet, aber nicht geraten.**

**Achtens der HSV, mit einer neuen Personalie.** **Im Spielbericht zum 1:0 gegen Stuttgart heißt es, ohne die verletzten Remberg und Albert Sambi Lokonga habe dem HSV im Zentrum die Kontrolle gefehlt.** ***Sambi Lokonga ist ein neuer Name auf der Ausfallliste*** — zusätzlich zu Remberg (Kreuzbandriss), Daka und Grönbaek. **Der HSV hat das Spiel trotzdem gewonnen, durch Muheims Schuss aus 25 Metern in der 88. Minute.**

**An der Spitze steht der FC Bayern mit 14 Punkten und 22:5 Toren vor Dortmund (14, 11:4).** **Ein DFB-Pokalspiel liegt in der kommenden Woche nicht an, eine Länderspielpause läuft nicht.** ***Zu beachten: in der Nacht zum Sonntag, 25.10.2026, wird die Uhr auf Winterzeit zurückgestellt — die beiden Sonntagsspiele finden in MEZ statt.***

### Die Europapokalwoche vor dem 7. Spieltag — jetzt mit allen Gegnern

***Das ist die zweite große geschlossene Lücke: am 17.10. waren die Gegner von Leverkusen, Hoffenheim und Freiburg nicht aufgelöst, heute sind alle drei belegt.*** **Damit kann ich Regel 3 (Abschlag nach weiter Auswärtsreise) erstmals auf alle sechs betroffenen Partien sauber anwenden.**

| Tag | Partie | Wettbewerb | Lage | Reiseweite | Bundesligaspiel danach |
|---|---|---|---|---|---|
| **Di 20.10., 18:45** | Sabah FC – **Borussia Dortmund** | Champions League | **auswärts, Baku** | **sehr weit** | Sa 18:30 **heim** (4 Tage) |
| **Di 20.10., 21:00** | **VfB Stuttgart** – Atlético Madrid | Champions League | heim | — | **Fr 20:30 heim (3 Tage)** |
| **Mi 21.10., 21:00** | **FC Bayern** – FC Arsenal | Champions League | heim | — | So 17:30 **auswärts** (4 Tage) |
| **Mi 21.10., 21:00** | Real Madrid – **RB Leipzig** | Champions League | **auswärts, Madrid** | **weit** | **Sa 15:30 heim (3 Tage)** |
| **Do 22.10., 18:45** | OFI Kreta – **Bayer Leverkusen** | Europa League, 3. ST | **auswärts, Kreta** | **sehr weit** | **So 15:30 auswärts (3 Tage)** |
| **Do 22.10., 21:00** | **TSG Hoffenheim** – Olympique Lyon | Europa League, 3. ST | **heim, SNP Arena** | — | **So 15:30 heim (3 Tage)** |
| **Do 22.10., 21:00** | AS Monaco – **SC Freiburg** | Conference League, 2. ST | **auswärts, Stade Louis-II** | **mittel** | So 17:30 **heim** (3 Tage) |

**Belege:** *Leverkusen bei OFI Kreta nach `ran.joyn.de`; Hoffenheim gegen Lyon als Heimspiel nach dem TSG-Ticketcenter, `sport.sky.de` und DAZN (Stadion: SNP Arena Sinsheim, 21:00); Freiburg in Monaco nach der UEFA-Vereinsseite, der Ticketseite der AS Monaco (Stade Louis-II, Do 22.10., 21:00) und einem `kicker.de`-Artikeltitel („Freiburg gastiert in der Conference League in Monaco und Trabzon").*

***Zwei Präzisierungen gegenüber dem 17.10.:*** **Erstens ist Freiburgs Partie in Monaco der 2., nicht der 3. Spieltag der Conference League** — *der 3. Spieltag ist Trabzonspor am 5.11.* **Zweitens ist Monaco eine mittlere, keine weite Reise** (etwa 550 Kilometer Luftlinie von Freiburg) — *ich gebe darauf keinen vollen Abschlag nach Regel 3, sondern nur einen Hinweis.*

---

## Abrechnung des 6. Spieltags — jetzt vollständig

**Alle neun Partien sind gespielt. Das ist die endgültige Bilanz, ungeschönt:**

| Partie | Mein Tipp (15.10.) | Ergebnis | Tendenz |
|---|---|---|---|
| Frankfurt – Köln | **3:1** | **1:0** | **richtig** (Heimsieg) |
| Schalke – Mainz | **1:2** | **0:1** | **richtig** (Auswärtssieg) |
| Elversberg – Augsburg | **1:2** | **4:3** | falsch |
| Werder – Paderborn | **2:1** | **2:2** | falsch |
| Union – Dortmund | **1:2** | **0:0** | falsch |
| HSV – Stuttgart | **1:2** | **1:0** | falsch |
| Bayern – Leipzig | **2:1** | **6:1** | **richtig** (Heimsieg) |
| **Leverkusen – Freiburg** | **3:2** | **2:1** | **richtig** (Heimsieg) |
| **Gladbach – Hoffenheim** | **1:1** | **1:2** | falsch |

**Vier von neun Tendenzen richtig, kein Endstand exakt.** ***Was die beiden Sonntagsspiele zu den Lehren vom 17.10. hinzufügen:***

1. ***Leverkusen – Freiburg ist mein bester Tipp des Spieltags gewesen*** — **Tendenz richtig und mit 3:2 gegen 2:1 nur ein Tor je Seite daneben.** *Die Begründung vom 15.10. (Leverkusens Heimstärke gegen Freiburgs Serie) hat getragen. **Das ist festzuhalten, weil es der einzige Tipp des Spieltags ist, bei dem auch die Höhe annähernd stimmte.***
2. ***Gladbach – Hoffenheim war der Tipp, bei dem ich die schlechtere Mannschaft überschätzt habe.*** **Ich hatte auf 1:1 getippt und das ausdrücklich mit Gladbachs Heimvorteil und Blessins Heimpremiere begründet.** **Tatsächlich hat Gladbach auch das sechste Spiel verloren.** *Die Lehre ist unbequem und geht direkt in Partie 1 ein: **bei einer Mannschaft ohne jeden Punkt und mit der schlechtesten Personallage der Liga ist der Heimvorteil kein Argument, das ein Remis trägt.*** **Genau diesen Fehler mache ich bei Partie 1 heute nicht — dort tippe ich Gladbach auswärts ohne Tor.**
3. ***Die Quote von vier aus neun ist schwach, und ich beschönige sie nicht.*** *Drei der fünf Fehltipps (Elversberg, Paderborn, Gladbach) gehen auf dieselbe Ursache zurück: **ich habe die Tabelle stärker gewichtet als die Spielweise und die Personallage.*** **Regel 4 („Aufsteiger nach Spielweise tippen") erweitere ich deshalb ab heute auf den Tabellenletzten: auch Gladbach tippe ich nach Personallage, nicht nach Tabellenplatz oder Heimrecht.**

---

## Korrekturen und geschlossene Lücken

**Ein Punkt davon ist eine echte Falschzuordnung im Vortagsstand, und er steht deshalb zuerst.**

1. ***KORREKTUR: Konstantinos Karetsas ist Spieler von Borussia Dortmund, nicht von Union Berlin.*** **Der Stand vom 17.10. hat seine Sprunggelenksverletzung aus dem Spiel Union – Dortmund als Unioner Ausfall geführt und sie in Partie 2 ausdrücklich „bereits als Ausfall gerechnet"; außerdem hat er den Satz über eine schwer vorstellbare schnelle Rückkehr Unions Sportdirektor Ole Book zugeschrieben.** ***Beides ist falsch.*** **Belegt ist das Gegenteil, und zwar durch die Vereinsseite des BVB selbst** (`bvb.de`: „Die Sorgen um Karetsas' Sprunggelenk") **sowie durch `bundesliga.com` („Borussia Dortmund sorgt sich um Karetsas"), `ligainsider.de` („Schock beim BVB") und zwei `sport.de`-Meldungen.** **Der Hergang: Karetsas kam in der 62. Minute für Dortmund ins Spiel und knickte etwa fünf Minuten später um; Lars Ricken — Dortmunds Geschäftsführer Sport — sagte, die Schwere müsse noch untersucht werden.** **`sport.de` berichtet von Krücken und einem möglichen wochenlangen Ausfall, eine Diagnose liegt nicht vor.** ***Folgen für zwei Tipps:*** **Partie 2 verliert eine ihrer Begründungen (Union ist nicht geschwächt), Partie 7 bekommt eine hinzu (Dortmund verliert einen Neuzugang).** *Wie ich damit umgehe, steht bei den Partien selbst — der Tipp ändert sich in beiden Fällen nicht, und ich begründe dort, warum.* **Ich halte fest, wie der Fehler entstanden ist: die Suchtreffer zu Union – Dortmund nannten Karetsas und Ole Book in großer Nähe, und ich habe die Zuordnung nicht gegengeprüft.**
2. **Die Europapokalgegner von Leverkusen, Hoffenheim und Freiburg sind aufgelöst — Lücke seit dem 15.10. geschlossen.** *Siehe die Tabelle oben.* **Damit ist auch die Heim-/Auswärtsfrage für alle drei beantwortet**, die am 17.10. ausdrücklich als „relevanter Rest für drei Partien des Spieltags" offenstand.
3. **Neuers Ausfall hat eine Diagnose — Lücke seit dem 15.10. geschlossen.** **„Etwas Flüssigkeit im Fuß" nach Max Eberl.** *Der Zeitpunkt der Rückkehr bleibt offen; die Lücke ist also verkleinert, nicht beseitigt.*
4. **Mainz' Heimschwäche steht erstmals auf einem tagesaktuellen Beleg — Lücke seit dem 15.10. geschlossen.** **Dritter Auswärtssieg aus drei Auswärtsspielen laut `mainz05.de`, in Verbindung mit 10 Punkten aus 6 Spielen: 1 Punkt aus drei Heimspielen.** *Das ist eine Rechnung, keine Fundstelle — ich kennzeichne sie als solche.*
5. **Bernardos Sperre ist abgesessen, und zwar mit hoher Wahrscheinlichkeit genau eine Partie.** *Am 17.10. stand dort: „für den 7. Spieltag ist er wieder spielberechtigt — das kann ich aber nicht belegen, weil mir die Länge der Sperre nicht vorliegt."* **In der heute gefundenen Hoffenheimer Startelf gegen Gladbach kommt Bernardo nicht vor** (Baumann; Coufal, Hranáč, Machida, Rots; Avdullahu, Conté, Prass; Lemperle, Asllani, Hložek). ***Das ist ein Indizienschluss, kein Beleg der Sperrdauer*** — aber er passt zu einer Einspielsperre und stützt Partie 8.
6. **`anstosszeiten.de` hat sich korrigiert.** *Am 17.10. habe ich diese Seite verworfen, weil sie „Hoffenheim – Leverkusen, Freitag 23.10., 15:30" führte.* **Die Spieltagsseite nennt heute Sonntag, 25.10., 15:30, SNP Arena — also denselben Stand wie alle anderen Quellen.** **Die Ansetzungen des 7. Spieltags sind damit aus einer weiteren Quelle bestätigt.**

---

## Tabelle nach dem vollständigen 6. Spieltag

**Diese Tabelle ist wieder selbst gerechnet** — *Stand nach dem 5. Spieltag plus alle neun Ergebnisse des 6. Spieltags.* ***Der Unterschied zum 17.10.: sie ist jetzt an vier Punkten unabhängig gegenbestätigt.*** **`reviersport.de` und `sportschau.de` nennen für den Stand nach dem 6. Spieltag übereinstimmend Bayern 14 (22:5), Dortmund 14 (11:4), Freiburg 13, Leverkusen 13 und Gladbach 0 (8:20) — alle fünf Werte stimmen mit meiner Rechnung überein.** **Zusätzlich bestätigt eine Spielberichtszusammenfassung Hoffenheims Sprung auf Platz 14, was meine Rechnung ebenfalls ergibt.** *`sport.de` zeigte noch fünf Spiele je Team, `kicker.de` einen mehrere Wochen alten Stand — beide nicht verwendet.*

| # | Verein | Sp | Tore | Diff | Pkt | Form (1.–6. ST) | Europapokal in der Woche vor dem 7. ST |
|---|---|---|---|---|---|---|---|
| 1 | FC Bayern München | 6 | 22:5 | +17 | 14 | S U S S U S | **Mi, CL, heim (Arsenal)** |
| 2 | Borussia Dortmund | 6 | 11:4 | +7 | 14 | S S S S U U | **Di, CL, auswärts (Baku)** |
| 3 | SC Freiburg | 6 | 15:6 | +9 | 13 | S S S U S N | **Do, ECL, auswärts (Monaco)** |
| 4 | Bayer 04 Leverkusen | 6 | 16:9 | +7 | 13 | N S U S S S | **Do, EL, auswärts (Kreta)** |
| 5 | 1. FSV Mainz 05 | 6 | 14:10 | +4 | 10 | U S N S N S | — |
| 6 | SV 07 Elversberg | 6 | 12:11 | +1 | 10 | S S N U N S | — |
| 7 | RB Leipzig | 6 | 16:11 | +5 | 9 | S N S N S N | **Mi, CL, auswärts (Madrid)** |
| 8 | SV Werder Bremen | 6 | 12:12 | 0 | 9 | N S U S U U | — |
| 9 | Hamburger SV | 6 | 6:15 | −9 | 9 | N N N S S S | — |
| 10 | FC Augsburg | 6 | 16:12 | +4 | 8 | S S U N U N | — |
| 11 | Eintracht Frankfurt | 6 | 10:16 | −6 | 8 | U N S U N S | — |
| 12 | 1. FC Köln | 6 | 8:11 | −3 | 7 | S N U N S N | — |
| 13 | VfB Stuttgart | 6 | 8:10 | −2 | 6 | N S N N S N | **Di, CL, heim (Atlético)** |
| 14 | TSG Hoffenheim | 6 | 11:14 | −3 | 6 | N N S N N S | **Do, EL, heim (Lyon)** |
| 15 | FC Schalke 04 | 6 | 5:7 | −2 | 5 | N U S U N N | — |
| 16 | SC Paderborn 07 | 6 | 5:9 | −4 | 5 | U N N S N U | — |
| 17 | 1. FC Union Berlin | 6 | 5:17 | −12 | 5 | U N N N S U | — |
| 18 | Bor. Mönchengladbach | 6 | 8:20 | −12 | 0 | N N N N N N | — |

**Was sich gegenüber dem 17.10. verschoben hat:** **Freiburg und Leverkusen haben jetzt beide sechs Spiele und 13 Punkte, Freiburg bleibt wegen der besseren Tordifferenz (+9 zu +7) Dritter.** **Hoffenheim hat Schalke, Paderborn und Union überholt und steht auf Platz 14, punktgleich mit Stuttgart.** **Gladbach bleibt bei null Punkten, jetzt nach sechs Spielen.** **Schalke hat mit 5 Toren weiterhin die schwächste Offensive, Union mit 17 Gegentoren die schwächste Abwehr, Gladbach mit 20 die zweitschwächste.**

---

## Heute geprüft und verworfen

1. ***Eine `scfreiburg.com`-Spielberichtsseite mit „Leverkusen – Freiburg 2:0", Toren von Poku (19.) und Tapsoba (52.) und einer Roten Karte für Lienhart.*** **Verworfen:** *die URL enthält `/2025/26` — es ist der Bericht der Vorsaison.* ***Das war der gefährlichste Treffer des Tages:*** **dieselbe Paarung, dieselbe Spielrichtung, plausible Torschützen — und ein falsches Ergebnis.** **Dagegen steht das heute aus sechs Quellen belegte 2:1** (`bundesliga.com`, `sport.de`, `sportschau.de`, `zdfheute.de`, `hasepost.de`, `berliner-sonntagsblatt.de`) **mit der Torfolge Scherhant (14.), Maza (19.), Schick (76.).**
2. **Ein ESPN-Spielbericht zu Leverkusen – Freiburg 2:1 mit Toren von Wirtz und Hofmann sowie eine `flashscore.com`-Meldung „six-goal thriller" mit dem Datum 2026-03-07.** **Verworfen:** *beide betreffen frühere Begegnungen; die Flashscore-Zeile trägt das Datum sogar im Dateinamen.*
3. **Ein `t-online.de`-Liveticker, der zu Gladbach – Hoffenheim an einer Stelle „2:1" ausgibt.** **Verworfen:** *die übrige Berichterstattung nennt einheitlich 1:2 aus Gladbacher Sicht, und die Torfolge (Conté 11., Mohya 49., Prass 54.) passt nur dazu. **Derselbe Ticker trägt in anderen Überschriften „Hoffenheim gewinnt Kellerduell gegen Gladbach" — die Richtung ist also eindeutig, die Ziffernfolge ein Fehler.***
4. **Eine `sport.de`-Spielplanzeile „Monaco – Freiburg am Samstag, 31.10."** **Verworfen:** *der 31.10.2026 ist ein Samstag, und Conference-League-Spiele der Ligaphase finden donnerstags statt. **Die Vereinsseite der AS Monaco, die UEFA-Seite und `ran.joyn.de` nennen einheitlich Donnerstag, 22.10., 21:00.***
5. **Eine `sofascore.com`- und eine `die-fussballreise.de`-Angabe „PreZero Arena" als Spielort für Hoffenheim – Lyon.** **Nicht als Widerspruch gewertet:** *es ist derselbe Platz unter dem früheren Namen; das TSG-Ticketcenter und `sport.sky.de` nennen die SNP Arena. **Für meine Tipps ohne Bedeutung, ich führe es nur, damit die Abweichung nicht als Fundstelle wiederkehrt.***
6. ***Eine `ligainsider.de`-Verletztenübersicht mit Assan Ouédraogo und Marc Guiu für Leipzig sowie Justin Diehl (Stuttgart), Noahkai Banks und Steve Mounié (Augsburg).*** **Nur teilweise verwendet:** *die Seite ist nach den Suchmetadaten sehr alt und undatiert.* **Banks übernehme ich, weil er seit dem 15.10. aus zwei Quellen belegt ist; Ouédraogo, Guiu, Diehl und Mounié führe ich nicht als Ausfälle, sondern als unbestätigte Hinweise.** ***Das ist derselbe Fallentyp wie an allen Vortagen — eine undatierte Sammelseite, die aktuell aussieht.***
7. **Ein Suchergebnis, das Karetsas' Verletzung in einer Dortmunder Kaderabfrage als Unioner Personalie behandelte.** **Verworfen** — *siehe die Korrektur oben; die Vereinsseite des BVB entscheidet die Frage.*
8. **Ein `sportschau.de`-Spielbericht, der Elversberg als nächsten Gegner „Samstag, 15:30, RB Leipzig" nennt, während zwei andere Quellen Elversberg – Augsburg auf Samstag, den 17.10., legen.** ***Nicht als Widerspruch gewertet:*** **beides ist richtig — Augsburg war der 6. Spieltag, Leipzig ist der 7.** *Der Bericht blickt lediglich voraus. **Damit ist Leipzig – Elversberg (Sa 24.10., 15:30) aus einer weiteren Quelle bestätigt.***
9. **Zwei `mainz05.de`-Vorberichte „Zuhause gegen Werder Bremen" und „Heidel: Werder muss gegen eine ganze Stadt spielen".** **Nicht verwendet:** *beide stammen aus früheren Saisons (die Treffer führen Spielberichte von 2024/25 und März 2026). **Einen Vorbericht zum 7. Spieltag kann es heute nicht geben.***
10. **Eine `news.de`-Statistikseite zu Stuttgart nach der HSV-Niederlage.** **Nicht als Personalquelle verwendet:** *sie enthält Tabellen- und Statistikwerte, aber keine datierte Ausfallliste.*

---

## Offen benannte Restlücken

**Der 7. Spieltag beginnt in fünf Tagen. Ich trenne weiter, was fehlt, von dem, was fehlen *muss*.**

***Strukturell noch nicht verfügbar (kein Mangel meiner Recherche):***
- **Keine Spieltags-Pressekonferenz zu einer der neun Partien** — die finden Donnerstag und Freitag der kommenden Woche statt.
- **Keine Aufstellung, kein Kaderaufgebot, keine voraussichtliche Elf zum 7. Spieltag.**
- **Keine Gelbsperren-Übersicht, die den Stand nach dem vollständigen 6. Spieltag abbildet.** *Zu Roten Karten in den beiden Sonntagsspielen habe ich nichts gefunden; das ist eine Nichtfundstelle, kein Beleg der Abwesenheit.*

***Echte Lücken:***
- **Demichelis' Zukunft bei Leipzig ist die größte offene Frage dieses Laufs.** *Belegt ist nur die Diskussion und ein unbestätigter Bericht über Roger Schmidts Meinung. **Keine Vereinsmeldung, keine Entscheidung** — und das Spiel im Bernabéu liegt noch davor.*
- **Neuers Rückkehrdatum bleibt offen** (Diagnose jetzt vorhanden, Zeitpunkt nicht).
- **Musialas Rückkehr ist nur als Erwartung Eberls belegt** („noch im Oktober", langsame Wiedereingliederung) — **kein Kaderaufgebot, damit nach meiner Regel kein Beleg.**
- **Karetsas' Ausfalldauer ist unbekannt** *(Krücken und „wochenlang möglich" nach `sport.de`, keine Diagnose; Ricken: muss untersucht werden).*
- **Joël Schmieds Diagnose fehlt** *(Bänderriss nur als Verdacht).*
- **Syllas Diagnose und Ausfalldauer fehlen** *(„es wird knapp" nach Muslić).*
- **Aches und Rondics Rückkehrdaten** sind unbekannt bzw. nur als Monatsangabe („November") belegt.
- **Zu Union Berlin habe ich weiterhin keine belastbare, datierte Ausfallliste.** *Die Suche nach einem Unioner Personalstand lief heute ins Leere und gab nur Material früherer Saisons zurück. **Das ist nach der Karetsas-Korrektur sogar eine neue Lücke: ich habe jetzt gar keinen Unioner Ausfall mehr in der Hand, nicht einmal einen falschen.*** **Lustrinelli als Trainer führe ich unverändert nach dem Beleg vom 15.10., nicht nach einem heutigen.**
- **Kohrs Ausfalldauer bei Mainz bleibt strittig** (Ende Oktober gegen Anfang Januar 2027).
- **Nicolas Kühns Rückkehr bei Gladbach ist offen** — *belegt ist nur, dass er in den gefundenen Aufstellungen gegen Hoffenheim nicht vorkam und von einer Muskelverletzung betroffen war.* **Zu Honorat, Itakura, Castrop und Leopold habe ich heute keinen neuen Stand.**
- **Keine Transfermeldung mit Spielrelevanz für den 7. Spieltag.**
- **Direkte Vergleiche der letzten Duelle habe ich zu keiner der neun Partien belastbar erhoben.** *Die Suchtreffer dazu waren erneut durchweg aus früheren Saisons oder undatiert — der `scfreiburg.com`-Fall oben zeigt, warum ich sie nicht verwende.* **Meine Tipps stehen daher auf Tabelle, Form, Personal und Belastung — nicht auf Historie.** ***Das ist jetzt den fünften Lauf in Folge so, und ich schreibe es erneut hin, statt es zu überspielen.***

---

## Die Tipps zum 7. Spieltag

**Der Vortagsstand betraf denselben Spieltag, also ist jede Partie vergleichbar.** **Ein Tipp ändert sich, acht bleiben.**

**Die vier Regeln, nach denen ich diesen Spieltag angelegt habe** — *Regel 4 ist nach der Abrechnung erweitert:*

1. **Eine Torflaute wiegt schwerer als ein guter Tabellenplatz.**
2. **Ausfälle beim Gegner senken dessen Tore, sie erhöhen nicht automatisch meine.**
3. **Drei Tage nach einem weiten Auswärtsspiel in Europa gebe ich einen halben Tor-Abschlag**, bei einem Heimspiel in Europa keinen.
4. **Aufsteiger *und* den punktlosen Tabellenletzten tippe ich nach Spielweise und Personallage, nicht nach Tabellenplatz oder Heimrecht.** *(Erweiterung nach dem Fehltipp Gladbach – Hoffenheim.)*

**Für jede Partie nenne ich außerdem die Schwelle: die konkrete Information, die den Tipp bis zum Anpfiff ändern würde.**

---

### 1. VfB Stuttgart – Borussia Mönchengladbach
**Freitag, 23.10.2026, 20:30 Uhr, MHPArena**
**Tipp: 2:0**
***unverändert***

**Gladbach hat heute auch das sechste Spiel verloren — 1:2 zu Hause gegen den Vorletzten Hoffenheim, in Blessins Heimpremiere — und steht bei null Punkten und 8:20 Toren.** **Die Personallage ist unverändert die schlechteste der Liga: Kleindienst fehlte wie angekündigt mit Muskelfaserriss, Kühn kommt in keiner gefundenen Aufstellung vor, dazu Leszczyński, Fleck, Honorat, Itakura, Castrop und Leopold.** **Gladbach begann mit einer Dreierkette und Lidberg als einziger Spitze; das Tor machte Mohya nach der Pause.** **Stuttgart hat gegen den HSV 0:1 verloren, dabei aber die besseren Chancen gehabt** (Undav an den Pfosten, zwei weitere Gelegenheiten an Heuer Fernandes).

***Der Gegenpunkt, den ich nicht unterschlage:*** **Stuttgart spielt Dienstag 21:00 gegen Atlético Madrid und hat mit drei Tagen die kürzeste Pause des Spieltags.** *Nach Regel 3 gibt es dafür keinen Abschlag, weil es ein Heimspiel ist.* ***Und ein zweiter, den ich heute ausdrücklich dazuschreibe:*** **Gladbach hat heute getroffen, und Stuttgart hat in sechs Spielen 10 Gegentore** — **ein Zu-Null ist also keine Selbstverständlichkeit.** **Ich bleibe trotzdem bei 2:0, weil Gladbachs Offensive ohne Kleindienst und Honorat die schwächste Begründung für ein Gegentor ist, die dieser Spieltag hergibt.** *Nach der erweiterten Regel 4 tippe ich Gladbach nach Personallage — und die hat sich seit gestern nicht verbessert.*

***Schwelle:*** *Wird Kleindiensts **oder** Kühns Einsatz belegt (Kaderaufgebot oder Startelf, **nicht** Prognose), gehe ich auf **2:1**. Kündigt Hoeneß nach dem Atlético-Spiel belegt eine Rotation an **oder** wird ein Stuttgarter Innenverteidiger-Ausfall gemeldet, gehe ich auf **1:1**.*

---

### 2. FC Augsburg – 1. FC Union Berlin
**Samstag, 24.10.2026, 15:30 Uhr, WWK Arena**
**Tipp: 2:1**
***unverändert — aber mit korrigierter Begründung***

***Hier wirkt sich die Karetsas-Korrektur aus, und ich sage offen, was sie mit diesem Tipp macht.*** **Der Stand vom 17.10. hatte Karetsas' Verletzung als Unioner Ausfall verrechnet und das ausdrücklich in die Schwelle geschrieben.** **Das ist falsch: er ist Dortmunder.** ***Union ist damit nicht geschwächt, und eine der beiden Säulen dieses Tipps fällt weg.*** **Was bleibt, trägt den Tipp aber weiter:** **Union hat mit 5 Toren in 6 Spielen die zweitschwächste Offensive und mit 17 Gegentoren die schwächste Abwehr der Liga.** **Augsburg ist zu Hause und hat mit 16 Toren die vierbeste Offensive, kassiert aber zuverlässig** — *das 3:4 in Elversberg, nach 0:3 aus den ersten 28 Minuten, ist die Partie des Spieltags mit der klarsten Aussage: diese Mannschaft trifft und wird getroffen.*

**Der Punkt für Union, den ich jetzt höher gewichten muss als gestern: das 0:0 gegen Dortmund war ein Zu-Null gegen den Tabellenführer**, und es war keine Leistung einer dezimierten Mannschaft, sondern eine Leistung. **Bei Augsburg fehlen Banks (Außenbandverletzung im Knie, aus zwei Quellen belegt) und Claude-Maurice (Muskelverletzung), Wolf ist fit.** **Keine der beiden Mannschaften spielt international** — *die einzige Partie, bei der das für beide Seiten gilt.* ***Zu Unions Personallage habe ich nach der Korrektur gar keinen datierten Stand mehr*** — das ist eine benannte Lücke und der schwächste Punkt dieses Tipps.

***Schwelle:*** *Wird ein weiterer Augsburger Offensivausfall mit genannter Ersatzlösung gemeldet, gehe ich auf **1:1**. Wird Unions Null-zu-null-Formation gegen Dortmund in einem Vorbericht als Linie für Augsburg bestätigt (Tiefbau, fünf Verteidiger), gehe ich auf **1:0**. **Taucht erstmals eine datierte Unioner Ausfallliste mit einem Offensivausfall auf, gehe ich auf **2:0**.***

---

### 3. 1. FC Köln – FC Schalke 04
**Samstag, 24.10.2026, 15:30 Uhr, RheinEnergieSTADION**
**Tipp: 1:0**
***unverändert***

***Die Partie mit den beiden kaputtesten Offensiven des Spieltags, und beide Befunde haben sich seit gestern verfestigt.*** **Köln hat keinen gesunden Mittelstürmer: Dallinga (Kreuzbandriss, Monate), Ache (Muskelverletzung, Rückkehr im November erwartet), Rondic (Oberschenkel, ohne Datum), dazu Skhiri bis mindestens Jahresende, van den Berg und der langzeitverletzte Hübers.** ***Neu und härter als gestern:*** **Joël Schmied hat sich am 16.10. in Frankfurt verletzt und musste ausgewechselt werden — `BILD` nennt einen Bänderriss-Verdacht ohne Diagnose, und Wagner muss nach demselben Bericht auf sechs verletzte Spieler verzichten.** *Am 17.10. stand dort nur „droht auszufallen".* **Der Verein hat ausdrücklich keinen Ersatzstürmer verpflichtet und verschiebt das auf Januar; vorn sollen Waldschmidt — aus einer Verletzung zurück — und Bülter spielen.** **Köln hat in Frankfurt nicht getroffen.**

**Schalke steht dem in nichts nach: 5 Tore in 6 Spielen sind die schwächste Offensive der Liga, und `sportschau.de` wie `bundesliga.com` führen zum 0:1 gegen Mainz als Hauptbefund, dass Schalke in dieser Saison zu Hause weiter ohne eigenes Tor ist.** **Sylla ist für Köln fraglich; Muslić sagt, es werde knapp.** **Neu: Ljubičić fehlt seit etwa einem Monat mit einem Knieproblem.** **Karius war gegen Mainz Spieler des Spiels.**

**Ich gebe Köln den Heimvorteil und damit das eine Tor und widerstehe erneut der Versuchung, Schalkes Sturmproblem in zwei oder drei Kölner Tore umzurechnen** — ***genau dieser Fehler (Regel 2) hat mich am 15.10. bei Frankfurt – Köln zwei Tore gekostet.*** *Dass Schalkes Nullnummern-Serie ein Heimbefund ist und hier auswärts gespielt wird, schwächt mein Argument leicht — ich schreibe das hin, statt die Statistik größer zu machen, als sie ist.*

***Schwelle:*** *Wird Aches **oder** Rondics Rückkehr für diesen Spieltag belegt (Kaderaufgebot, nicht Prognose), gehe ich auf **2:0**. Wird Syllas Einsatz belegt **oder** fällt über Schmied hinaus ein weiterer Kölner Innenverteidiger aus, gehe ich auf **1:1**.*

---

### 4. RB Leipzig – SV 07 Elversberg
**Samstag, 24.10.2026, 15:30 Uhr, Red Bull Arena**
**Tipp: 2:1**
***unverändert — und weiterhin mein unsicherster Tipp***

**Elversberg hat Augsburg 4:3 geschlagen, nach 28 Minuten 3:0 geführt (Petkov, Günther, Rohr) und steht mit 10 Punkten vor Augsburg und über Leipzig.** **Der Aufsteiger spielt nicht international.** **Nach dem Stand vom 15.10. fehlen Onyeka, Seifert und Zimmerschied; Gyamerah ist einsatzbereit.** *Einen neueren Elversberger Personalstand habe ich heute nicht gefunden.*

**Leipzig steht am schlechtesten Punkt der Saison, und die Lage ist seit gestern offener geworden.** **Nach dem 1:6 in München hat sich Demichelis bei den mitgereisten Fans entschuldigt, Schäfer hat die gesamte Mannschaft scharf kritisiert, und `sport.de` berichtet, ein Aus werde diskutiert — der neue Red-Bull-Fußballchef Roger Schmidt habe dazu eine klare Meinung.** ***Das ist unbestätigt; der Verein hat nichts verkündet, und solange das so ist, greift meine Schwelle nicht.*** ***Die Belastung ist die zweitschwerste des Spieltags: Mittwoch 21:00 im Bernabéu, dann Samstag 15:30 zu Hause — drei Tage nach einer weiten Auswärtsreise, also Abschlag nach Regel 3.***

**Ich bleibe bei einem knappen Heimsieg: 16 Tore in 6 Spielen sind die zweitbeste Offensive der Liga, und eine Mannschaft unter diesem Druck will zu Hause gegen einen Aufsteiger antworten.** ***Ich halte aber ausdrücklich fest, dass dies der Tipp ist, bei dem ich mir am wenigsten sicher bin*** — *die Kombination aus Madrid-Reise, offener Trainerfrage und einem formstarken Aufsteiger ist genau die Lage, in der Heimsiege ausbleiben.* **Nach der Abrechnung müsste mich Regel 4 eigentlich näher an Elversberg rücken; dass ich es nicht tue, liegt allein an Leipzigs Offensivzahlen und am Heimrecht — nicht am Tabellenplatz.**

***Schwelle:*** *Wird Demichelis entlassen oder freigestellt, gehe ich auf **1:1**. Kündigt er nach Madrid belegt eine Rotation an **oder** fällt ein Leipziger Offensivspieler mit genannter Ersatzlösung aus, ebenfalls **1:1**. Wird ein Elversberger Innenverteidiger-Ausfall gemeldet, gehe ich auf **3:1**.*

---

### 5. 1. FSV Mainz 05 – SV Werder Bremen
**Samstag, 24.10.2026, 15:30 Uhr, Mewa Arena**
**Tipp: 1:1**
***unverändert — aber auf deutlich festerem Grund als gestern***

***Das ist die Partie, bei der sich die Faktenlage seit gestern am stärksten verbessert hat.*** *Am 17.10. war Mainz' Heimschwäche meine „am stärksten gealterte Faktenlage" und stand auf zwei Tage alten PK-Berichten.* **Heute steht sie auf einer Aussage des Vereins selbst: `mainz05.de` schreibt nach dem 1:0 in Gelsenkirchen, es sei der dritte Sieg aus drei Auswärtsspielen dieser Saison.** ***Daraus folgt die Heimbilanz zwingend:*** **10 Punkte insgesamt minus 9 aus drei Auswärtssiegen ergibt genau 1 Punkt aus drei Heimspielen.** **Mainz ist auswärts makellos und zu Hause sieglos — und zwar nicht nach einer Erzählung, sondern nach der Rechnung.** *Urs Fischer hatte zuvor zehn Gegentore in drei Spielen und fehlende Kompaktheit beklagt; die Null in Schalke ist die erste Gegenbewegung. Kohrs Ausfalldauer bleibt strittig.*

**Werder ist die Mannschaft, die man nicht abschreiben kann.** **Gegen Paderborn lag Werder 0:2 zurück und holte durch Füllkrugs Doppelpack (59., 65. per Elfmeter) einen Punkt — als erste Bundesligamannschaft, die das dreimal in Folge geschafft hat; sechs Punkte nach Rückstand sind Ligabestwert.** **Thioune war dennoch unzufrieden, Weiser kam zur Pause und strukturierte das Spiel, Pieper war für die Startelf zurück. Werder spielt nicht international.**

**Ein Heimspiel, in dem die Heimmannschaft aus drei Versuchen einen Punkt geholt hat, gegen eine Auswärtsmannschaft, die dreimal in Folge einen Zwei-Tore-Rückstand aufgeholt hat** — ***1:1 ist hier kein Mittelweg, sondern das Ergebnis beider Befunde.***

***Schwelle:*** *Wird in einem Vorbericht die Heimschwäche ausdrücklich als überwunden beschrieben (etwa durch eine Systemumstellung), gehe ich auf **2:1**. Fällt Füllkrug aus (Meldung, nicht Vermutung), gehe ich auf **2:0**. Wird Kohrs Rückkehr belegt, gehe ich auf **2:1**.*

---

### 6. SC Paderborn 07 – Hamburger SV
**Samstag, 24.10.2026, 15:30 Uhr, Home Deluxe Arena**
**Tipp: 1:1**
***unverändert***

***Regel 4 ausdrücklich angewandt.*** **Paderborn steht mit 5 Punkten auf Platz 16, hat aber bei Werder 2:0 geführt (Marino 18., Tigges 30.) und stand in der Nachspielzeit durch Philippe am Pfosten vor dem Auswärtssieg; Torwart Noll hielt mehrfach stark.** **Kettemann beschreibt seine Mannschaft als „Gruppe junger, unerfahrener Bundesliga-Menschen", der es an Torgefahr fehlt** — **5 Tore in 6 Spielen bestätigen das**, *aber zwei davon fielen zuletzt auswärts in Bremen.* **Es fehlen Gayret, Klaas und Baur; bei Awortwie-Grant zeichnet sich ein Comeback ab. Bilbija ist zu Derby County gewechselt.**

**Der HSV kommt mit drei Siegen in Folge, zuletzt 1:0 gegen Stuttgart durch Muheims Schuss aus 25 Metern in der 88. Minute.** ***Die Zahlen hinter der Serie bleiben dünn: 6 Tore in 6 Spielen, 15 Gegentore, Torverhältnis −9 bei 9 Punkten.*** ***Neu und für diesen Tipp stützend:*** **neben Remberg (Kreuzbandriss), Daka und Grönbaek fehlt auch Albert Sambi Lokonga** — **im Spielbericht zum Stuttgart-Spiel heißt es, ohne Remberg und Sambi Lokonga habe dem HSV im Zentrum die Kontrolle gefehlt.** *Der HSV hat trotzdem gewonnen, aber er hat es spät und mit einem Distanzschuss getan.* **Keine der beiden Mannschaften spielt international.**

**Eine Heimmannschaft, die gerade gezeigt hat, dass sie führen kann, gegen eine Auswärtsmannschaft, die mit 6 Saisontoren drei Spiele hintereinander gewonnen hat und im Zentrum zwei Ausfälle hat** — **1:1.**

***Schwelle:*** *Wird eine HSV-Offensivverstärkung belegt (Daka oder Grönbaek im Kaderaufgebot), gehe ich auf **1:2**. Fällt bei Paderborn Tigges **oder** Marino aus, ebenfalls **1:2**. Wird Awortwie-Grants Rückkehr belegt, gehe ich auf **2:1**.*

---

### 7. Borussia Dortmund – Eintracht Frankfurt
**Samstag, 24.10.2026, 18:30 Uhr, Signal Iduna Park**
**Tipp: 2:0**
***unverändert — trotz der Karetsas-Korrektur***

***Hier landet die zweite Hälfte der Korrektur: Karetsas ist Dortmunder, nicht Unioner, und er fällt aus.*** **Er kam gegen Union in der 62. Minute, knickte fünf Minuten später um, war laut `sport.de` auf Krücken unterwegs, und ein wochenlanger Ausfall gilt als möglich; Ricken sagte, die Schwere müsse untersucht werden.** ***Warum ich den Tipp trotzdem nicht ändere:*** **meine Schwelle verlangt einen Innenverteidiger-Ausfall mit genannter Ersatzlösung oder Guirassys Ausfall — Karetsas ist weder das eine noch das andere, und er kam als Einwechselspieler, war also nicht gesetzt.** *Ihn jetzt zum Anlass einer Tippänderung zu machen, wäre genau die Überreaktion, die mir Regel 2 verbietet.* **Ich halte aber fest, dass Dortmunds Offensive damit eine Option weniger hat als gestern angenommen.**

**Dortmund ist drei Pflichtspiele ohne eigenes Tor** (Werder, Bodø, Union), **steht aber mit 14 Punkten und 4 Gegentoren an der Spitze.** **Guirassy ist selbst drei Spiele ohne Treffer und stand in Bodø nicht in der Startelf; Kovač hat eigene Rotationsfehler eingeräumt, sein Vertrag läuft bis 2029** — *eine Entlassung vor dem Spieltag ist damit unwahrscheinlich.* **Nwaneri ist nach der zurückgenommenen Roten Karte spielberechtigt, Schlotterbeck hat gegen Union gespielt.** **Belastung: Dienstag 18:45 in Baku, die weiteste Reise des Spieltags — aber mit vier Tagen Abstand und einem Gegner, gegen den rotiert werden kann.**

**Frankfurt ist der Gegner, gegen den eine Torflaute am ehesten endet: 16 Gegentore in 6 Spielen sind die zweitschwächste Abwehr der Liga.** **Der 1:0-Sieg gegen Köln war Frankfurts erster Heimsieg seit März — auswärts steht die Mannschaft weiter ohne Ausweis.**

***Die eigentliche Schwelle liegt am Dienstag:*** **bleibt Dortmund auch in Baku ohne Tor, sind es vier Spiele, und dann gehe ich auf 1:0.** *Ein 0:0 wäre die Fortsetzung der Flaute und ist das Ergebnis, das mich hier am ehesten widerlegt.*

***Schwelle:*** *Bleibt Dortmund in Aserbaidschan ohne Tor, gehe ich auf **1:0**. Wird ein Dortmunder Innenverteidiger-Ausfall mit genannter Ersatzlösung gemeldet **oder** fällt Guirassy aus, gehe ich auf **1:1**. Wird Kovač entlassen, ebenfalls **1:1**. Wird bei Frankfurt ein weiterer Innenverteidiger-Ausfall gemeldet, gehe ich auf **3:0**.*

---

### 8. TSG Hoffenheim – Bayer 04 Leverkusen
**Sonntag, 25.10.2026, 15:30 Uhr (MEZ), SNP Arena**
**Tipp: 2:2**
***Änderung gegenüber gestern: 1:2 → 2:2, weil heute beide Schwellen dieses Tipps gleichzeitig ausgelöst haben — Hoffenheim hat in Gladbach 2:1 gewonnen, und die Europapokal-Ansetzungen sind aufgelöst: Leverkusen muss Donnerstag nach Kreta, Hoffenheim spielt zu Hause gegen Lyon.***

***Das ist die einzige Änderung dieses Laufs, und sie steht auf zwei unabhängigen Auslösern.***

**Erstens der Sieg.** **Meine Schwelle vom 17.10. lautete wörtlich: „Holt Hoffenheim am Sonntag gegen Gladbach einen Sieg, gehe ich auf 2:2 — ein erster Dreier gegen den Letzten wäre bei sechs Niederlagen aus acht Spielen der erste belastbare Formumschwung."** **Hoffenheim hat 2:1 gewonnen** (Conté 11., Prass 54. nach langem Ball von Hložek) **und ist von Platz 17 auf Platz 14 geklettert.** *Die TSG hat dabei auswärts zweimal getroffen — mehr als in den meisten Spielen davor.*

**Zweitens die Belastung, und hier ist der Befund schärfer, als ich ihn gestern erwarten konnte.** **Meine zweite Schwelle lautete: „Wird Leverkusens Europapokalgegner als weite Auswärtsreise bekannt (außerhalb Mitteleuropas) und Hoffenheims als Heimspiel, gehe ich auf 1:1."** ***Genau das ist eingetreten:*** **Leverkusen spielt Donnerstag 18:45 bei OFI Kreta — etwa 2.300 Kilometer einfach, die weiteste Europapokalreise aller Bundesligisten dieser Woche nach Dortmunds Baku-Fahrt — und muss dann Sonntag um 15:30 schon wieder auswärts antreten.** **Hoffenheim empfängt Lyon zu Hause in der SNP Arena.** ***Aus „die Belastung hebt sich exakt auf" ist damit ein klarer Nachteil für Leverkusen geworden.*** **Nach Regel 3 ist das ein voller Abschlag.**

***Beide Schwellen zeigen in dieselbe Richtung (Remis), nennen aber verschiedene Ergebnisse — 2:2 und 1:1. Ich löse das zugunsten von 2:2 auf, und zwar aus zwei Gründen:*** **Hoffenheim hat gerade belegt, dass es zwei Tore erzielen kann, und Schick hat in allen sechs Saisonspielen getroffen — eine Null für Leverkusen zu tippen, wäre gegen die beste Einzelform des Spieltags.** *Dazu kommt, dass Bernardo in der Hoffenheimer Startelf gegen Gladbach fehlte und seine Sperre damit sehr wahrscheinlich abgesessen hat — ein Indizienschluss, kein Beleg, aber er spricht für Hoffenheim.*

**Dagegen steht der Qualitätsunterschied, den ich nicht kleinrede: Leverkusen ist Vierter mit 13 Punkten, hat heute Freiburg geschlagen und mit Schick und Maza die beiden Torschützen in Form.** **Die Ausfallliste bleibt lang (Terrier mit Oberschenkelverletzung, dazu Ben Seghir, Doué, Eichhorn, Kofane), Hajdari fehlt bei Hoffenheim.** ***Ohne die Kreta-Reise hätte ich bei einem Leverkusener Sieg belassen — mit ihr und dem Hoffenheimer Sieg nicht mehr.***

***Schwelle:*** *Wird Schicks Ausfall oder Schonung belegt, gehe ich auf **1:1**. Kündigt Leverkusen nach Kreta belegt eine Rotation an, gehe ich auf **2:1** (für Hoffenheim). Verliert Hoffenheim am Donnerstag gegen Lyon hoch (drei Tore oder mehr), gehe ich zurück auf **1:2**. Wird Bernardos Sperre als länger als ein Spiel belegt, gehe ich auf **1:2**.*

---

### 9. SC Freiburg – FC Bayern München
**Sonntag, 25.10.2026, 17:30 Uhr (MEZ), Europa-Park Stadion**
**Tipp: 1:2**
***unverändert***

***Die entscheidende Unbekannte dieses Tipps hat sich heute aufgelöst, und zwar genau in dem schmalen Bereich, der nichts ändert.*** **Meine Schwelle vom 17.10. lautete: „Verliert Freiburg am Sonntag gegen Leverkusen deutlich (zwei Tore oder mehr), gehe ich auf 1:3. Gewinnt Freiburg und ist damit Tabellenführer, gehe ich auf 2:2."** **Freiburg hat 1:2 verloren — mit einem Tor Unterschied, nach eigener Führung durch Scherhant (14.).** ***Weder „deutlich" noch ein Sieg: keine der beiden Schwellen greift, der Tipp bleibt.*** **Freiburg ist Dritter mit 13 Punkten und 15:6 Toren, die Serie ist beendet, aber die Mannschaft hat in Leverkusen geführt und bis zur 76. Minute gestanden.**

**Auch die zweite Lücke ist geschlossen: Freiburg spielt Donnerstag 21:00 im Stade Louis-II bei der AS Monaco.** ***Das ist eine mittlere Reise (rund 550 Kilometer), kein Kreta und kein Baku*** — **ich gebe darauf keinen vollen Abschlag nach Regel 3, wohl aber den Hinweis, dass Freiburg am Sonntag drei Tage nach einem Auswärtsspiel antritt und Bayern vier Tage nach einem Heimspiel.** **Suzukis Gelb-Rot-Sperre ist heute gegen Leverkusen abgesessen, er ist wieder spielberechtigt. Muslija fehlt mit Kreuzbandriss.**

**Bayern hat Leipzig 6:1 geschlagen, steht bei 22:5 Toren und ist in sechs Spielen unbesiegt.** ***Bei den Personalien ist die Lage heute klarer, bleibt aber ohne Tippwirkung:*** **Neuers Ausfall hat erstmals eine Diagnose — „etwas Flüssigkeit im Fuß" nach Eberl —, ein Rückkehrdatum gibt es nicht; fällt er weiter aus, hütet Urbig das Tor, was Bayern sechs Spiele lang nicht geschadet hat.** **Musiala fehlt gegen Arsenal; Eberl erwartet eine Rückkehr noch im Oktober — das ist eine Prognose und nach meiner eigenen Regel kein Beleg, also löst es die 1:3-Schwelle nicht aus.** ***Ein kleiner Punkt für Bayern, der heute neu ist:*** **Olise ist für das Arsenal-Spiel gesperrt (zwei Gelbe gegen Viking FK) und geht damit ausgeruht in den Sonntag.**

**Ich bleibe bei Bayern mit einem Tor Unterschied: der Offensivunterschied ist in Zahlen eindeutig (22:5 gegen 15:6), Freiburgs Heimstärke und die drei Tage nach Monaco sprechen gegen eine klare Angelegenheit.**

***Schwelle:*** *Wird Musialas Rückkehr belegt gemeldet (Kaderaufgebot, nicht Prognose), gehe ich auf **1:3**. Wird Kompanys Rotation nach dem Arsenal-Spiel belegt angekündigt, gehe ich auf **1:1**. Verliert Freiburg am Donnerstag in Monaco hoch und wird eine Freiburger Rotation gemeldet, gehe ich auf **0:2**. **Neuers Rückkehr ändert nichts.***

---

## Verteilung und Selbstkontrolle

| Tipp-Typ | Anzahl | Partien |
|---|---|---|
| **Heimsieg** | **5** | 1 (2:0), 2 (2:1), 3 (1:0), 4 (2:1), 7 (2:0) |
| **Remis** | **3** | 5 (1:1), 6 (1:1), 8 (2:2) |
| **Auswärtssieg** | **1** | 9 (1:2) |

**Gesamttore: 23 in 9 Partien, 2,56 je Spiel** — *etwas unter dem Bundesligaschnitt, was zu einem Spieltag mit vier Europapokal-Nachwirkungen passt.*

***Drei Dinge, die ich an meiner eigenen Tippreihe kritisch sehe:***
1. **Fünf Heimsiege sind viel** — *nach einer Abrechnung, in der ich dreimal die schwächere Heimmannschaft überschätzt habe (Elversberg ausgenommen, dort lag ich andersherum falsch), ist das ein Muster, auf das ich beim nächsten Lauf achten muss.*
2. **Partie 4 bleibt der Tipp, bei dem Regel 4 und meine Entscheidung auseinanderlaufen.** *Ich tippe Leipzig trotz der Lehre, dass ich Aufsteiger unterschätze. **Wenn dieser Tipp falsch wird, ist es kein Pech, sondern ein wiederholter Denkfehler** — und dann ziehe ich beim nächsten Mal die Konsequenz.*
3. **Partie 2 steht nach der Karetsas-Korrektur auf der dünnsten Personalgrundlage des ganzen Spieltags** — *zu Union habe ich keinen einzigen datierten Ausfall.*

---

## Quellen

**Alle Angaben dieses Laufs stammen aus `WebSearch`-Ergebnislisten (Titel und Zusammenfassungen), nicht aus Volltexten** — *die vier im Routine-Prompt genannten Leitquellen sind durch die Egress-Policy gesperrt, `WebFetch` scheitert an der Namensauflösung.*

**Für die Ergebnisse und Berichte des 6. Spieltags:** `bundesliga.com`, `sportschau.de`, `zdfheute.de`, `sport.de`, `t-online.de`, `hasepost.de`, `berliner-sonntagsblatt.de`, `fussballnationalmannschaft.net`, `reviersport.de`, `mainz05.de`, `ms-aktuell.de`, `absolutfussball.com`, `fuldainfo.de`.
**Für Personalien und Korrekturen:** `bvb.de` (Karetsas), `ligainsider.de` (nur teilweise, siehe „geprüft und verworfen"), `ran.joyn.de`, `sport.sky.de`, `ruhrnachrichten.de`, `magazin.comunio.de`, `frankenpost.de`, `bavarianfootballworks.com`, `sports.yahoo.com`.
**Für die Europapokal-Ansetzungen:** `de.uefa.com`, `asmonaco.com` (Ticketseite), `tsg-hoffenheim.de` (Ticketcenter), `ran.joyn.de`, `sport.sky.de`, `cbssports.com`, ein `kicker.de`-Artikeltitel aus der Ergebnisliste.
**Für die Ansetzungen des 7. Spieltags:** `anstosszeiten.de` (heute korrigiert), `profis.eintracht.de`, DFL-Spielplan-PDF, `sportschau.de`.

***Nicht erreichbar und deshalb nicht verwendet:*** **`kicker.de`, `bundesliga.com`, `transfermarkt.de` und `weltfussball.de` im Volltext** *(403 der Egress-Policy; Inhalte dieser Seiten erscheinen hier nur, soweit sie in Suchergebnis-Zusammenfassungen auftauchen).*
