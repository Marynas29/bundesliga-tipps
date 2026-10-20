# Bundesliga-Tipps – 7. Spieltag 2026/27 (Stand: 19.10.2026)

**Ansetzung:** Freitag, 23.10. bis Sonntag, 25.10.2026.
**Vortagsstand:** 18.10.2026, **ebenfalls 7. Spieltag** — also ist ein echter Vergleich für alle neun Partien möglich.

**Ergebnis dieses Laufs in einem Satz:** **Kein einziger Tipp geändert, alle neun unverändert** — **und das ist heute das sachlich richtige Ergebnis, kein Ausweichen.** ***Der Grund ist nachprüfbar:*** **am Montag vor einem Spieltag, der erst Freitag beginnt, existiert keines der Beweisstücke, die meine neun Schwellen ausdrücklich verlangen** (Kaderaufgebot, Startelf, belegte Rotationsankündigung). **Neu hinzugekommen sind trotzdem fünf verwertbare Personalien, zwei davon kurz vor einer Schwelle.** ***Die wichtigste: Gladbachs Nicolas Kühn hat eine Stunde im Mannschaftstraining absolviert, und Blessin nennt ihn selbst für „spätestens nächste Woche" — das ist genau dieser Spieltag.*** **Eine Korrektur am Vortagsstand war nicht nötig; den einen Punkt, der danach aussah (Kölns Trainername), habe ich geprüft, und der Vortagsstand hat gehalten.** **Die Quellensperre besteht zum neunten Tag.**

---

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Zwei Dinge sind heute anders als an den Vortagen, eines davon neu.**

- ***NEU und ausdrücklich zu melden: die Proxy-Statusabfrage selbst wurde heute blockiert.*** **`curl -sS "$HTTPS_PROXY/__agentproxy/status"` wurde vom Auto-Mode-Klassifizierer der Sitzung abgelehnt** (Begründung: `Exfil Scouting`). ***Das ist keine Netzsperre, sondern eine Berechtigungsgrenze meiner eigenen Sitzung*** — an den Vortagen lief dieser Befehl durch und belegte `enabled: true`. **Ich kann den Proxy-Zustand heute also nicht mehr direkt auslesen und führe ihn als unbelegt.** *Falls der Nutzer diese Prüfung weiter im Bericht haben will, muss er den Befehl in den Berechtigungen der Sitzung freigeben.*
- **Die Sperre der Leitquellen besteht unverändert, heute wieder direkt belegt.** **`www.kicker.de` und `www.bundesliga.com` über `WebFetch` getestet, beide enden mit `getaddrinfo ENOTFOUND`.** ***Das ist derselbe Befund wie seit dem 15.10.: die Namensauflösung scheitert, bevor überhaupt eine Verbindung versucht wird.***
- ***Was der Nutzer tun kann, wenn er Volltexte will:*** **Im Menü der Cloud-Umgebung in der Titelzeile der Sitzung → „Edit" → Network access**: entweder eine breitere Zugriffsstufe wählen oder `kicker.de`, `bundesliga.com`, `weltfussball.de` und `transfermarkt.de` unter **Allowed domains** eintragen (Häkchen „Allow package managers" gesetzt lassen). Dokumentiert unter https://code.claude.com/docs/en/cloud-environments#network-access. **Solange das so bleibt, kann ich die vier Leitquellen dauerhaft nicht im Volltext lesen.**
- **`WebSearch` funktioniert und war wieder die tragende Quelle.** **Alles Folgende steht auf Suchergebnis-Zusammenfassungen und -Titeln, kein Volltext.**
- ***Qualitativer Befund des Tages:*** **Schlechter als am 18.10., und zwar aus einem strukturellen Grund.** *Gestern waren die beiden Sonntagsspiele frisch und damit dicht belegt. Heute ist Montag: gespielt wurde nichts, die Spieltags-Pressekonferenzen liegen noch vier Tage entfernt, und was an Material kommt, betrifft die Europapokalwoche, nicht den Spieltag.* ***Der Anteil veralteter Treffer war heute auffällig hoch — ich habe sechs Fundstellen verworfen, darunter zwei, die ohne Gegenprüfung zu falschen Tippänderungen geführt hätten.***

---

## Die Nachrichtenlage

**Montag vor einer Europapokalwoche: die Nachrichten kommen heute aus den Abschlusstrainings und Pressekonferenzen der vier international spielenden Vereine, nicht vom Spieltag.**

**Erstens Dortmund, und hier schließt sich die Karetsas-Lücke von gestern fast vollständig.** **Der BVB ist heute nach Baku geflogen und hat einen 24-Mann-Kader nominiert; genannt werden unter anderem Kobel, Anton, Schlotterbeck, Bensebaini, Bellingham, Nmecha, Guirassy und Svensson.** ***Konstantinos Karetsas steht nicht im Kader, und Lars Ricken wird jetzt konkret: „Kos hat eine Bandverletzung im Fuß."*** *Gestern lag nur „umgeknickt, Schwere muss untersucht werden" vor.* **Nach den `Ruhr Nachrichten` ist eine Rückkehr nicht vor der Länderspielpause Mitte November zu erwarten, mehrere Berichte sprechen von wochenlangem Ausfall.** **Eine offizielle Vereinsdiagnose mit Ausfalldauer fehlt weiter.** **Kovač hat sich auf der Pressekonferenz klar positioniert: Dortmund sei „klarer Favorit" und müsse das Spiel gewinnen** — ***keine Rotationsankündigung, was für Partie 7 zählt.*** *Laut Liveticker wurde der Ablauf vor Ort geändert und das Abschlusstraining im Olympiastadion vorgezogen.*

**Zweitens Stuttgart, mit der dichtesten Personalmeldung des Tages.** **Auf der Montags-Pressekonferenz vor Atlético Madrid hat Hoeneß drei Rückkehrer genannt: Maximilian Mittelstädt ist nach einer Fersenverletzung zurück im vollen Mannschaftstraining und kann in den Kader, Nikolas Nartey und Ameen Al-Dakhil trainieren ebenfalls wieder mit.** **Tiago Tomás arbeitet weiter individuell und fällt für die Champions League voraussichtlich aus; Dan-Axel Zagadou wird als Ausfall genannt.** ***Die Torwartfrage hat Hoeneß offengelassen:*** **Dennis Seimen ist die gesetzte Nummer eins und hat die letzten beiden Bundesligaspiele gemacht, Bredlow hat die Champions-League-Erfahrung.** *Hoeneß nannte Atlético eine der besten Mannschaften Europas und betonte Struktur, Balance und Umschaltverteidigung.*

**Drittens Gladbach, und das ist die Mannschaft mit den zwei wichtigsten neuen Fakten des Tages.** ***Zum Guten:*** **Nicolas Kühn hat rund eine Stunde am Mannschaftstraining teilgenommen, danach Steigerungsläufe gemacht.** **Blessin wörtlich: „Da sind wir noch am abwägen, ob es dann für den Spieltag reicht … Aber spätestens nächste Woche sollte er zur Verfügung stehen."** ***Diese Aussage stammt aus der Zeit vor dem Hoffenheim-Spiel — „spätestens nächste Woche" bezeichnet damit genau die Woche des 7. Spieltags.*** ***Zum Schlechten, und zwar zweifach:*** **Blessin rechnet bei Tim Kleindienst mit einem Ausfall von etwa zwei weiteren Spielen, Stuttgart eingeschlossen.** **Und Isac Lidberg — gegen Hoffenheim die einzige Spitze — musste kurz nach dem Ausgleich mit Oberschenkelbeschwerden runter; ob eine Muskelverletzung vorliegt und wie lange er fehlt, ist offen.** *Ein Gladbacher Portal fragt bereits nach dem „9. Ausfall".* **Weiter geführt: Itakura, Leszczyński, Castrop, Leopold, Fleck und Honorat.**

**Viertens Leipzig, wo die Trainerfrage genau da steht, wo sie gestern stand — nur mit einem Beleg mehr dafür, dass Demichelis im Amt ist.** **Er hat sich heute in einer virtuellen Medienrunde zum Real-Spiel geäußert, einen Tag vor seiner eigentlichen Pressekonferenz am Dienstag, und inhaltlich über Ballbesitz und Reals Umschaltspiel gesprochen** („Solo necesitan dos pases…"). ***Damit ist belegt: Leipzig geht mit Demichelis ins Bernabéu.*** **Keine Vereinsmeldung über ein Aus, aber die Kritik läuft weiter** — *`sport.de` berichtet von harscher Kritik nach dem 1:6, und ein Bericht nennt Spekulationen über eine Nagelsmann-Rückkehr, für die es laut demselben Bericht keine konkrete Vereinbarung gibt.* **Das bleibt unbestätigt.**

**Fünftens Köln und Schalke, wo sich beide Offensivprobleme weiter verschärft haben.** ***Bei Köln eine echte Verbesserung:*** **Ragnar Ache ist teilintegriert ins Mannschaftstraining eingestiegen.** *Joël Schmied hat dort verletzt gefehlt; eine Diagnose zu seinem Umknicken vom 16.10. liegt weiterhin nicht vor, es bleibt beim Bänderverdacht.* **Unverändert aus: Dallinga, Rondic, Skhiri, van den Berg, Hübers.** ***Bei Schalke kommt ein Name hinzu:*** **Edin Džeko musste gegen Mainz nach einem Zusammenprall mit einer Platzwunde ausgewechselt werden und fällt laut Vorbericht womöglich aus.** **Sylla bleibt fraglich — Muslić: die Verletzung sei „nicht so tragisch", aber „ob wir es bis Köln schaffen, weiß ich nicht".** **Ljubičić fehlt mit Knieproblemen.**

**Sechstens Hoffenheim, wo die Nachrichtenlage schlechter ist als gestern.** **Nathan De Cat hat sich am linken Knie verletzt, eine Operation gilt als wahrscheinlich, und er fällt voraussichtlich länger aus; eine Ausfalldauer steht laut `kicker` nicht fest.** **Ozan Kabak gilt nach seiner Auswechslung gegen Beşiktaş als Sorgenfall, ohne offizielle Diagnose** — *er stand auch in der Startelf gegen Gladbach nicht.* **Ilzer sprach von „ein paar angeschlagenen" Spielern, ohne Namen.** **Hajdari fehlt weiter.**

**Siebtens Leverkusen, mit einem präzisierten Ausfall.** **Martin Terrier fällt mit seiner Oberschenkelverletzung bis Dezember aus** — *gestern stand dort nur „Oberschenkelverletzung".* **Dazu Ben Seghir, Doué, Eichhorn und Kofane.** ***Patrik Schick ist fit:*** **die Sorge um ihn nach dem 4:0 gegen Lech Posen hat er selbst ausgeräumt; er war in der 18. Minute für den verletzten Terrier gekommen, traf zweimal per Elfmeter und wurde in der 76. Minute ausgewechselt.**

**Achtens der HSV und Werder, beide ohne Europapokal und entsprechend ruhig.** **Beim HSV fehlen Grönbaek und Daka mit Muskelblessuren, dazu der verletzte Kapitän Remberg; Polzin sucht laut `sport1` neue Lösungen für die Offensive.** **Bei Werder gibt es keine Verletzungsmeldung zu Füllkrug** — *er und Grüll hatten vor einer Woche dosiert trainiert, der Verein nannte dafür ausdrücklich Belastungssteuerung, keine Beschwerden.*

**An der Spitze steht der FC Bayern mit 14 Punkten und 22:5 Toren vor Dortmund (14, 11:4).** **Ein DFB-Pokalspiel liegt in dieser Woche nicht an, eine Länderspielpause läuft nicht.** ***Zu beachten: in der Nacht zum Sonntag, 25.10.2026, wird die Uhr auf Winterzeit zurückgestellt — die beiden Sonntagsspiele finden in MEZ statt.***

### Die Europapokalwoche vor dem 7. Spieltag

**Die Tabelle ist gegenüber gestern unverändert; neu ist nur eine aufgelöste Zeitangabe und eine Personalie beim Gegner.**

| Tag | Partie | Wettbewerb | Lage | Reiseweite | Bundesligaspiel danach |
|---|---|---|---|---|---|
| **Di 20.10., 18:45** | Sabah FK – **Borussia Dortmund** | Champions League | **auswärts, Baku** | **sehr weit** | Sa 18:30 **heim** (4 Tage) |
| **Di 20.10., 21:00** | **VfB Stuttgart** – Atlético Madrid | Champions League | heim, MHP Arena | — | **Fr 20:30 heim (3 Tage)** |
| **Mi 21.10., 21:00** | **FC Bayern** – FC Arsenal | Champions League | heim | — | So 17:30 **auswärts** (4 Tage) |
| **Mi 21.10., 21:00** | Real Madrid – **RB Leipzig** | Champions League | **auswärts, Madrid** | **weit** | **Sa 15:30 heim (3 Tage)** |
| **Do 22.10., 18:45** | OFI Kreta – **Bayer Leverkusen** | Europa League, 3. ST | **auswärts, Kreta** | **sehr weit** | **So 15:30 auswärts (3 Tage)** |
| **Do 22.10., 21:00** | **TSG Hoffenheim** – Olympique Lyon | Europa League, 3. ST | **heim, SNP Arena** | — | **So 15:30 heim (3 Tage)** |
| **Do 22.10., 21:00** | AS Monaco – **SC Freiburg** | Conference League, 2. ST | **auswärts, Stade Louis-II** | **mittel** | So 17:30 **heim** (3 Tage) |

***Aufgelöst: der scheinbare Widerspruch bei Dortmunds Anstoßzeit.*** **Die Quellen von heute nennen „20:45 Uhr im Olympiastadion Baku", meine Tabelle führt 18:45.** **Beides ist richtig: Baku liegt bei UTC+4, Deutschland bis zum 25.10. bei UTC+2.** *20:45 Ortszeit sind 18:45 MESZ. Ich halte das fest, damit die Abweichung nicht als Fundstelle wiederkehrt.*

***Neu beim Gegner:*** **Monacos wertvollster Spieler Folarin Balogun ist nach einem am Deadline Day gescheiterten Transfer nicht für den Conference-League-Kader nominiert und fehlt Freiburgs Gegner am Donnerstag.** *Das macht Freiburgs Europapokalaufgabe eher leichter — für Partie 9 ein kleiner, aber echter Punkt.*

---

## Abrechnung des 6. Spieltags

**Unverändert gegenüber gestern, hier nur als Gedächtnis: vier von neun Tendenzen richtig, kein Endstand exakt.** *Die vollständige Tabelle steht im Archiv unter `archiv/2026-10-18.md`.* **Die drei Lehren daraus — Torflaute vor Tabellenplatz, keine Umrechnung fremder Ausfälle in eigene Tore, Tabellenletzter nach Personallage — sind in den vier Regeln unten verarbeitet.**

---

## Korrekturen und geschlossene Lücken

***Eine Korrektur war heute nicht nötig. Einen Punkt habe ich aber ausdrücklich gegengeprüft, weil er nach einem Fehler aussah — und der Vortagsstand hat gehalten.***

1. ***GEPRÜFT, VORTAGSSTAND BESTÄTIGT: Kölns Trainer heißt René Wagner.*** **Ein Suchtreffer von `absolutfussball.com` trug heute die Überschrift „Köln-Trainer Kwasniok gibt Update zu verletztem Schmied" und hätte damit meinen Vortagsstand widerlegt.** **Die Gegenprüfung entscheidet die Frage eindeutig gegen diesen Treffer:** **`zdfheute.de` führt unter dem Titel „Die Gründe für das Kwasniok-Aus beim 1. FC Köln", dass Lukas Kwasniok im März 2026 entlassen wurde und Co-Trainer René Wagner übernahm.** ***Der Kwasniok-Treffer betrifft eine frühere Verletzung Schmieds*** — *er hatte im November 2025 und im Februar 2026 Muskelverletzungen, und mehrere Treffer des Tages mischten diese mit dem Umknicken vom 16.10.2026.* **Ich halte das fest, weil es nach der Karetsas-Falschzuordnung von gestern der zweite Fall derselben Art ist: ein Treffer, der aktuell aussieht und eine Personalie der falschen Zeit zuordnet.**
2. **Karetsas' Verletzung ist präzisiert — Lücke von gestern weitgehend geschlossen.** **„Bandverletzung im Fuß" nach Ricken, Rückkehr laut `Ruhr Nachrichten` nicht vor Mitte November, und er fehlt im 24-Mann-Kader für Baku.** *Eine offizielle Vereinsdiagnose mit Ausfalldauer fehlt weiter — die Lücke ist verkleinert, nicht beseitigt.*
3. **Terriers Ausfalldauer ist belegt: bis Dezember.** *Gestern ohne Zeitangabe.*
4. **Kohrs Ausfalldauer tendiert jetzt klar zur längeren Variante — die seit Tagen offene Streitfrage ist damit entschieden, wenn auch nicht amtlich.** **`bundesliga.com` nennt eine Syndesmoseverletzung, eine Spielvorschau nennt eine Rückkehr Anfang Januar 2027.** ***Eine Syndesmoseverletzung passt zu Januar und nicht zu „Ende Oktober"*** — *ich führe die Angabe „Ende Oktober" ab heute als überholt.*
5. **Leipzig geht mit Demichelis ins Bernabéu.** *Belegt durch seine eigene Medienrunde von heute. **Das beantwortet nicht, ob er den Spieltag erlebt** — aber es beantwortet, dass bis heute Abend keine Entscheidung gefallen ist.*
6. **Ein aktueller, datierter Unioner Beleg ist erstmals seit Tagen aufgetaucht — die größte Lücke von gestern ist dadurch kleiner, aber nicht geschlossen.** **Der `Berliner Kurier` schreibt, Lustrinelli werde in Augsburg voraussichtlich erneut Uduokhai und van den Bosch aufbieten, womit Leopold Querfeld auf der Bank bliebe.** ***Das bestätigt Lustrinelli als Trainer aus einer heutigen Quelle*** (bisher stand er auf einem Beleg vom 15.10.) ***und zeigt, dass Union in der Abwehr keine Not hat.*** **Eine datierte Unioner Ausfallliste habe ich weiterhin nicht.**

---

## Tabelle nach dem 6. Spieltag

**Unverändert gegenüber dem 18.10.** *Sie war dort an fünf Werten unabhängig gegenbestätigt (`reviersport.de`, `sportschau.de`: Bayern 14/22:5, Dortmund 14/11:4, Freiburg 13, Leverkusen 13, Gladbach 0/8:20).* **Heute ist kein Spiel gelaufen, es gibt also nichts zu verschieben.**

| # | Verein | Sp | Tore | Diff | Pkt | Form (1.–6. ST) | Europapokal diese Woche |
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

---

## Heute geprüft und verworfen

***Der Anteil veralteter Treffer war heute der höchste aller Läufe. Zwei der sechs hätten ohne Gegenprüfung zu falschen Tippänderungen geführt — die beiden stehen deshalb zuerst.***

1. ***Eine Freiburger Kadermeldung, nach der Derry Scherhant und Niklas Beste mit Muskelproblemen kurzfristig fehlten.*** **Verworfen:** *sie betrifft das Conference-League-Spiel gegen FK Jablonec, also eine frühere Woche.* ***Warum das gefährlich war:*** **hätte ich Scherhant als Freiburger Ausfall übernommen, wäre Partie 9 nach unten gerutscht** — **tatsächlich hat Scherhant am 18.10. in Leverkusen in der 14. Minute getroffen und ist damit belegt fit.** *Ein eigener Beleg von gestern widerlegt eine Fundstelle von heute.*
2. ***Eine Hoffenheimer Meldung, nach der Torwart Oliver Baumann verletzt ausfällt und von Luca Philipp vertreten wird.*** **Verworfen:** *die Fundstelle gehört zu einem älteren Spiel, und die Suchzusammenfassung weist selbst darauf hin.* ***Entschieden wird es durch meinen Stand von gestern: Baumann stand am 18.10. gegen Gladbach in der Startelf.*** **Hätte ich das übernommen, wäre Partie 8 auf Basis eines Torwartausfalls verschoben worden, den es nicht gibt.**
3. **Eine `absolutfussball.com`-Überschrift „Köln-Trainer Kwasniok gibt Update zu verletztem Schmied".** **Verworfen** — *siehe die Prüfung oben; Kwasniok ist seit März 2026 nicht mehr Kölns Trainer.*
4. **Eine `deichstube.de`-Meldung „Rutschpartie in Mainz: Werder Bremen und Füllkrug rätseln über Standprobleme beim Last-Minute-Remis".** **Verworfen:** *Mainz – Werder ist meine Partie 5 und am 24.10. noch nicht gespielt; Werders Last-Minute-Remis der Vorwoche war das 2:2 gegen Paderborn zu Hause.* **Die Fundstelle betrifft eine frühere Saison.** ***Derselbe Fallentyp wie der `scfreiburg.com`-Treffer von gestern: richtige Paarung, falsche Zeit.***
5. **Eine `ligainsider.de`-Übersicht „Nach 7 Spieltagen: Hier drohen Gelbsperren!" mit Joe Scally, Joël Schmied und Christopher Trimmel.** **Verworfen:** *der Artikel ist vom 20.10.2025 und betrifft die Vorsaison.* ***Besonders tückisch, weil die Spieltagsnummer genau passt*** — **und weil Schmied darin vorkommt, also ein Name, der heute aus einem anderen Grund in den Meldungen steht.**
6. ***Zwei Verletztenlisten zu Union Berlin, die einander zu bestätigen schienen.*** **`oddspedia.com` nennt Juranović, N'Soki, Markgraf und Burke; `fotmob.com` nennt Juranović, Friedrich, Ilić, N'Soki und Markgraf.** **Verworfen:** *die Oddspedia-Seite trägt nach den Suchmetadaten ein Alter von rund 1.182 Tagen.* ***Die Übereinstimmung ist deshalb kein Beleg, sondern ihr Gegenteil: beide Seiten recyceln offenbar denselben alten Datenbestand.*** **Genau deshalb bleibt die Unioner Ausfallliste bei mir eine offene Lücke, obwohl heute zwei Listen dazu auffindbar waren.**
7. **Eine `tips.gg`-Vorschau, die für Leipzig Baumgartner, Guiu und Ouédraogo als verletzt und Zingerle als gesperrt führt.** **Nur als unbestätigter Hinweis geführt:** *eine einzelne Wett-Tipp-Seite, ohne Vereinsbestätigung, und ohne genannte Ersatzlösung.* ***Baumgartner wäre für Partie 4 relevant — deshalb schreibe ich ausdrücklich hin, dass ich ihn nicht als Ausfall verrechne.***
8. **Ein `hessenschau.de`-Ticker zur Frankfurter Personallage.** **Nicht verwendet:** *er nennt Adi Hütter als Trainer und ist damit erkennbar älter.*

---

## Offen benannte Restlücken

**Der 7. Spieltag beginnt in vier Tagen. Ich trenne weiter, was fehlt, von dem, was fehlen *muss*.**

***Strukturell noch nicht verfügbar (kein Mangel meiner Recherche):***
- **Keine Spieltags-Pressekonferenz zu einer der neun Partien** — die finden Donnerstag und Freitag statt.
- **Keine Aufstellung, kein Kaderaufgebot, keine voraussichtliche Elf zum 7. Spieltag.** ***Das ist der Grund, aus dem heute kein Tipp wechselt: acht meiner neun Schwellen verlangen genau dieses Beweismittel.***
- **Keine belastbare Gelbsperren-Übersicht nach dem 6. Spieltag.** *Gesucht und nicht gefunden: die `dfb.de`-Sperrenseite war zwar auf den 19.10.2026 datiert, enthielt aber nur Fälle der Frauen-Bundesliga; die auffindbaren Männer-Übersichten stammten aus 2023/24 und 2025/26.* **Zu Roten Karten in den Sonntagsspielen habe ich nichts gefunden — eine Nichtfundstelle, kein Beleg der Abwesenheit.**

***Echte Lücken:***
- ***NEU: Der Proxy-Zustand ist heute unbelegt***, weil die Statusabfrage von der Sitzungsberechtigung abgelehnt wurde (siehe oben).
- ***NEU: Wer Eintracht Frankfurt trainiert, kann ich nicht belegen.*** *Belegt ist nur, dass Dino Toppmöller im Januar 2026 entlassen wurde und Dennis Schmitt mit Alexander Meier interimistisch übernahm; ein Treffer nennt Adi Hütter und ist veraltet.* **Für Partie 7 habe ich deshalb bewusst keinen Frankfurter Trainernamen in die Begründung geschrieben.** *Der Routine-Prompt verlangt Trainerwechsel ausdrücklich — diese Lücke gehört also benannt.*
- **Demichelis' Zukunft bleibt die größte offene Frage.** *Heute belegt: er ist im Amt und reist nach Madrid. Nicht belegt: ob er den Spieltag erlebt.*
- **Karetsas' Ausfalldauer ist nicht amtlich** („Bandverletzung im Fuß", Mitte November nach Presseberichten).
- **Joël Schmieds Diagnose fehlt weiter** *(Bänderverdacht seit dem 17.10., drei Tage ohne Diagnose).*
- **Syllas Diagnose und Ausfalldauer fehlen** *(„nicht so tragisch", aber „ob wir es bis Köln schaffen, weiß ich nicht").* **Džekos Status ist nur aus einem Vorbericht bekannt, nicht vom Verein.**
- ***NEU: Lidbergs Diagnose fehlt*** *(Oberschenkelbeschwerden, Auswechslung, keine Aussage zur Dauer).* **Kühns Einsatz ist eine Blessin-Prognose, kein Kaderaufgebot.** **Zu Honorat, Itakura, Castrop und Leopold kein neuer Stand.**
- ***NEU: De Cats Ausfalldauer fehlt*** *(Knie-OP wahrscheinlich, Dauer laut `kicker` offen).* **Kabaks Zustand ist unbelegt.**
- **Neuers Rückkehrdatum und Musialas Rückkehr** bleiben offen wie gestern — ***zu Bayern gab es heute nichts Neues, und das ist erwartbar: die Pressekonferenz vor Arsenal ist am Dienstag.*** *Die auffindbaren Kompany-Zitate zu Neuer stammen aus der Zeit vor dem Leipzig-Spiel.*
- **Aches Rückkehr ist nur „teilintegriert im Training"**, kein Kaderaufgebot. **Rondics Rückkehr ohne Datum.**
- **Zu Paderborn habe ich heute keinen Personalstand gefunden** — *die auffindbaren Berichte stammen aus dem Trainingslager und sind rund 98 Tage alt.*
- **Claude-Maurices Status bei Augsburg ist widersprüchlich** *(`bundesliga.com` führt muskuläre Probleme zum 6. Spieltag, eine Spielvorschau führt ihn zum 24.10. als verletzt ohne Art der Verletzung).* **Banks ist dagegen solide belegt: Außenbandverletzung im rechten Knie, Vereinsmeldung vom 4.10., keine Operation, Reha begonnen.**
- **Keine Transfermeldung mit Spielrelevanz für den 7. Spieltag.** *Die einzige transfernahe Personalie des Tages betrifft Monacos Balogun, also einen Europapokalgegner.*
- **Direkte Vergleiche der letzten Duelle habe ich zu keiner der neun Partien belastbar erhoben.** ***Das ist jetzt den sechsten Lauf in Folge so, und die beiden verworfenen Fundstellen 1 und 4 von heute zeigen erneut, warum:*** *Treffer zu „Mainz – Werder" und „Leverkusen – Freiburg" führen zuverlässig auf frühere Saisons.* **Meine Tipps stehen daher auf Tabelle, Form, Personal und Belastung — nicht auf Historie.**

---

## Die Tipps zum 7. Spieltag

**Der Vortagsstand betraf denselben Spieltag, also ist jede Partie vergleichbar.** ***Kein Tipp ändert sich, alle neun bleiben.***

**Die vier Regeln, nach denen ich diesen Spieltag angelegt habe** — *unverändert gegenüber gestern:*

1. **Eine Torflaute wiegt schwerer als ein guter Tabellenplatz.**
2. **Ausfälle beim Gegner senken dessen Tore, sie erhöhen nicht automatisch meine.**
3. **Drei Tage nach einem weiten Auswärtsspiel in Europa gebe ich einen halben Tor-Abschlag**, bei einem Heimspiel in Europa keinen.
4. **Aufsteiger *und* den punktlosen Tabellenletzten tippe ich nach Spielweise und Personallage, nicht nach Tabellenplatz oder Heimrecht.**

**Für jede Partie nenne ich außerdem die Schwelle: die konkrete Information, die den Tipp bis zum Anpfiff ändern würde.**

---

### 1. VfB Stuttgart – Borussia Mönchengladbach
**Freitag, 23.10.2026, 20:30 Uhr, MHP Arena**
**Tipp: 2:0**
***unverändert — aber die Partie mit der heute am stärksten bewegten Faktenlage***

***Hier haben sich heute drei Dinge verändert, und sie ziehen nicht in dieselbe Richtung. Ich schreibe das offen hin, weil dieser Tipp als nächster fallen dürfte.***

**Für Stuttgart:** **Mittelstädt ist nach einer Fersenverletzung zurück im vollen Mannschaftstraining und kann in den Kader, Nartey und Al-Dakhil trainieren ebenfalls wieder mit.** ***Für meine Schwelle ist Al-Dakhil der entscheidende Name: er ist Innenverteidiger und kommt zurück*** — **ein Stuttgarter Innenverteidiger-Ausfall, der mich auf 1:1 gebracht hätte, ist damit nicht eingetreten, sondern das Gegenteil.** *Zagadou fehlt weiter, Tiago Tomás arbeitet individuell.*

**Für Gladbach, zum Schlechten:** **Blessin rechnet bei Kleindienst mit etwa zwei weiteren Spielen Ausfall, dieses eingeschlossen** — *gestern war das nur eine Fortschreibung des Muskelfaserrisses, heute ist es eine Trainerangabe mit Zeitraum.* **Und Lidberg, gegen Hoffenheim die einzige Spitze, musste mit Oberschenkelbeschwerden runter; ob eine Muskelverletzung vorliegt, ist offen.** ***Gladbach droht damit, auch noch den Stürmer zu verlieren, der das Tor vom Sonntag vorbereitet hat.***

***Für Gladbach, zum Guten — und das ist die Information, die diesem Tipp am nächsten kommt:*** **Nicolas Kühn hat eine Stunde im Mannschaftstraining absolviert und Steigerungsläufe gemacht. Blessin: „Da sind wir noch am abwägen, ob es dann für den Spieltag reicht … Aber spätestens nächste Woche sollte er zur Verfügung stehen."** **Die Aussage fiel vor dem Hoffenheim-Spiel, „spätestens nächste Woche" ist also diese Woche — und damit Stuttgart.** ***Meine Schwelle verlangt wörtlich „Kaderaufgebot oder Startelf, nicht Prognose".*** **Eine Trainererwartung ist eine Prognose, also ändere ich nicht** — *dieselbe Regel, mit der ich Musialas Rückkehr seit Tagen nicht verrechne, und ich wende sie hier gegen meinen eigenen Tipp an.* ***Aber ich sage voraus: wenn bis Freitag ein Gladbacher Kaderaufgebot mit Kühn erscheint, wechselt dieser Tipp auf 2:1.***

**Dass ich bei 2:0 bleibe, hat einen zweiten Grund, den ich gestern schon genannt habe: Stuttgart hat in sechs Spielen nur 8 Tore erzielt.** **Ein höherer Tipp wäre nicht gedeckt, auch wenn Gladbachs Lage ihn nahelegt.**

***Schwelle:*** *Wird Kleindiensts **oder** Kühns Einsatz belegt (Kaderaufgebot oder Startelf, **nicht** Prognose), gehe ich auf **2:1**. Kündigt Hoeneß nach dem Atlético-Spiel belegt eine Rotation an **oder** wird doch ein Stuttgarter Innenverteidiger-Ausfall gemeldet, gehe ich auf **1:1**. **Wird Lidbergs Ausfall bestätigt, bleibe ich bei 2:0 und gehe nicht höher — Regel 2.***

---

### 2. FC Augsburg – 1. FC Union Berlin
**Samstag, 24.10.2026, 15:30 Uhr, WWK Arena**
**Tipp: 2:1**
***unverändert***

***Die Partie, die gestern auf der dünnsten Personalgrundlage des Spieltags stand — und heute auf einer etwas besseren, aber nicht auf einer guten.***

**Der eine echte Fortschritt: es gibt erstmals seit Tagen einen datierten Unioner Beleg.** **Der `Berliner Kurier` schreibt, Lustrinelli werde in Augsburg voraussichtlich erneut Uduokhai und van den Bosch aufbieten, Querfeld bliebe auf der Bank.** ***Das bestätigt den Trainer aus einer heutigen Quelle und zeigt, dass Union in der Innenverteidigung keine Not hat.*** *Es ist eine voraussichtliche Aufstellung, also eine Prognose — für die Schwelle taugt sie nicht, für die Einschätzung schon.*

***Die Lücke bleibt aber, und heute ist sie besser dokumentiert als gestern:*** **ich habe zwei Unioner Verletztenlisten gefunden und beide verworfen, weil sie sich gegenseitig nur zu bestätigen schienen und erkennbar denselben alten Datenbestand wiedergeben** (Juranović, N'Soki, Markgraf in beiden; eine der Seiten ist rund 1.182 Tage alt). ***Zwei scheinbar übereinstimmende Quellen sind hier gerade kein Beleg*** — das ist der Lehrsatz des heutigen Laufs.

**Was den Tipp trägt, ist unverändert die Tordifferenz:** **Union hat mit 5 Toren in 6 Spielen die zweitschwächste Offensive und mit 17 Gegentoren die schwächste Abwehr der Liga.** **Augsburg ist zu Hause und hat mit 16 Toren die vierbeste Offensive, kassiert aber zuverlässig** — *das 3:4 in Elversberg nach 0:3 Rückstand bleibt die klarste Aussage über diese Mannschaft.* **Banks fehlt belegt (Außenbandverletzung im rechten Knie, Vereinsmeldung vom 4.10., keine OP, Reha läuft).** **Claude-Maurices Status ist widersprüchlich und wird von mir nicht als gesicherter Ausfall geführt.** **Keine der beiden Mannschaften spielt international** — *die einzige Partie, bei der das für beide Seiten gilt, und nach der Europapokalwoche ein echter Vorteil für beide.*

**Der Punkt für Union bleibt das 0:0 gegen Dortmund: ein Zu-Null gegen den Tabellenführer, und laut `Berliner Kurier` zwei Spiele hintereinander ohne Gegentor.**

***Schwelle:*** *Wird ein weiterer Augsburger Offensivausfall mit genannter Ersatzlösung gemeldet, gehe ich auf **1:1**. Wird Unions Null-zu-null-Formation gegen Dortmund in einem Vorbericht als Linie für Augsburg bestätigt (Tiefbau, fünf Verteidiger), gehe ich auf **1:0**. **Taucht erstmals eine datierte Unioner Ausfallliste mit einem Offensivausfall auf, gehe ich auf **2:0**.***

---

### 3. 1. FC Köln – FC Schalke 04
**Samstag, 24.10.2026, 15:30 Uhr, RheinEnergieSTADION**
**Tipp: 1:0**
***unverändert***

***Die Partie mit den beiden kaputtesten Offensiven des Spieltags, und heute ist bei beiden je eine Personalie dazugekommen — eine in jede Richtung.***

**Bei Köln zum Guten: Ache ist teilintegriert ins Mannschaftstraining eingestiegen.** ***Meine Schwelle für 2:0 verlangt ein Kaderaufgebot, nicht eine Trainingsmeldung*** — **„teilintegriert" ist ausdrücklich weniger als vollständiges Mannschaftstraining, und ich löse die Schwelle nicht aus.** *Schmied hat im Training verletzt gefehlt, seine Diagnose steht nach drei Tagen weiterhin aus.* **Unverändert aus: Dallinga (Kreuzbandriss), Rondic (Oberschenkel, ohne Datum), Skhiri (bis mindestens Jahresende), van den Berg, Hübers.** **Der Verein hat keinen Ersatzstürmer verpflichtet und verschiebt das auf Januar; vorn sollen Waldschmidt und Bülter spielen.** **Köln hat in Frankfurt nicht getroffen.**

**Bei Schalke zum Schlechten, und zwar deutlich: zu Sylla (fraglich, Muslić: „ob wir es bis Köln schaffen, weiß ich nicht") und Ljubičić (Knieprobleme) kommt heute Edin Džeko.** **Er musste gegen Mainz nach einem Zusammenprall mit einer Platzwunde ausgewechselt werden und fällt laut Vorbericht womöglich aus** — *eine Vereinsbestätigung dazu habe ich nicht, ich führe es als Vorbericht.* **Dazu die 5 Saisontore und der aus zwei Quellen belegte Befund, dass Schalke in dieser Saison zu Hause ohne eigenes Tor ist.**

***Und genau hier wende ich Regel 2 gegen meine eigene Versuchung an:*** **Schalke verliert möglicherweise seinen dritten Angreifer, aber das macht Kölns Sturm nicht besser — Köln hat keinen gesunden Mittelstürmer.** **Drei fehlende Schalker Offensivkräfte rechne ich deshalb nicht in Kölner Tore um.** *Genau dieser Fehler hat mich am 15.10. bei Frankfurt – Köln zwei Tore gekostet.* **Es bleibt beim Heimvorteil und dem einen Tor.** *Dass Schalkes Nullnummern-Serie ein Heimbefund ist und hier auswärts gespielt wird, schwächt mein Argument leicht — ich schreibe das weiter hin.*

***Schwelle:*** *Wird Aches **oder** Rondics Rückkehr für diesen Spieltag belegt (Kaderaufgebot, nicht Trainings- oder Prognosemeldung), gehe ich auf **2:0**. Wird Syllas Einsatz belegt **oder** fällt über Schmied hinaus ein weiterer Kölner Innenverteidiger aus, gehe ich auf **1:1**. **Džekos bestätigter Ausfall ändert nach Regel 2 nichts.***

---

### 4. RB Leipzig – SV 07 Elversberg
**Samstag, 24.10.2026, 15:30 Uhr, Red Bull Arena**
**Tipp: 2:1**
***unverändert — und weiterhin mein unsicherster Tipp***

**Die Trainerfrage ist heute einen Schritt klarer geworden, und zwar in die Richtung, die meine Schwelle nicht auslöst.** **Demichelis hat sich am Montag in einer virtuellen Medienrunde zum Real-Spiel geäußert — einen Tag vor seiner eigentlichen Pressekonferenz am Dienstag — und inhaltlich über Ballbesitz und Reals Umschaltspiel gesprochen.** ***Damit ist belegt: Leipzig geht mit ihm ins Bernabéu, und bis heute Abend ist keine Entscheidung gefallen.*** **Die Kritik läuft weiter; die Nagelsmann-Spekulation bleibt unbestätigt und laut dem berichtenden Medium ohne konkrete Vereinbarung.**

**Elversberg hat Augsburg 4:3 geschlagen, nach 28 Minuten 3:0 geführt (Petkov, Günther, Rohr) und steht mit 10 Punkten vor Augsburg und über Leipzig.** **Der Aufsteiger spielt nicht international.** **Nach dem Stand vom 15.10. fehlen Onyeka, Seifert und Zimmerschied; Gyamerah ist einsatzbereit.** *Einen neueren Elversberger Personalstand habe ich auch heute nicht gefunden — vierter Lauf ohne Fortschritt an diesem Punkt.*

***Zu Leipzigs Personal muss ich eine Einschränkung machen, die gegen meinen eigenen Tipp arbeitet:*** **eine Wett-Vorschau führt Baumgartner, Guiu und Ouédraogo als verletzt und Zingerle als gesperrt.** **Ich verrechne das nicht** — *eine einzelne Wett-Tipp-Seite ohne Vereinsbestätigung und ohne genannte Ersatzlösung reicht nach meiner Regel nicht.* ***Aber Baumgartner wäre für diesen Tipp erheblich, und ich halte ausdrücklich fest, dass ich hier auf einer Quelle verzichte, die mich näher an ein Remis gebracht hätte.***

**Ich bleibe bei einem knappen Heimsieg: 16 Tore in 6 Spielen sind die zweitbeste Offensive der Liga, und eine Mannschaft unter diesem Druck will zu Hause gegen einen Aufsteiger antworten.** ***Die Belastung ist die zweitschwerste des Spieltags: Mittwoch 21:00 im Bernabéu, dann Samstag 15:30 — drei Tage nach einer weiten Auswärtsreise, also Abschlag nach Regel 3.*** **Es bleibt der Tipp, bei dem ich mir am wenigsten sicher bin, und der Grund ist unverändert: Madrid-Reise, offene Trainerfrage und ein formstarker Aufsteiger sind genau die Lage, in der Heimsiege ausbleiben.**

***Schwelle:*** *Wird Demichelis entlassen oder freigestellt, gehe ich auf **1:1**. Kündigt er nach Madrid belegt eine Rotation an **oder** wird ein Leipziger Offensivausfall mit genannter Ersatzlösung **vom Verein** gemeldet, ebenfalls **1:1**. Wird ein Elversberger Innenverteidiger-Ausfall gemeldet, gehe ich auf **3:1**.*

---

### 5. 1. FSV Mainz 05 – SV Werder Bremen
**Samstag, 24.10.2026, 15:30 Uhr, Mewa Arena**
**Tipp: 1:1**
***unverändert***

**Die Grundlage von gestern hält, und eine strittige Angabe ist heute entschieden.** **Mainz ist auswärts makellos und zu Hause sieglos:** **`mainz05.de` schrieb nach dem 1:0 in Gelsenkirchen vom dritten Auswärtssieg aus drei Auswärtsspielen; zusammen mit 10 Punkten aus 6 Spielen bleibt für drei Heimspiele genau 1 Punkt.** *Das ist eine Rechnung, keine Fundstelle — ich kennzeichne sie weiter als solche.*

***Entschieden ist heute Kohrs Ausfalldauer, die ich seit Tagen als „strittig" geführt habe.*** **`bundesliga.com` nennt eine Syndesmoseverletzung, eine Spielvorschau nennt eine Rückkehr Anfang Januar 2027.** **Eine Syndesmoseverletzung passt zu Januar und nicht zu „Ende Oktober"** — ***ich führe die kurze Variante ab heute als überholt, und damit ist meine 2:1-Schwelle über Kohrs Rückkehr praktisch erledigt.*** *Weiter aus bei Mainz: Zentner (Handverletzung), dazu nach Vorberichten Widmer, Martel, Nebel und Silas — letztere aus einer Vorschau, deren Datierung ich nicht prüfen konnte, deshalb ohne Gewicht.*

**Bei Werder gibt es zu Füllkrug keine Verletzungsmeldung.** ***Das ist für meine 2:0-Schwelle die entscheidende Nichtmeldung:*** **er und Grüll hatten vor rund einer Woche dosiert trainiert, und der Verein nannte dafür ausdrücklich Belastungssteuerung, keine Beschwerden.** **Werder bleibt die Mannschaft, die man nicht abschreiben kann: gegen Paderborn 0:2 zurück, dann Füllkrugs Doppelpack (59., 65. per Elfmeter) — als erste Bundesligamannschaft dreimal in Folge ein Punktgewinn nach Zwei-Tore-Rückstand, sechs Punkte nach Rückstand sind Ligabestwert.** **Werder spielt nicht international.**

**Ein Heimspiel, in dem die Heimmannschaft aus drei Versuchen einen Punkt geholt hat, gegen eine Auswärtsmannschaft, die dreimal in Folge einen Zwei-Tore-Rückstand aufgeholt hat** — ***1:1 ist hier kein Mittelweg, sondern das Ergebnis beider Befunde.***

***Schwelle:*** *Wird in einem Vorbericht die Heimschwäche ausdrücklich als überwunden beschrieben (etwa durch eine Systemumstellung), gehe ich auf **2:1**. Fällt Füllkrug aus (Vereinsmeldung, nicht Belastungssteuerung), gehe ich auf **2:0**. **Die Kohr-Schwelle entfällt faktisch — eine Rückkehr im Januar berührt diesen Spieltag nicht.***

---

### 6. SC Paderborn 07 – Hamburger SV
**Samstag, 24.10.2026, 15:30 Uhr, Home Deluxe Arena**
**Tipp: 1:1**
***unverändert — die Partie mit der dünnsten neuen Faktenlage***

***Hier ist heute am wenigsten passiert, und das sage ich offen: zu Paderborn habe ich keinen einzigen aktuellen Personalstand gefunden.*** *Die auffindbaren Ausfallberichte stammen aus dem Trainingslager und sind rund 98 Tage alt; ich verwende sie nicht.* **Es bleibt beim Stand der Vortage: Gayret, Klaas und Baur fehlen, bei Awortwie-Grant zeichnet sich ein Comeback ab, Bilbija ist zu Derby County gewechselt.**

***Regel 4 ausdrücklich angewandt.*** **Paderborn steht mit 5 Punkten auf Platz 16, hat aber bei Werder 2:0 geführt (Marino 18., Tigges 30.) und stand in der Nachspielzeit durch Philippe am Pfosten vor dem Auswärtssieg; Torwart Noll hielt mehrfach stark.** **Kettemann beschreibt seine Mannschaft als „Gruppe junger, unerfahrener Bundesliga-Menschen", der es an Torgefahr fehlt** — **5 Tore in 6 Spielen bestätigen das**, *aber zwei davon fielen zuletzt auswärts in Bremen.*

**Beim HSV ist der Befund von gestern bestätigt und der Trainername jetzt belegt: Merlin Polzin sucht laut `sport1` neue Lösungen für die Offensive.** **Grönbaek und Daka fehlen mit Muskelblessuren, Kapitän Remberg mit Kreuzbandriss.** *Sambi Lokonga hatte ich gestern aus dem Spielbericht zum Stuttgart-Spiel aufgenommen; heute ist er in keiner Meldung aufgetaucht — ich führe ihn weiter, aber ohne neuen Beleg.* ***Die Zahlen hinter der Dreier-Serie bleiben dünn: 6 Tore in 6 Spielen, 15 Gegentore, Torverhältnis −9 bei 9 Punkten.*** **Der 1:0-Sieg gegen Stuttgart fiel in der 88. Minute durch Muheims Schuss aus 25 Metern.** **Keine der beiden Mannschaften spielt international.**

**Eine Heimmannschaft, die gerade gezeigt hat, dass sie führen kann, gegen eine Auswärtsmannschaft, die mit 6 Saisontoren drei Spiele hintereinander gewonnen hat und im Zentrum Ausfälle hat** — **1:1.**

***Schwelle:*** *Wird eine HSV-Offensivverstärkung belegt (Daka oder Grönbaek im Kaderaufgebot), gehe ich auf **1:2**. Fällt bei Paderborn Tigges **oder** Marino aus, ebenfalls **1:2**. Wird Awortwie-Grants Rückkehr belegt, gehe ich auf **2:1**.*

---

### 7. Borussia Dortmund – Eintracht Frankfurt
**Samstag, 24.10.2026, 18:30 Uhr, Signal Iduna Park**
**Tipp: 2:0**
***unverändert — und die Schwelle entscheidet sich morgen Abend***

**Der heute nominierte Kader für Baku beantwortet zwei meiner drei Schwellenfragen mit Nein.** **Der BVB hat 24 Spieler nominiert; genannt werden unter anderem Kobel, Anton, Schlotterbeck, Bensebaini, Bellingham, Nmecha, Guirassy und Svensson.** ***Guirassy ist im Kader — der Teil meiner Schwelle, der auf seinen Ausfall zielt, ist damit erledigt.*** ***Schlotterbeck, Anton und Bensebaini sind im Kader — es gibt keinen Dortmunder Innenverteidiger-Ausfall.*** **Und Kovač hat auf der Pressekonferenz keine Rotation angekündigt, sondern das Gegenteil signalisiert: Dortmund sei „klarer Favorit" und müsse das Spiel gewinnen.** *Sein Vertrag läuft bis 2029; eine Entlassung vor dem Spieltag bleibt unwahrscheinlich.*

**Karetsas fehlt im Kader, und seine Verletzung ist heute präzisiert: Ricken spricht von einer „Bandverletzung im Fuß", die `Ruhr Nachrichten` erwarten eine Rückkehr nicht vor Mitte November.** ***Am Tipp ändert das weiterhin nichts*** — **er kam gegen Union als Einwechselspieler, war also nicht gesetzt, und meine Schwelle verlangt einen Innenverteidiger oder Guirassy.** *Ihn zum Anlass einer Änderung zu machen, wäre die Überreaktion, die mir Regel 2 verbietet.*

**Dortmund ist drei Pflichtspiele ohne eigenes Tor** (Werder, Bodø, Union), **steht aber mit 14 Punkten und 4 Gegentoren an der Spitze.** **Guirassy ist selbst drei Spiele ohne Treffer und stand in Bodø nicht in der Startelf.** **Nwaneri ist nach der zurückgenommenen Roten Karte spielberechtigt.** **Belastung: Dienstag 18:45 in Baku (20:45 Ortszeit), die weiteste Reise des Spieltags — aber mit vier Tagen Abstand und einem Gegner, gegen den rotiert werden kann.**

**Frankfurt ist der Gegner, gegen den eine Torflaute am ehesten endet: 16 Gegentore in 6 Spielen sind die zweitschwächste Abwehr der Liga.** **Der 1:0-Sieg gegen Köln war Frankfurts erster Heimsieg seit März — auswärts steht die Mannschaft weiter ohne Ausweis.** ***Was ich zu Frankfurt nicht sagen kann, sage ich auch nicht:*** **wer die Eintracht aktuell trainiert, konnte ich heute nicht belegen** (Toppmöller im Januar 2026 entlassen, Schmitt und Meier interimistisch; ein Treffer nennt Hütter und ist veraltet). **Ein Frankfurter Ausfall ist nur unzuverlässig auffindbar (Ngankam im Aufbautraining, undatierte Sammelseite) und wird von mir nicht verrechnet.**

***Die eigentliche Schwelle liegt morgen Abend:*** **bleibt Dortmund auch in Baku ohne Tor, sind es vier Spiele, und dann gehe ich auf 1:0.** *Das ist die Information, die diesen Tipp mit der höchsten Wahrscheinlichkeit noch bewegt — vor jedem Personalbericht.*

***Schwelle:*** *Bleibt Dortmund in Aserbaidschan ohne Tor, gehe ich auf **1:0**. Wird ein Dortmunder Innenverteidiger-Ausfall mit genannter Ersatzlösung gemeldet **oder** fällt Guirassy aus, gehe ich auf **1:1**. Wird Kovač entlassen, ebenfalls **1:1**. Wird bei Frankfurt ein Innenverteidiger-Ausfall **belegt** gemeldet, gehe ich auf **3:0**.*

---

### 8. TSG Hoffenheim – Bayer 04 Leverkusen
**Sonntag, 25.10.2026, 15:30 Uhr (MEZ), SNP Arena**
**Tipp: 2:2**
***unverändert — aber mit einem neuen Gegenargument, das ich nicht verschweige***

**Die beiden Auslöser meiner Änderung von gestern halten unverändert.** **Hoffenheim hat in Gladbach 2:1 gewonnen (Conté 11., Prass 54.) und ist auf Platz 14 geklettert; Leverkusen muss Donnerstag 18:45 nach Kreta und dann Sonntag 15:30 schon wieder auswärts antreten, während Hoffenheim Lyon zu Hause empfängt.** ***Der Abschlag nach Regel 3 bleibt also voll bestehen.***

***Was heute dagegen spricht, und es ist nicht wenig:*** **Hoffenheims Personallage hat sich verschlechtert.** **Nathan De Cat hat sich am linken Knie verletzt, eine Operation gilt als wahrscheinlich, und er fällt voraussichtlich länger aus; eine Ausfalldauer steht laut `kicker` nicht fest.** **Ozan Kabak gilt nach seiner Auswechslung gegen Beşiktaş als Sorgenfall ohne offizielle Diagnose** — *er stand auch gegen Gladbach nicht in der Startelf.* **Ilzer sprach von „ein paar angeschlagenen" Spielern, ohne Namen zu nennen. Hajdari fehlt weiter.** ***Warum ich den Tipp trotzdem halte:*** **keiner dieser Spieler stand in der Startelf, die am Sonntag in Gladbach gewonnen hat** (Baumann; Coufal, Hranáč, Machida, Rots; Avdullahu, Conté, Prass; Lemperle, Asllani, Hložek). **Es sind Kaderverluste, keine Stammelfverluste** — *und meine vier Schwellen zielen alle auf andere Ereignisse.*

***Ausdrücklich verworfen und für diesen Tipp entscheidend:*** **eine Fundstelle, nach der Hoffenheims Torwart Baumann verletzt ausfällt und von Luca Philipp vertreten wird.** **Sie gehört zu einem älteren Spiel — Baumann stand am Sonntag gegen Gladbach im Tor.** *Hätte ich sie übernommen, hätte ich diesen Tipp auf einem Torwartausfall verschoben, den es nicht gibt.*

**Bei Leverkusen ist Schick fit — die Sorge um ihn nach dem 4:0 gegen Lech Posen hat er selbst ausgeräumt; er kam dort in der 18. Minute für den verletzten Terrier, traf zweimal per Elfmeter und ging in der 76. Minute runter.** **Er hat in allen sechs Bundesligaspielen getroffen.** ***Meine 1:1-Schwelle zielt auf seinen Ausfall oder seine Schonung — eingetreten ist das Gegenteil.*** **Terrier fällt mit Oberschenkelverletzung bis Dezember aus, dazu Ben Seghir, Doué, Eichhorn und Kofane.** **Leverkusen ist Vierter mit 13 Punkten und hat am Sonntag Freiburg geschlagen.**

**Dass Bernardo in der Hoffenheimer Startelf gegen Gladbach fehlte, bleibt mein Indizienschluss für eine abgesessene Einspielsperre — kein Beleg der Sperrdauer.**

***Schwelle:*** *Wird Schicks Ausfall oder Schonung belegt, gehe ich auf **1:1**. Kündigt Leverkusen nach Kreta belegt eine Rotation an, gehe ich auf **2:1** (für Hoffenheim). Verliert Hoffenheim am Donnerstag gegen Lyon hoch (drei Tore oder mehr), gehe ich zurück auf **1:2**. Wird Bernardos Sperre als länger als ein Spiel belegt, gehe ich auf **1:2**. **Neu: fällt über De Cat und Kabak hinaus ein Spieler der Gladbach-Startelf aus, gehe ich auf **1:2**.***

---

### 9. SC Freiburg – FC Bayern München
**Sonntag, 25.10.2026, 17:30 Uhr (MEZ), Europa-Park Stadion**
**Tipp: 1:2**
***unverändert***

***Zu Bayern gibt es heute nichts Neues, und das ist erwartbar statt lückenhaft:*** **die Pressekonferenz vor dem Arsenal-Spiel am Mittwoch findet am Dienstag statt.** **Die heute auffindbaren Kompany-Zitate zu Neuer stammen aus der Zeit vor dem Leipzig-Spiel und sind damit älter als mein Stand von gestern** — *ich verwende sie nicht.* **Es bleibt bei Eberls Angaben vom 18.10.: „etwas Flüssigkeit im Fuß" bei Neuer, kein Rückkehrdatum, Urbig als Vertreter; Musiala fehlt gegen Arsenal, Eberls Oktober-Erwartung ist eine Prognose und löst meine 1:3-Schwelle nicht aus.** **Olise ist für das Arsenal-Spiel gesperrt (zwei Gelbe gegen Viking FK) und geht ausgeruht in den Sonntag.** **Bayern hat Leipzig 6:1 geschlagen, steht bei 22:5 Toren und ist in sechs Spielen unbesiegt.**

***Bei Freiburg habe ich heute den gefährlichsten Treffer des Tages abgefangen.*** **Eine Kadermeldung führte Scherhant und Beste als kurzfristige Ausfälle mit Muskelproblemen.** **Sie betrifft das Conference-League-Spiel gegen Jablonec, also eine frühere Woche** — ***und sie wird durch meinen eigenen Stand von gestern widerlegt: Scherhant hat am Sonntag in Leverkusen in der 14. Minute getroffen.*** **Hätte ich ihn als Ausfall übernommen, wäre dieser Tipp auf einer falschen Grundlage nach unten gerutscht.**

**Freiburg ist Dritter mit 13 Punkten und 15:6 Toren; die Serie ist nach dem 1:2 in Leverkusen beendet, aber die Mannschaft hat dort geführt und bis zur 76. Minute gestanden.** ***Keine meiner beiden Schwellen von gestern hat gegriffen*** — weder eine deutliche Niederlage noch ein Sieg. **Suzukis Gelb-Rot-Sperre ist abgesessen, Muslija fehlt mit Kreuzbandriss.**

***Neu und ein kleiner Punkt für Freiburg:*** **Monacos wertvollster Spieler Folarin Balogun ist nicht für den Conference-League-Kader nominiert (gescheiterter Transfer am Deadline Day) und fehlt am Donnerstag.** *Freiburgs Europapokalaufgabe wird damit eher leichter, was die Belastung vor Sonntag etwas senkt — die Reise nach Monaco bleibt mit rund 550 Kilometern eine mittlere, für die ich keinen vollen Abschlag nach Regel 3 gebe.*

**Ich bleibe bei Bayern mit einem Tor Unterschied: der Offensivunterschied ist in Zahlen eindeutig (22:5 gegen 15:6), Freiburgs Heimstärke und die drei Tage nach Monaco sprechen gegen eine klare Angelegenheit.**

***Schwelle:*** *Wird Musialas Rückkehr belegt gemeldet (Kaderaufgebot, nicht Prognose), gehe ich auf **1:3**. Wird Kompanys Rotation nach dem Arsenal-Spiel belegt angekündigt, gehe ich auf **1:1**. Verliert Freiburg am Donnerstag in Monaco hoch und wird eine Freiburger Rotation gemeldet, gehe ich auf **0:2**. **Neuers Rückkehr ändert nichts.***

---

## Verteilung und Selbstkontrolle

| Tipp-Typ | Anzahl | Partien |
|---|---|---|
| **Heimsieg** | **5** | 1 (2:0), 2 (2:1), 3 (1:0), 4 (2:1), 7 (2:0) |
| **Remis** | **3** | 5 (1:1), 6 (1:1), 8 (2:2) |
| **Auswärtssieg** | **1** | 9 (1:2) |

**Gesamttore: 23 in 9 Partien, 2,56 je Spiel** — *unverändert gegenüber gestern.*

***Vier Dinge, die ich an diesem Lauf kritisch sehe:***
1. ***Null Änderungen bei neun Tipps ist ein Ergebnis, das Rechtfertigung braucht, und ich liefere sie nachprüfbar:*** **acht meiner neun Schwellen verlangen ausdrücklich ein Kaderaufgebot, eine Startelf oder eine belegte Rotationsankündigung.** **Keines dieser Dokumente existiert am Montag vor einem Spieltag, der Freitag beginnt.** *Die neunte Schwelle (Partie 7) hängt an Dortmunds Ergebnis in Baku und entscheidet sich morgen.* ***Hätte ich heute geändert, hätte ich es gegen meine eigenen Regeln getan — und zwar auf Basis von Prognosen und undatierten Sammelseiten.***
2. **Fünf Heimsiege bleiben viel**, *und die Abrechnung des 6. Spieltags hat mir dreimal die schwächere Heimmannschaft als Fehler nachgewiesen.* **Das Muster steht weiter unkorrigiert, weil heute keine Information kam, die eine Korrektur begründet hätte.** *Ich notiere es zum dritten Mal.*
3. ***Partie 1 ist der Tipp, der als nächster fällt.*** **Kühns Rückkehr ist von seinem Trainer für genau diese Woche erwartet; fehlt sie nur noch am Kaderaufgebot, wechselt der Tipp auf 2:1.** *Dass ich heute nicht geändert habe, ist Regelanwendung — nicht Überzeugung.*
4. ***Die Qualität meiner Quellen war heute schlechter als an allen Vortagen, und das ist das eigentliche Ergebnis des Laufs.*** **Sechs verworfene Fundstellen, davon zwei, die direkt zu falschen Tippänderungen geführt hätten** (Scherhant als Ausfall, Baumann als Ausfall), **und eine, die einen Trainernamen falsch zugeordnet hätte** (Kwasniok statt Wagner). ***In allen drei Fällen hat mein eigener Vortagsstand die Fundstelle widerlegt*** — **das Archiv ist damit heute die verlässlichste Quelle des Laufs gewesen, und das ist kein gutes Zeichen für die Quellenlage.**

---

## Quellen

**Alle Angaben dieses Laufs stammen aus `WebSearch`-Ergebnislisten (Titel und Zusammenfassungen), nicht aus Volltexten** — *die vier im Routine-Prompt genannten Leitquellen sind durch die Egress-Policy gesperrt, `WebFetch` scheitert an der Namensauflösung.*

**Für Dortmund und Baku:** `1news.az` und `operativmm.az` (24-Mann-Kader, mit Verweis auf die Vereinsseite), `dazn.com`, `onefootball.com` (Liveticker und Pressekonferenz), `sports.yahoo.com`, `ruhrnachrichten.de` (Karetsas, via Zusammenfassung), `neunzigplus.de`, `fussballdaten.de`, `4-4-2.com`, `news.de`.
**Für Stuttgart:** `vfb.de` (Pressekonferenzseite), `magazin.comunio.de`, `zvw.de`, `t-online.de`, `ligaportal.at`, `bulinews.com`, `90min.de`.
**Für Gladbach:** `magazin.comunio.de` (Kleindienst, Lidberg), `gladbachlive.de` und `sport1.de` (Kühn, Blessin-Zitat), `gladbachtotal.de`, `bmg-news.de`, `sportschau.de`, `neunzigplus.de`.
**Für Leipzig:** EFE über `unitel.bo`, `laestrella.com.pa` und `latingoles.com` (Medienrunde vom 19.10.), `sport.de`, `sports.yahoo.com`.
**Für Köln und Schalke:** `zdfheute.de` (Trainerfrage, entscheidend), `msn.com` (Ache im Training), `absolutfussball.com` (Sylla-Vereinsmeldung), `ms-aktuell.de`, `baykusen.de`, `fussballtransfers.com`, `come-on-fc.com`, `magazin.comunio.de`, `ligainsider.de` (nur Džeko-Hinweis).
**Für Hoffenheim und Leverkusen:** `hz.de` und `fussballdaten.de` (De Cat), `ligainsider.de` (Kabak, Ilzer), `sportschau.de`, `t-online.de`, `beinsports.com` (Schick), `de.uefa.com`.
**Für Freiburg und Monaco:** `scfreiburg.com` (Auswärtsgegner der Ligaphase), `sportschau.de`, `wochenblatt-reporter.de`, `de.uefa.com`.
**Für Mainz, Werder, Paderborn, HSV, Augsburg, Union:** `bundesliga.com` (Banks-Vereinsmeldung, Ausfallvorschauen), `werder.de`, `deichstube.de` (nur als verworfene Fundstelle), `rheinpfalz.de`, `sport1.de` (Polzin), `footy.de`, `nw.de` (verworfen, 98 Tage alt), `berliner-kurier.de` (Union, Lustrinelli), `ligainsider.de`, `tipico.de`.

***Nicht erreichbar und deshalb nicht verwendet:*** **`kicker.de`, `bundesliga.com`, `transfermarkt.de` und `weltfussball.de` im Volltext** *(Namensauflösung scheitert; Inhalte dieser Seiten erscheinen hier nur, soweit sie in Suchergebnis-Zusammenfassungen auftauchen).*
***Heute zusätzlich nicht verfügbar:*** **die Proxy-Statusabfrage** *(von der Sitzungsberechtigung abgelehnt).*
