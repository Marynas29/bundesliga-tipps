# Bundesliga-Tipps – 6. Spieltag 2026/27 (Stand: 13.10.2026)

**Ansetzung:** Freitag, 16.10. bis Sonntag, 18.10.2026.
**Vortagsstand:** 12.10.2026, **ebenfalls 6. Spieltag** — echter Vergleich für alle neun Partien möglich.

**Ergebnis dieses Laufs in einem Satz:** **Kein Tipp geändert, alle neun unverändert** — und das ist diesmal ein Befund, nicht Untätigkeit: **drei der vier Schwellen, die ich gestern für heute formuliert habe, sind heute ausgelöst worden, und alle drei in den Zweig „bleibt".** **Dazu kommen die beiden ersten echten Pflichtspielergebnisse der Woche** (Bayern 3:3 in Stavanger, Leipzig 1:0 gegen PSV) **und die ersten offiziellen Vereinsquellen des Spieltags** (BVB-Reisekader, HSV-Personalupdate). **Die Ursache des Abrufproblems ist nach drei Tagen erstmals host-genau geklärt — und sie liegt nicht an den Quellen, sondern an der Netzwerkeinstellung dieser Umgebung** (siehe nächster Abschnitt, mit der Stelle, an der der Nutzer sie ändern kann).

---

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Heute ist die Diagnose gelungen, die an den drei Vortagen gescheitert ist.**

- **Die Proxy-Diagnose war heute erstmals abrufbar.** `curl -sS "$HTTPS_PROXY/__agentproxy/status"` lief durch (gestern hatte der Auto-Mode-Klassifikator der Sitzung den Aufruf abgelehnt). Der Proxy meldet sich als funktionsfähig: `enabled: true`, `bundleCoversEveryHost: true`, **und zum Zeitpunkt der Abfrage keine einzige vorangegangene Fehlleitung** (`recentRelayFailures: []`).
- ***Damit ist belegt, was bisher nur Symptom war:*** **Die Fußballquellen sind durch die Egress-Policy dieser Umgebung gesperrt.** Ich habe `www.bundesliga.com`, `www.weltfussball.de` und `www.kicker.de` per `curl` angesprochen. **Alle drei scheiterten mit `CONNECT tunnel failed, response 403`**, und der Proxy hat genau diese drei Hosts anschließend protokolliert: `kind: "connect_rejected"`, `detail: "gateway answered 403 to CONNECT (policy denial or upstream failure)"`, mit Zeitstempel 21:15:43 UTC. ***Das ist eine Richtlinienablehnung, kein Defekt und kein Quellenproblem.*** *Die Anleitung in `/root/.ccr/README.md` sagt für 403/407 ausdrücklich: nicht umgehen, sondern den gesperrten Host melden. Genau das tue ich.*
- ***Was der Nutzer tun kann, wenn er Volltexte will:*** **Die Netzwerkfreigabe der Umgebung steuert das.** *Im Menü der Cloud-Umgebung in der Titelzeile der Sitzung → „Edit" → **Network access**: entweder eine breitere Zugriffsstufe wählen oder `kicker.de`, `bundesliga.com`, `weltfussball.de` und `transfermarkt.de` unter **Allowed domains** eintragen (das Häkchen „Allow package managers" dabei gesetzt lassen). Dokumentiert unter https://code.claude.com/docs/en/cloud-environments#network-access.* **Solange das so bleibt, kann ich die vier im Routine-Prompt genannten Leitquellen grundsätzlich nicht im Volltext lesen** — nicht an einem einzelnen Tag, sondern dauerhaft.
- **`WebFetch` scheitert zusätzlich eine Stufe früher.** Der Testabruf von `www.bundesliga.com` endete erneut mit `getaddrinfo ENOTFOUND`. *Da der Proxy für diesen Versuch keinen Eintrag führt, erreicht `WebFetch` den Proxy gar nicht; es löst den Namen selbst nicht auf. **Beide Befunde zusammen heißen: Volltext ist in dieser Umgebung auf keinem der beiden Wege zu bekommen.***
- **`WebSearch` funktioniert und war heute produktiv.** **Alles Folgende steht auf Suchergebnis-Zusammenfassungen und -Titeln, kein Volltext.**
- ***Qualitativer Fortschritt gegenüber gestern:*** **Heute stammt der Kern der Personalinformationen erstmals aus offiziellen Vereinsmeldungen und journalistischen Quellen** — `bvb.de`, `hsv.de`, `sportschau.de`/WDR, `stuttgarter-nachrichten.de`, `vfb.de`, `ligainsider.de` vom 13.10. *Das Wett-Portal `wetttippsheute.net`, auf dem gestern ein erheblicher Teil ruhte, brauche ich heute nur noch ergänzend. Wo ich es verwende, steht es dabei; fremde Ergebnisprognosen übernehme ich nicht.*
- **Die Tabelle unten ist weiterhin selbst gerechnet**, weil keine Tabellenseite abrufbar ist. *Sie hat heute eine zweite Fremdbestätigung bekommen (siehe dort).*

---

## Die Nachrichtenlage

**Zwei Bundesligisten haben heute Abend schon gespielt, und die Ergebnisse fallen gegensätzlich aus.** **Bayern kam bei Viking Stavanger nur zu einem 3:3**, lag zur Pause 0:2 hinten, führte durch zwei Tore von Harry Kane (54. Elfmeter, 60.) und Luis Díaz (71.) mit 3:2 und kassierte in der 90. Minute durch Herman Haugen den Ausgleich; **Michael Olise sah in der 73. Minute Gelb-Rot**, nachdem er Vikings Kapitän Tripić den Ball ins Gesicht geworfen hatte. **Leipzig gewann zur gleichen Zeit zu Hause 1:0 gegen PSV Eindhoven** — Brajan Gruda per Fernschuss in der 75., dazu ein gehaltener Elfmeter von Maarten Vandevoordt gegen Ivan Perišić in der 19. **Es war Leipzigs erster Sieg der Ligaphase nach dem 1:4 in Como.** *Beide Mannschaften treffen am Samstag um 18:30 in München aufeinander — die Belastung dieses Spiels ist damit nicht mehr Prognose, sondern Tatsache.*

**Der zweite große Block sind die ersten offiziellen Vereinsmeldungen zum Spieltag, und zwei davon sind tippnah.** **Dortmund reist mit 23 Spielern nach Bodø, aber ohne Nico Schlotterbeck** — **der Verein hat am Dienstag ausdrücklich mitgeteilt, dass der Abwehrchef „aus reiner Vorsicht" geschont wird und keine akute Verletzung vorliegt.** **Julian Ryerson ist nach seiner Verletzung aus der Länderspielpause zurück im Kader**, dazu nominierte Niko Kovač neben Mane drei weitere Nachwuchsspieler (Kaua Prates, Samuele Inacio, Mathis Albert). **Der BVB fliegt nach dem Spiel zurück nach Dortmund und reist bereits am Freitag nach Berlin.** **Beim HSV standen Bilal Nadir (Adduktoren) und Zakaria El Ouahdi (Erkältung) am Dienstag wieder auf dem Platz**, Bakery Jatta fehlte angeschlagen, Albert Grønbæk und Patson Daka arbeiten weiter individuell; **Kapitän Nicolai Remberg muss nach dem Kreuzbandriss operiert werden und fehlt Monate.**

**Drittens ist eine Diagnose aus dem Derby jetzt konkret.** **Ellyes Skhiri hat laut MRT einen Syndesmoseriss und fällt rund drei Monate aus** — gestern stand nur „Verletzung am Sprunggelenk" und ein vermuteter Bänderriss. **Entscheidend für den Tipp ist aber der zweite Teil der Meldung: Köln hat die Ersatzlösung benannt.** **Tom Krauß hat Skhiris Rolle schon im Derby übernommen, Marius Bülter ersetzt die verletzten Thijs Dallinga und Ragnar Ache in der Offensive, und Sportdirektor Thomas Kessler schließt eine Nachverpflichtung aus.**

**An der Spitze und am Ende ist die Lage die von gestern:** Freiburg führt mit 13 Punkten, Dortmund punktgleich, Bayern Dritter; **Gladbach ist punktlos Letzter**, Hoffenheim mit drei Punkten Siebzehnter. **Ein DFB-Pokalspiel liegt in dieser Woche nicht an, eine Länderspielpause läuft nicht** (sie lag vor dem 5. Spieltag).

### Die Europapokalwoche — Stand Dienstagnacht

| Tag | Partie | Wettbewerb | Lage für den Bundesligisten | Ergebnis |
|---|---|---|---|---|
| **Di 13.10., 21:00** | Viking Stavanger – **FC Bayern** | Champions League | auswärts (Norwegen) | **3:3** — Kane (54. E, 60.), Díaz (71.); Gelb-Rot Olise (73.) |
| **Di 13.10., 21:00** | **RB Leipzig** – PSV Eindhoven | Champions League | heim | **1:0** — Gruda (75.), Elfmeter gehalten (19.) |
| **Mi 14.10., 21:00** | Bodø/Glimt – **Bor. Dortmund** | Champions League | auswärts (Nordnorwegen) | *offen* |
| **Mi 14.10., 21:00** | Slovan Bratislava – **VfB Stuttgart** | Champions League | auswärts | *offen* |
| **Do 15.10., 18:45** | Lech Posen – **Bayer Leverkusen** | Europa League | auswärts (Polen) | *offen* |
| **Do 15.10., 21:00** | **TSG Hoffenheim** – Beşiktaş Istanbul | Europa League | heim | *offen* |
| **Do 15.10., 21:00** | **SC Freiburg** – FK Jablonec | Conference League | heim | *offen* |

**Zwei Einordnungen zu den Mittwochs- und Donnerstagsspielen:** **Stuttgart ist am Dienstagnachmittag von Echterdingen aus nach Bratislava geflogen**, die Pressekonferenz mit Sebastian Hoeneß und Leo Sauer war für 18 Uhr angesetzt. **Hoffenheim trifft am Donnerstag auf einen Gegner in Form: Beşiktaş hat zum Auftakt zu Hause 4:1 gegen Olympique Marseille gewonnen, während die TSG 0:2 bei OFI Kreta verlor.** *Das verschärft das Belastungsargument, auf dem mein 1:1 in Gladbach ruht.*

### Pressekonferenz-Termine — heute erstmals bekannt

**`ligainsider.de` führt die PK-Termine zum 6. Spieltag:** **Frankfurt und Köln am Mittwoch, 14.10.** · **Gladbach am Freitag, 16.10.** · **Bayern, Leverkusen, Stuttgart, Dortmund und Leipzig sind noch nicht angesetzt.** ***Das heißt: zu diesem Spieltag hat bis heute Abend keine einzige Pressekonferenz stattgefunden*** — die Lücke, die der Routine-Prompt mit „Aussagen aus Pressekonferenzen" anspricht, besteht zum vierten Tag in Folge, **aber sie schließt sich morgen zum ersten Mal.** *Die Dortmunder PK in Bodø (Kovač und Ryerson, ab 17 Uhr bei BVB-TV) und die Stuttgarter in Bratislava sind Europapokal-PKs, keine Spieltags-PKs; zu beiden lag bei Abschluss dieses Laufs noch kein Bericht vor.*

---

## Korrekturen am Vortagsstand

**Fünf Punkte. Drei sind eigene Unvollständigkeiten, zwei sind Präzisierungen fremder Angaben.**

1. ***Meine Elversberger Ausfallliste war falsch — und zwar in der Aussage, sie sei kurz.*** **Gestern schrieb ich: „Elversberg hat nur einen gesicherten Ausfall: Luis Seifert."** **Richtig ist, dass beim 0:1 in Berlin außerdem Jan Gyamerah (Muskelverletzung) und Francis Onyeka gefehlt haben.** *Gyamerah hat die Reha abgeschlossen und ist für Samstag wieder einsatzbereit, ob er sofort startet, ist offen — Luca Sirch hat ihn rechts hinten vertreten und wurde von Trainer Vincent Wagner für Berlin gelobt. Zu Onyeka bleibt offen, wann er zurückkehrt.* **Der Fehler lag nicht in einer falschen Zahl, sondern in einem zu selbstsicheren „nur".**
2. ***Kölns Trainerlage ist besser belegt als gestern — und meine Einschränkung von gestern war berechtigt, aber zu pessimistisch.*** **Gestern: „Wagners Status ist nur über einen Tipp-Blog belegt."** **Heute: René Wagner hat Köln als Interimstrainer nach der Entlassung von Lukas Kwasniok übernommen; sein Debüt war das 2:2 in Frankfurt im April 2026, bei dem ein Joker-Trio Köln den Punkt rettete.** *Das ist mehr als ein Blog, aber weiterhin keine Vereinsmeldung zur Vertragslage. Ich führe ihn als Trainer und die Vertragsfrage weiter als offen.*
3. ***Zu Bernardo (Hoffenheim) widersprechen sich die Quellen, und das habe ich gestern nicht gesehen.*** **Gestern führte ich nur die Gelb-Rot-Sperre aus dem HSV-Spiel.** **Heute nennt eine Quelle die Sperre bis 25.10. (nur Bundesliga, nicht Europa League), eine andere eine Achillessehnenverletzung mit Rückkehr nach dem Spieltag.** *Für meinen Tipp ist der Widerspruch ohne Folge — nach beiden Lesarten fehlt er in Gladbach. **Was wegfällt, ist meine gestrige Nebenangabe „als Ersatz wird Mats Rots erwartet"**: dafür habe ich heute keine Fundstelle mehr, und ich verwende sie nicht weiter.*
4. ***Zwei Ausfälle, die gestern in meinen Listen fehlten.*** **Bei Hoffenheim: Albian Hajdari (Knieverletzung, laut Ilzer zurück im leichten Training, Einsatz am Donnerstag offen) und Patrick Wimmer (Oberschenkel, fraglich — der SWR nennt ihn, Sportsgambler nicht).** **Bei Leipzig: Viggo Gebel (Kreuzbandriss).** *Keiner der drei verschiebt einen Tipp, aber sie gehörten gestern in die Listen.*
5. ***Eine Zahl zu Skhiri wird konkret, eine zweite bleibt es nicht.*** **Gestern: „Medien nennen einen Bänderriss, der Verein bestätigt nur eine Verletzung am Sprunggelenk; ein Fanblog hält ein Ausfallende erst 2027 für möglich."** **Heute: Syndesmoseriss nach MRT, circa drei Monate.** *Eine offizielle Prognose des Vereins steht laut Quellenlage weiter aus, und das Fanblog bleibt bei „mindestens bis Jahresende" — das ist mit drei Monaten ab dem 11.10. vereinbar. **Neu und für den Tipp relevanter als die Dauer: Tom Krauß ist als Ersatz benannt** (siehe Partie 1).*

**Unverändert strittig und heute nicht geklärt:** **Freiburgs Torverhältnis** (bundesliga.com `13:3` gegen meine Rechnung `14:4`; beide ergeben +10 und 13 Punkte). **Die Reviersport-Abweichung** bei Bayern und Leverkusen besteht fort. *Auf keinen Tipp hat beides Einfluss.*

---

## Tabelle nach dem 5. Spieltag (vollständig)

**Unverändert gegenüber gestern — in der Bundesliga ist seit dem 5. Spieltag kein Spiel hinzugekommen.** **Aus einzeln belegten Ergebnissen gerechnet.** **Form = 1. bis 5. Spieltag von links nach rechts.**

| # | Verein | Sp | S | U | N | Tore | Diff | Pkt | Form | Europapokal diese Woche |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | SC Freiburg | 5 | 4 | 1 | 0 | 14:4 | +10 | 13 | S S S U S | **Do, CL-Conf., heim** |
| 2 | Borussia Dortmund | 5 | 4 | 1 | 0 | 11:4 | +7 | 13 | S S S S U | **Mi, CL, auswärts** |
| 3 | FC Bayern München | 5 | 3 | 2 | 0 | 16:4 | +12 | 11 | S U S S U | **Di, CL, auswärts — 3:3** |
| 4 | Bayer 04 Leverkusen | 5 | 3 | 1 | 1 | 14:8 | +6 | 10 | N S U S S | **Do, EL, auswärts** |
| 5 | RB Leipzig | 5 | 3 | 0 | 2 | 15:5 | +10 | 9 | S N S N S | **Di, CL, heim — 1:0** |
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

**Die zweite Fremdbestätigung dieser Tabelle ist heute hinzugekommen:** **Ein Vorbericht zu Union – Dortmund führt Union auf Platz 16 und Dortmund auf Platz 2.** *Das deckt sich mit meinen Zeilen. **Derselbe Vorbericht bestätigt außerdem drei Einzelergebnisse, die ich bisher nur gerechnet hatte:** Dortmunds Auswärtssiege in Hoffenheim (3:2) und Stuttgart (1:0) und das 2:2 gegen Bremen nach 2:0-Führung — Letzteres passt zu Füllkrugs Kopfballausgleich in der 90.+2, den ich gestern schon führte.* **Und der WDR bestätigt den Derbyausgang: Köln 2:1 gegen Gladbach, Entscheidung durch El Mala** — *das ist Blessins Debütniederlage und passt zu beiden Tabellenzeilen.*

---

## Trainer — heute ergänzt

**Zwei Namen, die mir bisher fehlten, sind heute belegt:**

**Borussia Dortmund: Niko Kovač** — *der Vorbericht nennt ihn und hält fest, dass er in jedem Pflichtspiel außer dem Pokalauftritt ein 3-4-3 aufgeboten hat; die offizielle BVB-Meldung zur Bodø-Reise nennt ihn als den, der den Kader nominiert hat.* **SV 07 Elversberg: Vincent Wagner** — *mit Zitat zu Gyamerah: „Wir können froh sein, dass es nicht wie bei anderen ist und er Monate ausfällt, sondern vielleicht nur zwei oder drei Wochen."*

**Unverändert aus dem Vortagsstand:** Frankfurt Adi Hütter · Köln René Wagner (Interim, siehe Korrektur 2) · Werder Daniel Thioune · Gladbach Alexander Blessin (Vertrag laut Klub bis 2028, heute bestätigt) · Schalke Miron Muslić · Freiburg Julian Schuster · Mainz Urs Fischer · Hoffenheim Christian Ilzer · Stuttgart Sebastian Hoeneß · Union Lustrinelli.

***Zwei bleiben offen, und ich schreibe sie als offen hin:*** **Augsburgs Trainer habe ich erneut nicht belegt** — die einzige Fundstelle nennt Manuel Baum, ist aber undatiert und mit hoher Wahrscheinlichkeit veraltet; **ich verwende den Namen nicht.** **Leverkusens Trainer ebenso nicht:** in den Treffern erscheint Kasper Hjulmand, aber ausschließlich in Material aus der Saison 2025/26. *Für 2026/27 ist das keine Grundlage, und ich behaupte es nicht.*

---

## Heute geprüft und verworfen

1. **`flashscore.de`, „Bundesliga 6. Spieltag: Verletzungen und Sperren in der Übersicht".** **Verworfen:** *die Seite stammt aus der Saison 2023/24. Der Titel passt exakt auf meine Suche, der Inhalt auf eine andere Saison — derselbe Fallentyp, der mir an den Vortagen bei bundesliga.com und fussballdaten.de begegnet ist.*
2. **Die `ligainsider.de`-Verletztenliste „1. Bundesliga 2026/27".** **Nur eingeschränkt verwendet:** *sie ist mit 2026/27 richtig etikettiert, bezieht sich aber auf den 5. Spieltag; die Schalke- und Mainz-Teamseiten sind nach eigener Angabe 44 bzw. 171 Tage alt. **Ich verwende daraus nur, was eine zweite Quelle stützt** — und nenne Heekeren unten ausdrücklich mit diesem Vorbehalt.*
3. **Sämtliche Treffer zu Leverkusen – Freiburg.** **Verworfen:** *die Suche liefert ausschließlich Material zu früheren Begegnungen (Liveticker 8. Spieltag 2025/26, Freiburg – Leverkusen vom 07.03.2026, ein Schick-Update von Oktober 2025 vor einem Freiburg-Spiel, ein Arsenal-Vorbericht). **Die jüngsten Treffer sind rund 220 Tage alt.*** **Zu dieser Partie habe ich heute keinen aktuellen Vorbericht gefunden** — gestern hatte ich einen (vom Wett-Portal). *Das ist der einzige Punkt, an dem die Quellenlage heute schlechter ist als gestern.*
4. **Ein Vorbericht „Eintracht Frankfurt vs. 1. FC Köln" mit Hütter und Wagner.** **Teilweise verworfen:** *die Mehrheit der Treffer zu dieser Partie beschreibt das Hinspiel vom April 2026 (2:2, Wagners Debüt). **Ich verwende daraus nur die Trainerzuordnung und das Hinspielergebnis, nichts zur aktuellen Form.***
5. **`news.de`, „Sechs Verletzte nach Ausschreitungen beim Rheinderby".** **Nicht verwendet:** *die Meldung betrifft verletzte Personen bei Ausschreitungen, nicht verletzte Spieler. **Das ist eine Falle, in die ich beinahe gelaufen bin**, weil meine Gladbach-Zeile von gestern ebenfalls von „sechs Ausfällen" spricht — die kommen aber aus einer anderen Quelle (`ms-aktuell.de`) und meinen Profis. Die Zahlengleichheit ist Zufall.*
6. **`tipico.de`-Aufstellungsprognose zu Bodø/Glimt – Dortmund.** **Verworfen:** *sie betrifft die Begegnung vom Dezember 2025 (2:2) und führt Emre Can und Justin Lerma als verletzt — Letzteres widerspricht einer Fundstelle, die Lerma später im Monat erwartet. **Der offizielle BVB-Reisekader von heute ist die bessere Quelle, und ich folge ausschließlich ihm.***
7. **Die Mainz-Treffer von `footy.de` zu Zentner vom 15./16.09.2026.** **Nicht verwendet:** *sie nennen ein Schalke-Spiel im unmittelbaren Zusammenhang mit Zentners Ausfall und passen zeitlich nicht zum 6. Spieltag. **Die Zentner-Chronologie ist in den Quellen widersprüchlich** — dazu unten bei Partie 2 ein eigener Absatz.*

---

## Offen benannte Restlücken

**Der Spieltag ist noch drei bis fünf Tage entfernt.**

- **Keine einzige Spieltags-Pressekonferenz hat stattgefunden.** *Die erste ist morgen (Frankfurt und Köln, 14.10.); Gladbach folgt am Freitag; zu Bayern, Leverkusen, Stuttgart, Dortmund und Leipzig ist noch kein Termin angesetzt.*
- **Keine offizielle Startelf und kein Kaderaufgebot zu irgendeiner der neun Bundesligapartien.** *Was heute vorliegt, sind zwei **Europapokal**-Reisekader (Dortmund, Stuttgart) und zwei Trainingsstandsberichte (HSV, Werder).*
- **Zu Leverkusen – Freiburg gibt es heute keinen aktuellen Vorbericht** (verworfene Fundstelle 3). **Zu Bayern – Leipzig habe ich auch heute keinen gefunden** — bei dieser Partie ersetzen die beiden Dienstagsergebnisse den fehlenden Vorbericht teilweise.
- **Zu Paderborn habe ich zum dritten Tag in Folge keine eigene Verletztenliste gefunden** — nur die Werder-Seite der Partie. *Das bleibt die älteste offene Lücke.*
- **Augsburgs und Leverkusens Trainer bleiben unbelegt** (siehe Trainerabschnitt). *Bei Augsburg betrifft das eine Partie, zu der ich auch sonst heute nichts Neues habe.*
- **Kleindiensts Status für Sonntag ist weiter offen** — weder Diagnose noch Ausfalldauer. *Die Datierung der Meldungen ist uneinheitlich: eine Fundstelle spricht von einem Trainingsabbruch „am Dienstag", ohne dass erkennbar ist, ob der 6.10. oder der 13.10. gemeint ist. **Ich leite daraus nichts Neues ab und bleibe beim Stand von gestern.***
- **Mittelstädts Status widerspricht sich** (siehe Partie 6). **Zu El Ouahdi, Nadir und Jatta ist der Kadereinsatz am Samstag laut HSV ausdrücklich noch offen.**
- **Musialas Rückkehr bleibt unklar** — *die Verletzungsart ist heute übereinstimmend als Muskelfaserriss im Oberschenkel aus der Länderspielpause benannt, ein Rückkehrdatum nicht.*
- **Keine Transfermeldung mit Spielrelevanz** — *eine einzige Transferinformation ist heute aufgetaucht und sie ist historisch, nicht aktuell: **Skhiri ist im Sommer 2026 von Eintracht Frankfurt zurück nach Köln gewechselt.** Das ist eine Personalie der Partie 1 und steht dort.*
- **Freiburgs Torverhältnis bleibt strittig** (13:3 gegen 14:4).

---

## Die Tipps zum 6. Spieltag

**Die vier Regeln gelten unverändert weiter** und werden an jeder Partie geprüft:
**(1)** Eine Ausfallmeldung **ohne Angabe zur Ersatzlösung** verschiebt den Tipp nicht. **(2)** Die Tabellenposition der Heimmannschaft begründet keinen Auswärtstipp, solange keine partiebezogene Information dazukommt. **(3)** Kein einziger Zu-null-Tipp an diesem Spieltag. **(4)** Wenige, grob geschnittene Schwellen mit einander ausschließenden Zweigen.

### 1. Eintracht Frankfurt – 1. FC Köln
**Freitag, 16.10.2026, 20:30 Uhr**
**Tipp: 2:1**
***unverändert***

**Begründung:** **Frankfurt kommt vom 0:6 in Leipzig und hat mit 16 Gegentoren nach fünf Spieltagen laut Fundstelle einen Vereinsnegativrekord zu diesem Zeitpunkt aufgestellt.** **Adi Hütter fordert heute öffentlich eine bessere Rückwärtsbewegung und benennt die Defensive als Hauptproblem.** **Der dokumentierte Konflikt mit Kapitän Robin Koch besteht fort** (Hütter: Abwehrleistung „nicht bundesligatauglich", Auswechslung zur Halbzeit, „Ich habe Robin erlöst"; Koch im kicker: Weglaufen sei keine Option). **Köln hat in jedem der fünf Ligaspiele mindestens ein Tor erzielt** — darauf steht das eine Gästetor.

***Die neue Information läuft heute gegen die Kölner Abwertung von gestern, und ich korrigiere die Begründung entsprechend:*** **Skhiris Diagnose ist härter geworden (Syndesmoseriss, rund drei Monate), aber Köln hat die Ersatzlösungen benannt: Tom Krauß hat Skhiris Part schon im Derby übernommen, Marius Bülter ersetzt Dallinga (Kreuzbandriss, zugezogen im Testspiel gegen Viktoria Köln) und Ache (Muskelproblem) in der Offensive, und Sportdirektor Thomas Kessler schließt eine Nachverpflichtung ausdrücklich aus.** ***Das ist genau die Konstellation, für die Regel 1 gemacht ist — nur in der seltenen Richtung:*** *gestern habe ich geschrieben, Kölns Lage sei „personell schlechter als die Tabelle sagt". **Mit drei benannten Ersatzlösungen trägt dieser Satz nicht mehr.** Der Tipp bleibt 2:1, aber er ruht jetzt auf dem Heimrecht, der Reaktion nach dem 0:6 und Frankfurts Abwehr — **nicht mehr auf Kölns Personalnot.***

**Eine Personalie mit Doppelbezug:** **Skhiri ist im Sommer 2026 von Eintracht Frankfurt zurück nach Köln gewechselt** — *der prominenteste Ausfall dieser Partie fehlt also gegen seinen Vorsaisonverein.*

**Warum kein hohes Frankfurter Ergebnis:** *Ein Heimsieg nach einer solchen Niederlage ist plausibel, ein Zu-null bei der zweitschlechtesten Abwehr der Liga nicht — und Regel 3 verbietet es ohnehin.* **Keine der beiden Mannschaften spielt international.**

**Schwelle 1 geprüft:** *Erster Zweig (Frankfurter Startelf oder Kaderaufgebot **ohne Koch** → 1:1): **nicht ausgelöst**, es gibt kein Aufgebot. Zweiter Zweig (weiterer Kölner Ausfall im Mittelfeld oder in der Offensive **mit genannter Ersatzlösung** → 3:1): **nicht ausgelöst** — heute sind **Ersatzlösungen zu den bereits bekannten Ausfällen** benannt worden, kein neuer Ausfall. **Die Unterscheidung ist mir heute wichtig, weil sie knapp ist: die Schwelle verlangt einen neuen Ausfall, und den gibt es nicht.*** **Die PK beider Vereine ist morgen** — das ist die erste Gelegenheit, an der der erste Zweig überhaupt auslösen kann.

### 2. FC Schalke 04 – 1. FSV Mainz 05
**Samstag, 17.10.2026, 15:30 Uhr** (Veltins-Arena)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Der Offensivunterschied bleibt der größte belegte Einzelwert dieser Partie: Mainz 13 Tore in fünf Spielen, Schalke 5 — die schwächste Offensive der Liga.** **Mainz' Gegenwert ist eine Abwehr, die der eigene Trainer kritisiert** (Urs Fischer nach dem 3:4 gegen Leverkusen: „Du darfst keine vier Tore zu Hause bekommen"). **Die Anstoßzeit ist für diese Partie als einzige des Samstags offiziell bestätigt.**

***Hier ist heute die wichtigste Schwellenentscheidung des Spieltags gefallen, und sie fällt für den Tipp:*** **`ligainsider.de` meldet am 13.10. unter dem Titel „Zentner weiter eingeschränkt – Schalke wohl zu früh": Robin Zentner hat wieder trainiert, konnte aber noch nicht mit den Torwarttrainern arbeiten; seine Einsatzchancen am Samstag gelten als schlecht.** **Und der Ersatz ist namentlich benannt: Alexander Schwolow.** ***Entscheidend ist, wer das ist:*** **Schwolow hat Zentner in dieser Saison schon am 2. Spieltag vertreten — beim 5:0 gegen den HSV, ohne Gegentor.** *Dazu kommt eine Nebengeschichte: Schwolow stand 2022/23 selbst bei Schalke unter Vertrag und würde gegen seinen Ex-Klub spielen.*

**Schwelle 2 geprüft — der Zweig greift, und zwar der Zweig „bleibt":** *Sie lautete: „Wird **Zentners Ersatz namentlich benannt** und ist es **nicht der etatmäßige zweite Torwart**, gehe ich auf 1:1." **Der Ersatz ist benannt, aber er ist genau der etatmäßige zweite Torwart — mit einem zu null in dieser Saison.*** **Die Bedingung für 1:1 ist damit belegt nicht erfüllt, und der Tipp bleibt 1:2 — heute aus einem positiven Grund, nicht mehr nur aus Zurückhaltung.** *Gestern war das mein engster Tipp; heute ist er der am besten aufgelöste.*

***Eine Chronologie, die ich nicht glattbügele:*** **Die Quellen zu Zentner widersprechen sich im Ablauf.** **Eine nennt als Ursache die Handverletzung im 1:3-Heimspiel gegen Eintracht Frankfurt, eine andere, Schwolow habe schon am 2. Spieltag vertreten** — *das kann nicht beides dieselbe Verletzung sein, und eine Fundstelle titelt passend „Zentner hat es schon wieder erwischt". **Die plausibelste Lesart ist zwei Verletzungen; belegen kann ich sie nicht.** Für den Tipp ist nur der heutige Stand nötig, und der ist eindeutig: Zentner fehlt voraussichtlich, Schwolow steht bereit.*

**Schalkes Lage:** **Højlund (Achillessehne) und Siebeking (Bauchmuskel) fehlen.** ***Mit Vorbehalt:*** **dieselbe Liste führt Torwart Justin Heekeren mit Kreuzbandriss und „mindestens sechs Monate"** — *die Seite ist nach eigener Angabe 44 Tage alt, der Ausfall also kein neuer Befund, sondern ein länger bestehender. **Ich führe ihn als Kontext, nicht als Neuigkeit**, und leite daraus nichts ab: wenn Schalkes Nummer eins seit Wochen fehlt, ist der jetzige Torwart eingespielt.* **Zu Ljubičić (Knie, „bis auf Weiteres") habe ich heute keine Bestätigung gefunden; ich führe ihn aus dem Vortagsstand weiter.** **Zu Gantenbein, dessen Debüttreffer gestern mein Hauptargument für Schalke war, gibt es heute keine Meldung.** **Keine der beiden Mannschaften spielt international.**

### 3. SV 07 Elversberg – FC Augsburg
**Samstag, 17.10.2026, 15:30 Uhr** (Ursapharm-Arena)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Augsburg hat laut bundesliga.com an allen fünf Spieltagen mindestens zwei Tore erzielt** und **dem Dritten Bayern einen Punkt abgenommen** (Fellhauer nach 8,4 Sekunden, Ribeiro 64.). **Elversberg kommt von der 0:1-Niederlage in Berlin und hat 8 Tore in fünf Spielen.**

***Die neue Information spricht gegen meinen Tipp, und sie korrigiert zugleich einen Fehler von gestern:*** **Jan Gyamerah hat die Reha nach seiner Muskelverletzung abgeschlossen und ist für Samstag wieder einsatzbereit** — *er hatte beim 0:1 in Berlin gefehlt, was ich gestern nicht wusste (Korrektur 1). Trainer Vincent Wagner: „Wir können froh sein, dass es nicht wie bei anderen ist und er Monate ausfällt, sondern vielleicht nur zwei oder drei Wochen." **Ob er sofort startet, ist offen**; Luca Sirch hat ihn rechts hinten vertreten und wurde für Berlin gelobt.* **Elversberg ist damit personell besser dran als gestern angenommen — aber auch schlechter, als ich gestern geschrieben habe: Francis Onyeka fehlte in Berlin ebenfalls und seine Rückkehr ist offen, dazu Luis Seifert (Fußverletzung, länger) und Tom Zimmerschied (Rücken, einige Wochen).**

***Warum der Tipp trotzdem bleibt:*** *Ein zurückkehrender Rechtsverteidiger, dessen Vertreter gelobt wurde, ist nach Regel 1 kein Tor — die Position war besetzt und bleibt besetzt. **Die Rückkehr verbessert Elversbergs Kader, nicht seine Torausbeute**, und 8 Tore in fünf Spielen gegen eine Mannschaft, die fünfmal mindestens zwei erzielt hat, bleibt der tragende Unterschied.*

**Bei Augsburg** fehlen nach dem Stand von gestern Banks (Knie) und Mounié; Breithaupt (Fuß) und Kade sind fraglich, eine Übersicht nennt für Breithaupt sogar den 16.10. als Rückkehrdatum. **Heute habe ich dazu nichts Neues gefunden** — *eine Aufstellungsprognose führt Dahmen und Ibrahimović als angeschlagen, weist das Spiel aber als „0:0" aus und ist damit erkennbar keine Vorberichtsseite; **ich verwende sie nicht.*** **Augsburgs Trainer bleibt unbelegt** (siehe Trainerabschnitt). **Keine der beiden Mannschaften spielt international.** ***Das ist die Partie mit der dünnsten neuen Informationslage dieses Laufs.***

### 4. SV Werder Bremen – SC Paderborn 07
**Samstag, 17.10.2026, 15:30 Uhr**
**Tipp: 2:1**
***unverändert***

**Begründung:** **Der klarste Formunterschied des Spieltags: Niclas Füllkrug steht bei vier Saisontoren, ist laut bundesliga.com der einzige Spieler der Saison mit zwei Kopfballtoren und hat in Dortmund in der 90.+2 per Kopf ausgeglichen** — *das 2:2 ist heute durch einen zweiten Vorbericht gegenbestätigt.* **Paderborn hat mit 3 Toren in fünf Spielen die schwächste Offensive der Liga** und verlor zu Hause 0:2 gegen Stuttgart.

***Das größte Einzelrisiko dieses Spieltags ist heute kleiner geworden:*** **Gestern musste ich acht Werder-Ausfälle gegen meinen eigenen Tipp stellen. Heute meldet die Lokalpresse aus dem Dienstagstraining: Senne Lynen ist zurück auf dem Platz, und Thioune standen 17 Feldspieler und vier Torhüter zur Verfügung.** *Für Lynen kann Samstag „noch etwas zu früh" kommen, die Entscheidung fällt in den kommenden Tagen; zu Amos Pieper (Prellung aus Dortmund) existiert ein Update, dessen Inhalt ich nicht verifizieren konnte.* ***17 Feldspieler sind kein komfortabler Kader, aber eine Startelf plus sechs Feldspieler auf der Bank*** — *das ist etwas anderes als das Bild von gestern, und es stützt den Tipp, den ich gestern sehenden Auges gegen die Ausfallliste gehalten habe.*

**Warum nicht 2:0:** **Werder hat 10 Gegentore in fünf Spielen.** *Gegen eine Abwehr, die zwei pro Spiel zulässt, überwiegt „ein Paderborner Tor" gegenüber „keinem" — und Regel 3 verbietet das Zu-null ohnehin.* **Zu Paderborn selbst habe ich zum dritten Tag in Folge keine eigene Verletztenliste gefunden.** **Keine der beiden Mannschaften spielt international.**

### 5. 1. FC Union Berlin – Borussia Dortmund
**Samstag, 17.10.2026, 15:30 Uhr** (An der Alten Försterei)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Der größte Tabellenabstand des Spieltags: Dortmund 13 Punkte und 11:4, Union 4 Punkte und 5:17 — die schlechteste Tordifferenz der Liga.** **Dortmund ist ungeschlagen, hat auswärts in Hoffenheim 3:2 und in Stuttgart 1:0 gewonnen und spielt unter Niko Kovač in jedem Pflichtspiel außer dem Pokalauftritt ein 3-4-3.** **Der direkte Vergleich: 16 Pflichtspiele, elf Dortmunder Siege, vier für Union, ein Remis.**

***Hier hat die offizielle Vereinsmeldung des Tages die Begründung von gestern umgedreht — und meine eigene Schwelle greift exakt so, wie ich sie formuliert habe:*** **Der BVB reist mit 23 Spielern nach Bodø, aber ohne Nico Schlotterbeck. Der Verein hat am Dienstag mitgeteilt, dass der Abwehrchef „aus reiner Vorsicht" geschont wird und keine akute Verletzung vorliegt.** **Julian Ryerson, der gestern auf meiner Ausfallliste stand, ist nach seiner Länderspielverletzung zurück im Kader.** **Neben Mane hat Kovač drei weitere Nachwuchsspieler nominiert (Kaua Prates, Samuele Inacio, Mathis Albert).** **Die Mannschaft fliegt nach dem Spiel zurück nach Dortmund und reist bereits am Freitag nach Berlin.**

***Was das für den Tipp bedeutet, und warum er trotzdem nicht steigt:***

- ***Das Belastungsargument für Union, das gestern die eine Hälfte meiner Begründung trug, ist deutlich schwächer geworden.*** *Gestern schrieb ich, die Reise nach Nordnorwegen „verschärft den Faktor deutlich". **Heute ist belegt, dass der BVB den Faktor aktiv bewirtschaftet:** der Abwehrchef bleibt zu Hause, vier Nachwuchsspieler fliegen mit, der Rückflug ist noch für die Nacht geplant. **Dortmund behandelt Bodø sichtbar als das Spiel, für das rotiert wird — nicht Berlin.***
- ***Schwelle 3 ist ausgelöst, und zwar im Zweig „bleibt 1:2".*** *Sie lautete wörtlich: „Wird ein Dortmunder Ausfall **mit genannter Ersatzlösung** gemeldet, der die Innenverteidigung betrifft, gehe ich auf 2:2. Wird nach dem Bodø-Spiel eine Dortmunder Rotation für Berlin **belegt angekündigt**, gehe ich ebenfalls auf 2:2. **Wird Schlotterbeck belegt fit gemeldet, bleibt 1:2.**" **Der dritte Zweig ist erfüllt: „keine akute Verletzung, reine Vorsicht" ist eine Fitmeldung mit Vereinsquelle.** Der erste Zweig ist nicht erfüllt (kein Innenverteidiger-Ausfall), der zweite nicht (die angekündigte Rotation betrifft Bodø, nicht Berlin).*
- ***Warum ich nicht auf 1:3 gehe, obwohl die Begründung in Dortmunds Richtung gekippt ist.*** **Meine Schwelle von gestern kannte für diesen Fall nur den Zweig „bleibt" — keinen Zweig „mehr Dortmunder Tore".** *Ich halte mich daran. **Eine Schwelle, von der ich abweiche, sobald die Information in die für mich bequeme Richtung zeigt, ist keine Schwelle.** Dass Union 17 Gegentore in fünf Spielen hat und Dortmund 2,2 Tore pro Spiel erzielt, würde ein 1:3 rechnerisch tragen; **ich schreibe das hin und setze es unten als neue Schwelle, statt es heute nachträglich in den Tipp zu schieben.** Abweichen von einer Schwelle habe ich gestern einmal getan und ausführlich begründet (Partie 9); zweimal hintereinander wäre es ein Muster.*

**Unions Lage ist unverändert:** **Markgraf (Kreuzbandriss bis voraussichtlich Anfang März 2027), Ilić (mehrere Wochen), Juranović (Erkrankung, ein bis zwei Wochen), dazu Friedrich, N'Soki und Burke (Achillessehne).** **Union hat zuletzt 1:0 gegen Elversberg seinen ersten Saisonsieg geholt**, Lustrinelli lobte „eine reife, konstante Leistung über 90 Minuten", **und an der Alten Försterei habe ich am 5. Spieltag genau einen Tipp verloren.** *Deshalb bleibt es beim Union-Tor.*

### 6. Hamburger SV – VfB Stuttgart
**Samstag, 17.10.2026, 15:30 Uhr** (Volksparkstadion)
**Tipp: 1:2**
***unverändert***

**Begründung:** **Beide stehen bei 6 Punkten, der Unterschied liegt in der Abwehr: HSV 15 Gegentore in fünf Spielen, Stuttgart 9.** **Die Heimbilanz des HSV ist die schwächste Teilbilanz dieses Spieltags: drei Punkte und 2:6 Tore aus drei Heimspielen** — *zwei erzielte Tore in drei Heimspielen, und darauf steht das eine HSV-Tor unten.* **Stuttgart holte mit dem 2:0 in Paderborn den ersten Auswärtssieg; Stiller legte beide Tore auf.** **Die Anstoßzeit ist heute mehrfach mit 15:30 bestätigt** — *die gestrige `sport.de`-Abweichung (18:30) halte ich damit endgültig für einen Fehler.*

***Die neue Information spricht gegen meinen Tipp, und sie kommt aus der offiziellen Vereinsquelle:*** **Laut HSV-Bericht vom Dienstag standen Bilal Nadir (Adduktoren) und Zakaria El Ouahdi (Erkältung) wieder auf dem Platz** — sie begannen mit der Mannschaft und wechselten nach rund einer halben Stunde ins individuelle Programm mit Reha-Coach Sebastian Capel. **Bakery Jatta (Adduktoren) fehlte angeschlagen.** **Grønbæk und Daka arbeiten weiter individuell; laut Hamburger Morgenpost kommt das Duell gegen Stuttgart für beide zu früh.** ***Der HSV schreibt ausdrücklich, dass der Kadereinsatz der Rückkehrer vom weiteren Trainingsverlauf abhängt*** — *und genau deshalb bleibt der Tipp: **nach Regel 1 ist „stand wieder auf dem Platz, Einsatz offen" keine Verstärkung, die ich in ein Tor umrechne.** Ein 90min-Bericht hat gestern aus denselben Meldungen „Trio vor schnellem Comeback" gemacht; die Vereinsmeldung ist zurückhaltender, und ich folge der Vereinsmeldung.*

**Zulasten des HSV steht dagegen eine Verschärfung:** **Remberg muss operiert werden.** *Der Kreuzbandriss war gestern bestätigt, die Operation ist heute neu — ein Kapitänsausfall über Monate, ohne jede Rückkehrperspektive für die Hinrunde.* **Dazu nennt eine Übersicht Torwart Fernando Dickes mit Schulterproblemen** *(Wett-Portal, einzeln; ich führe es als Hinweis, nicht als Argument).*

**Auf Stuttgarter Seite ist die Lage heute uneinheitlich, und ich löse den Widerspruch nicht auf:** **Die Mannschaft ist am Dienstagnachmittag von Echterdingen nach Bratislava geflogen, die PK mit Hoeneß und Leo Sauer war für 18 Uhr angesetzt, und Hoeneß hält sich zur Startelf bedeckt.** ***Zu Maximilian Mittelstädt widersprechen sich die Quellen offen:*** **ein Portal führt ihn unter den Ausfällen für Bratislava, zwei andere in der voraussichtlichen Startelf, und eine Verletztenliste nennt ihn nicht.** *Gestern hatte ich eine genähte Fersenwunde und ein voraussichtliches Fehlen in Bratislava notiert. **Beide Lesarten lassen seinen Einsatz am Samstag offen, und ich verwende ihn deshalb in keiner Richtung.*** **Chabot erscheint in mehreren Prognosen als Innenverteidiger** (gestern: Oberschenkelproblem laut Verein nicht schwerwiegend). **Weiter fehlen nach dem Stand von gestern Diehl, Malanga und Zagadou; Nartey und Al-Dakhil sind angeschlagen.**

**Was gegen meinen Tipp spricht:** **Stuttgart spielt Mittwoch in Bratislava und tritt am Samstag zum zweiten Auswärtsspiel binnen vier Tagen an, der HSV ist spielfrei, hat zwei Siege in Serie und bekommt möglicherweise drei Spieler zurück.** *Das ist ein echtes Gegenargument und es ist heute stärker als gestern. **Ich bleibe bei 1:2, weil der HSV zu Hause in drei Spielen zwei Tore erzielt hat und seinen Kapitän dauerhaft verloren hat** — und weil keiner der drei Rückkehrer belegt im Kader steht.*

### 7. FC Bayern München – RB Leipzig
**Samstag, 17.10.2026, 18:30 Uhr**
**Tipp: 2:1**
***unverändert***

**Begründung:** **Bayern hat mit 16:4 die beste Offensive der Liga und ist ungeschlagen, hat aber zwei der fünf Spiele unentschieden gespielt.** **Leipzig kommt vom 6:0 gegen Frankfurt und hat mit 5 Gegentoren die zweitbeste Abwehr der Liga.** *Rechnerisch komme ich für Bayern auf etwa zwei, für Leipzig auf etwa ein Tor.*

***Dies ist die Partie, zu der heute die meiste neue Information vorliegt — und sie ist die unbequemste des Laufs:*** **Beide haben am Dienstag gespielt, und beide Ergebnisse stehen fest.** **Bayern kam bei Viking Stavanger nur zu einem 3:3**: 0:2 zur Pause (Stensness 2., Christiansen 38.), dann Kane per Elfmeter (54.) und erneut (60.), Díaz zum 2:3 (71.) — **und in der 90. Minute der Ausgleich durch Herman Haugen.** **Kompany reagierte zur Pause mit drei Wechseln (Davies, Upamecano, Saibari) und nach dem Platzverweis mit Stanišić und Ito.** **Michael Olise sah in der 73. Minute Gelb-Rot, bestätigt durch VAR-Überprüfung**, nachdem er dem Viking-Kapitän den Ball ins Gesicht geworfen hatte. **Leipzig gewann zu Hause 1:0 gegen PSV** — Gruda (75.), Vandevoordt hielt in der 19. einen Elfmeter von Perišić; laut Spielbericht ein verdienter Sieg wegen der stärkeren zweiten Hälfte und der erste der Ligaphase.

***Warum der Tipp trotzdem 2:1 bleibt, und wo ich mir dabei unsicher bin:***

- ***Olises Platzverweis hat für Samstag keine Folge.*** **Gelb-Rot in der Champions League sperrt für das nächste Europapokalspiel, nicht für die Bundesliga.** *Ich schreibe das ausdrücklich hin, weil es die naheliegende Fehlschlussquelle dieser Partie ist. **Was ich nicht behaupte: dass die Szene vereinsinterne Folgen hat** — dazu habe ich keine Fundstelle, und ich habe heute ausdrücklich nach Reaktionen und Kritik gesucht und keine gefunden.*
- ***Die Belastung ist jetzt gemessen statt geschätzt, und sie fällt leicht zugunsten Leipzigs aus.*** **Beide haben volle 90 Minuten gespielt, beide haben bis Samstagabend dieselbe Erholungszeit — aber Bayern muss aus Norwegen zurückreisen und hat nach dem Platzverweis rund 20 Minuten in Unterzahl gearbeitet.** *Gestern hatte ich diesen Vorteil für Leipzig als Grund genannt, **nicht über 2:1 hinauszugehen.** **Heute ist er belegt, und er begründet die Obergrenze weiterhin — nicht mehr.***
- ***Die Versuchung, aus dem 3:3 ein Leipzig-Tor mehr zu machen, weise ich zurück — und das ist die Entscheidung, an der dieser Tipp hängt.*** *Bayern hat gegen einen norwegischen Außenseiter drei Gegentore kassiert; das lädt dazu ein, Leipzig unten ein zweites zu geben (2:2). **Dagegen stehen drei Dinge: Bayern hat in der Bundesliga 4 Gegentore in fünf Spielen; Bayern hat in Stavanger selbst drei Tore erzielt und Kane hat zweimal getroffen; und ein Auswärtsspiel am Polarkreisrand in einer anderen Wettbewerbslogik ist ein schlechter Schätzer für ein Heimspiel an der Säbener Straße.*** **Genau diese Übersetzung eines einzelnen Spiels in Gegentore war mein wiederkehrender Fehler am 5. Spieltag** — damals mit Ausfalllisten, hier wäre es mit einem Ergebnis. *Ich lasse es, und ich benenne das als die Stelle, an der dieser Tipp fällt, wenn er fällt.*

**Personalien:** **Musiala fehlt mit einem Muskelfaserriss im Oberschenkel aus der Länderspielpause; ein Rückkehrdatum ist nicht genannt, Bayern plant weiter ohne ihn.** **Laimer fehlt wegen Vaterfreuden.** **Bei Leipzig fehlen Ouédraogo (bis Jahresende), Baumgartner (bis Ende Oktober) und Viggo Gebel (Kreuzbandriss); Guiu wird mit einer Oberschenkelverletzung geführt.** ***Zu dieser Partie gibt es auch heute keinen Vorbericht*** — *die beiden Dienstagsergebnisse ersetzen ihn teilweise, die Personallage für Samstag nicht.* **Eine PK ist für keinen der beiden Vereine angesetzt.**

### 8. Bayer 04 Leverkusen – SC Freiburg
**Sonntag, 18.10.2026, 15:30 Uhr**
**Tipp: 2:2**
***unverändert***

**Begründung:** **Das Spitzenspiel des Spieltags: Vierter gegen Ersten, 14:8 gegen 14:4.** **Leverkusen holte in Mainz mit dem 4:3 den ersten Auswärtssieg, Patrik Schick führt mit fünf Treffern die Torjägerliste an.** **Freiburg ist ungeschlagen, steht bei einem Vereinsrekord von 13 Punkten und hat gegen Schalke in Unterzahl gewonnen.** **Freiburg hat mit 4 Gegentoren die beste Abwehr der Liga, Leverkusen mit 8 eine durchschnittliche; Leverkusen hat Heimrecht und den Torjäger, Freiburg die Stabilität und den Lauf.** *Beide haben zusammen 28 Tore in zehn Spielen erzielt — ein 2:2 folgt den Offensivzahlen.*

***Zu dieser Partie ist die Quellenlage heute schlechter als gestern, und das ist der einzige Rückschritt des Laufs:*** **Die Suche liefert ausschließlich Material zu früheren Begegnungen; die jüngsten Treffer sind rund 220 Tage alt** (verworfene Fundstelle 3). **Gestern hatte ich einen Vorbericht, heute keinen.** *Ich führe die Personallage daher unverändert aus dem Vortagsstand weiter und kennzeichne sie als Stand vom 12.10.:* **Suzuki fehlt Freiburg gesperrt (Sperre bis 25.10., nur Bundesliga), dazu Muslija (Kreuzbandriss, bis ins neue Jahr), Beste (ohne Rückkehrdatum), Osterhage (Muskelverletzung) und Yılmaz (nach Zahnoperation, laut Schuster „noch ein paar Tage"). Bei Leverkusen fehlen Kofane (Oberschenkel), Doué (Wade), Mbamba (Oberschenkelbeuger) und der erkrankte Eichhorn; Ben Seghir und Culbreath sind fraglich.** **Leverkusens Trainer kann ich für 2026/27 nicht belegen** (siehe Trainerabschnitt).

**Die Belastung bleibt nahezu symmetrisch:** **beide spielen Donnerstag — Leverkusen um 18:45 auswärts bei Lech Posen, Freiburg um 21:00 zu Hause gegen FK Jablonec** — *mit einem kleinen Vorteil für Freiburg, das nicht reisen muss, und einem für Leverkusen, das drei Stunden früher fertig ist. Das Unentschieden bleibt das konsistente Ergebnis.*

**Schwelle 3 (alte Nummerierung) geprüft:** *Sie verlangte eine **veröffentlichte Freiburger Startelf** mit mindestens zwei weiteren Ausfällen neben Suzuki, oder Maza belegt als Starter. **Keine Startelf ist veröffentlicht, und zu Maza gibt es auch heute keine Meldung.** Nicht ausgelöst.*

### 9. Borussia Mönchengladbach – TSG Hoffenheim
**Sonntag, 18.10.2026, 17:30 Uhr**
**Tipp: 1:1**
***unverändert*** — *die gestrige Änderung (2:1 → 1:1) hält.*

**Begründung:** **Letzter gegen Siebzehnten, und beide stehen unter Druck.** **Für Gladbach ist es das erste Heimspiel unter Alexander Blessin** (Vertrag laut Klub bis 2028), **nach der 1:2-Derbyniederlage in Köln, die El Mala entschieden hat.** **Eine WDR-Analyse von heute hält fest, dass Gladbach auch unter Blessin „viele Baustellen" hat — in allen Mannschaftsteilen, vom Torwart Moritz Nicolas bis zum Mittelstürmer Isac Lidberg — und nur „starke Ansätze und Phasen" zeigt.** *Dieselbe Analyse bestätigt, dass Blessin im Derby auf die angeschlagenen Itakura, Honorat und Kleindienst verzichten musste.* **Hoffenheim hat vier der fünf Spiele verloren, 13 Gegentore, und über die TSG wird öffentlich von einer Krise gesprochen.**

***Die neue Information stützt den Tipp auf der Hoffenheimer Seite, und sie ist konkreter als gestern:*** **Hoffenheim spielt Donnerstag um 21:00 zu Hause gegen Beşiktaş — und der Gegner ist in Form: Beşiktaş hat zum Auftakt 4:1 gegen Olympique Marseille gewonnen, während Hoffenheim 0:2 bei OFI Kreta verlor.** ***Ein Verein mit drei Punkten, der am Donnerstagabend um 21:00 ein Europa-League-Heimspiel gegen einen Gegner dieser Form bestreiten muss und am Sonntag um 17:30 in Mönchengladbach antritt, trägt den Belastungsnachteil, auf dem mein 1:1 ruht*** — *und dieser Nachteil ist heute größer als gestern, weil die sportliche Notwendigkeit des Donnerstagsspiels sichtbar geworden ist: nach einer Auftaktniederlage kann Hoffenheim nicht rotieren.* **Dazu kommen Ausfälle: Bernardo fehlt** (Gelb-Rot-Sperre bis 25.10. oder Achillessehne — siehe Korrektur 3; **meine gestrige Angabe „Ersatz Mats Rots" streiche ich**), **Hajdari (Knie) ist laut Ilzer zurück im leichten Training mit offenem Einsatz, Wimmer (Oberschenkel) ist fraglich.** **Gladbach ist spielfrei.**

**Zu Kleindienst gibt es heute nichts Belastbares Neues, und ich bleibe ausdrücklich beim Stand von gestern.** *Belegt ist: er hat das Derby wegen muskulärer Beschwerden verpasst, der Verein hat weder Diagnose noch Ausfalldauer veröffentlicht und hofft auf eine baldige Rückkehr. **Eine Fundstelle nennt einen Trainingsabbruch „am Dienstag", lässt aber offen, ob der 6.10. oder der 13.10. gemeint ist — ich verwende sie deshalb nicht.*** **Die Ko-Itakura-Diagnose von gestern (Muskelfaserriss im linken mittleren Gesäßmuskel, zugezogen bei der Nationalmannschaft) steht unverändert.**

**Schwelle 4 geprüft:** *Alle drei Zweige sind **nicht** ausgelöst. **Kein Kleindienst-Einsatz ist belegt bestätigt** (sonst zurück auf 2:1), **sein Ausfall für Sonntag ist nicht belegt bestätigt** (dann bliebe 1:1 ohne weitere Prüfung), **und eine Hoffenheimer Entwarnung zu einem Stammspieler liegt nicht vor** — Hajdaris leichtes Training ist keine Entwarnung, sondern eine offene Lage. *Der Tipp bleibt also aus demselben Grund wie gestern, und die Unsicherheit ist dieselbe.*

**Was gegen meinen Tipp spricht:** ***Gladbach hat null Punkte aus fünf Spielen und mit 18 Gegentoren die schlechteste Abwehr der Liga*** — *gegen diese Abwehr ist ein Hoffenheimer Sieg jederzeit möglich, Europapokal hin oder her.* *Nach Regel 2 werte ich Gladbach nicht wegen der Tabellenposition ab; die Abwertung von gestern beruhte auf der Personalinformation zu Kleindienst und Itakura, und die gilt weiter.*

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
| Bayern – Leipzig | Sa 18:30 | **2:1** | unverändert | **Di auswärts 3:3** / **Di heim 1:0** |
| Leverkusen – Freiburg | So 15:30 | **2:2** | unverändert | **Do auswärts** / **Do heim** |
| Gladbach – Hoffenheim | So 17:30 | **1:1** | unverändert | — / **Do heim** |

**Verteilung:** **3 Heimsiege, 4 Auswärtssiege, 2 Unentschieden** — *unverändert gegenüber gestern.* **Kein einziger Zu-null-Tipp** (Regel 3 eingehalten). **Keine Partie ohne Tor der Heimmannschaft.** **27 Tore in neun Partien, exakt 3,0 pro Spiel.**

***Zur Selbstkontrolle gehört heute die Frage, ob „neunmal unverändert" ein Ergebnis oder eine Unterlassung ist.*** **Mein Befund: ein Ergebnis — aber nur, weil drei Schwellen tatsächlich geprüft und ausgelöst wurden, nicht weil nichts passiert ist.** *Zentners Ersatz ist benannt (Schwelle 2 → bleibt). Schlotterbeck ist fit gemeldet (Schwelle 3 → bleibt). Zu Skhiri ist eine Ersatzlösung benannt statt eines neuen Ausfalls (Schwelle 1 → nicht ausgelöst). **An zwei Partien hätte ich heute mit guten Argumenten ändern können — Bayern – Leipzig auf 2:2 und Union – Dortmund auf 1:3 — und ich habe es in beiden Fällen bewusst nicht getan und den Grund jeweils hingeschrieben.*** **Wenn dieser Lauf falsch ist, ist er an diesen zwei Stellen falsch.**

**Die vier Schwellen für die nächsten Läufe — zwei neu, weil zwei alte heute abgearbeitet sind:**

1. **Frankfurt – Köln (fortgeführt):** *Die PK ist morgen. Wird eine Frankfurter Startelf oder ein Kaderaufgebot veröffentlicht, in dem **Koch nicht steht**, gehe ich auf 1:1. Wird ein **neuer** Kölner Ausfall im Mittelfeld oder in der Offensive **mit genannter Ersatzlösung** gemeldet, gehe ich auf 3:1. Bei beiden gilt der zuerst genannte.*
2. **Union – Dortmund (neu, weil Schwelle 3 abgearbeitet ist):** *Wird nach dem Bodø-Spiel belegt, dass Schlotterbeck **in Berlin spielt** (Startelf, Kaderaufgebot oder Kovač-Aussage auf einer Spieltags-PK), **und** ist Unions Ausfallliste unverändert, gehe ich auf **1:3** — das ist die Zahl, die Unions 17 Gegentore in fünf Spielen tragen und die ich heute nur deshalb nicht genommen habe, weil meine Schwelle sie nicht vorsah. Wird umgekehrt ein Dortmunder Innenverteidiger-Ausfall **mit genannter Ersatzlösung** gemeldet oder eine Rotation **für Berlin** belegt angekündigt, gehe ich auf 2:2.*
3. **Bayern – Leipzig (neu, weil die Partie jetzt die unsicherste ist):** *Wird eine Bayern-Verletzung **aus dem Stavanger-Spiel** gemeldet **und** eine Ersatzlösung benannt, oder kündigt Kompany auf der Spieltags-PK eine Rotation für Samstag belegt an, gehe ich auf **2:2**. Wird Musialas Rückkehr belegt gemeldet (Kaderaufgebot, nicht Prognose), gehe ich auf 3:1. Allein das 3:3 von Stavanger löst keinen der beiden Zweige aus — das ist der Punkt, an dem ich mich heute festlege.*
4. **Gladbach – Hoffenheim (fortgeführt):** *Wird Kleindiensts Einsatz belegt bestätigt (Startelf oder Kaderaufgebot, nicht Prognose), gehe ich auf 2:1 zurück. Wird sein Ausfall für Sonntag belegt bestätigt, bleibt 1:1, und 0:1 prüfe ich nicht, solange Hoffenheim Donnerstag spielt. **Neu:** Verliert Hoffenheim am Donnerstag gegen Beşiktaş **und** steht Kleindienst belegt im Kader, gehe ich auf 2:1 — die Gladbacher PK am Freitag ist dafür die erste Gelegenheit.*

**Was dieser Lauf geleistet hat:** **die Ursache des dreitägigen Abrufproblems host-genau geklärt und als Einstellungsfrage der Umgebung benannt, mit der Stelle zum Ändern** · **die beiden ersten Pflichtspielergebnisse der Woche erfasst und für Partie 7 ausgewertet** (Bayern 3:3, Leipzig 1:0, inklusive Torschützen, Minuten, Wechsel und Platzverweis) · **erstmals offizielle Vereinsquellen zum Spieltag ausgewertet** (`bvb.de`-Reisekader mit der Schlotterbeck-Fitmeldung, `hsv.de`-Personalupdate, `vfb.de`) · **drei der vier gestrigen Schwellen abgearbeitet, alle drei im Zweig „bleibt", und die Auslösung jeweils an der Formulierung geprüft** · **Skhiris Diagnose auf Syndesmoseriss und drei Monate präzisiert und, wichtiger, drei benannte Kölner Ersatzlösungen gefunden, die meine gestrige Begründung zu Partie 1 widerlegen** · **Zentners Ersatz identifiziert und als etatmäßigen zweiten Torwart mit Zu-null-Spiel eingeordnet** · **die PK-Termine des Spieltags beschafft** (erste PK morgen) · **zwei fehlende Trainernamen belegt (Kovač, Vincent Wagner) und zwei weitere ausdrücklich offen gelassen, statt sie aus altem Material zu übernehmen** · **die eigene Tabelle zum zweiten Mal fremdbestätigt, dazu drei Einzelergebnisse und den Derbyausgang** · **fünf Korrekturen am Vortagsstand, darunter eine eigene falsche Behauptung („nur ein Elversberger Ausfall") und eine gestrichene Nebenangabe (Rots)** · sieben Fundstellen geprüft und verworfen, darunter eine Flashscore-Seite aus 2023/24 und eine Verwechslung von verletzten Zuschauern mit verletzten Spielern.

**Was dieser Lauf nicht geleistet hat:** **kein Volltext einer einzigen Quelle — die Hosts sind durch die Netzwerk-Policy gesperrt, und das wird sich ohne Eingriff des Nutzers nicht ändern** · **keine Spieltags-Pressekonferenz** (es hat noch keine gegeben) · **kein Vorbericht zu Leverkusen – Freiburg, erstmals schlechter als gestern** · **kein Vorbericht zu Bayern – Leipzig** · **keine offizielle Bundesliga-Startelf oder -Kaderliste zu irgendeiner Partie** · **keine Verletztenliste zu Paderborn, dritter Tag** · **Augsburgs und Leverkusens Trainer unbelegt** · **Kleindiensts Status offen, Mittelstädts Status widersprüchlich, Musialas Rückkehr offen** · **die Zentner-Chronologie bleibt widersprüchlich** · **Freiburgs Torverhältnis bleibt zwischen 13:3 und 14:4 strittig.**

---

## Quellen

**Alle Fundstellen stammen aus Suchergebnis-Zusammenfassungen und -Titeln. Kein Volltext — siehe Hinweis zur Quellenlage.** **Datumsangaben, wo die Suche sie geliefert hat.**

**Dienstagsergebnisse (neu):** `sportschau.de` (Spielbericht Leipzig – Eindhoven, „Gruda erlöst Leipzig") · `rbleipzig.com` (Liveticker/Spielbericht 13.10.2026) · `sport.de` (Liveticker Leipzig – PSV 1:0; Liveticker Viking – Bayern 3:3) · `dazn.com` (Liveticker Viking – Bayern) · `t-online.de` (Liveticker und Bericht „Bayern stolpert beim Außenseiter in Stavanger") · `fcbinside.de` / `footy.de` („Spektakel in Stavanger! Bayern patzt, Olise fliegt vom Platz", 13.10.) · `oe24.at` (Matchbericht) · `vavel.com` (beide Spiele) · `fussballnationalmannschaft.net` (beide Spiele)

**Offizielle Vereinsquellen (neu):** `bvb.de` („Schlotterbeck fehlt, Ryerson dabei: Mit diesen BVB-Profis geht's nach Norwegen", 13.10.; Ticker zur Bodø-Reise) · `hsv.de` („Personal-Update vor Stuttgart-Heimspiel") · `vfb.de` (PK vor Slovan Bratislava; Faninfos Bratislava) · `tsg-hoffenheim.de` (Ilzer-PK-Bericht, älter)

**Vorberichte, Personal und Termine 6. Spieltag:** `ligainsider.de` („Zentner weiter eingeschränkt – Schalke wohl zu früh", 13.10.; „6. Spieltag: Die PK-Termine in der Übersicht"; Teamseiten Schalke, Mainz, Werder, Frankfurt, Hoffenheim — mit Altersvorbehalt) · `sportschau.de`/WDR („Auch unter Blessin hat Gladbach viele Baustellen"; „Kölns El Mala entscheidet rheinisches Derby") · `stuttgarter-nachrichten.de` (Abflug nach Bratislava) · `deichstube.de` (Werder-Personalupdate, Lynen zurück im Training) · `weser-kurier.de` („Schon wieder viele Ausfälle"; „Lynen zurück im Training, Update bei Pieper") · `absolutfussball.com` (Gyamerah-Ausfall „Schlag" für SVE, mit Wagner-Zitat) · `africasoccer.com` (Gyamerah vor Elversberg – Augsburg; El Ouahdi) · `90min.de` („Lazarett lichtet sich: HSV-Trio vor schnellem Comeback") · `nurdieraute.de` (12.10., HSV-Rückkehrer) · `magazin.comunio.de` (Verletzten-Update HSV/Skhiri) · `wochenblatt-reporter.de` („Eintracht Frankfurt vor Köln-Spiel: Defensive im Fokus") · `anstosszeiten.de` (Spieltagsübersicht, Vorbehalt zur Zeitgenauigkeit) · `ruhrnachrichten.de` (TV-Übersicht 6. Spieltag) · `wetttippsheute.net` (Verletzungs-Radar 13.–18.10., Stand 12.10.; Vorberichte HSV – Stuttgart, Union – Dortmund, Hoffenheim – Beşiktaş; **nur Ausfalllisten und Termine, keine Prognosen**)

**Skhiri und Köln:** `wp.sport1.de` („Längere Pause für Kölns Skhiri") · `fussballdaten.de` (Skhiri-Update) · `koeln.t-online.de` (Diagnose; „Wagner setzte nach Skhiri-Aus auf Tom Krauß") · `neunzigplus.de` (Skhiri fällt länger aus) · `come-on-fc.com` (Skhiri verletzt; „klare Transfer-Entscheidung" mit Kessler-Zitat) · `geissblog.koeln` (Derby-Schock) · `kicker.at` (Wagners Debüt in Frankfurt, April 2026)

**Europapokalwoche:** `uefa.com` / `de.uefa.com` (Hoffenheim – Beşiktaş; Ligaphase) · `bundesliga.com` (CL-Liveticker beide Dienstagsspiele; Bodø/Glimt – BVB-Vorschau) · `sport1.de` („Borussia Dortmunds skurriler Champions-League-Trip") · `foxsports.com` / `365scores.com` (Hoffenheim – Beşiktaş, Termin) · `goal.com` (Übertragung Leipzig – PSV; Slovan – VfB)

**Verworfen oder nur mit Vorbehalt verwendet** (siehe eigener Abschnitt): `flashscore.de` (6. Spieltag 2023/24) · `tipico.de` (Bodø – BVB, Dezember 2025; Slovan – VfB) · `fotmob.com` (undatierte Kader- und Trainerangaben) · `footy.de` (Zentner, 15./16.09.2026) · `news.de` (verletzte Zuschauer beim Derby) · `sportsmole.co.uk` / `zdfheute.de` / `fussballdaten.de` (Leverkusen- und Freiburg-Material aus 2025/26)
