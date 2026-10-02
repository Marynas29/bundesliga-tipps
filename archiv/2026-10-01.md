# Bundesliga-Tipps – 5. Spieltag 2026/27 (Stand: 01.10.2026)

**Ansetzung:** Freitag, 09.10. bis Sonntag, 11.10.2026. Der Vortagsstand (30.09.) betraf denselben Spieltag – **alle neun Tipps sind vergleichbar.**

**Elfter Tag der Länderspielpause (21.09.–06.10.2026).** Bis zum Anpfiff sind es 8 Tage. Heute Abend spielt die Nationalmannschaft in München gegen Serbien (20:45, Allianz Arena), am Sonntag in Thessaloniki gegen Griechenland.

**Heute ändert sich kein einziger Tipp – erstmals in diesem Repo.** Das ist ein Ergebnis, das ich rechtfertigen muss, und ich tue es unten in einem eigenen Abschnitt. In Kürze: **Die beiden Änderungen von gestern sind heute besser belegt als bei ihrer Vornahme** – Schlotterbecks Verletzung ist inzwischen DFB-bestätigt und wird von einer Fundstelle als **Riss** geführt, und die drei HSV-Offensivausfälle haben sich einzeln bestätigt. **Bei den übrigen sieben Partien ist nichts hinzugekommen, was einen Tipp trägt** – im wichtigsten Fall, Köln – Gladbach, weil **die zwei neuen Fundstellen in entgegengesetzte Richtungen zeigen und sich aufheben.**

**Der eigentliche Gewinn des Laufs liegt woanders: Dieses Repo führt ab heute für alle 18 Vereine einen Trainer.** Die letzte Lücke – Augsburg – ist über die Vereinsseite geschlossen, und damit fällt eine Verwerfung von gestern. Dazu kommt **ein Datierungswerkzeug, das ich vorher nicht hatte** (siehe „Methodisch neu"), **die Auflösung der Vereinszuordnung von Lerma und Ryerson**, **das Paderborner Testspielergebnis** und **sechs ausdrücklich verworfene Fundstellen**, darunter zwei, die zu ganz anderen Spielen gehören.

## Hinweis zur Quellenlage (bitte zuerst lesen)

Die vorgesehenen Fachquellen sind aus dieser Umgebung **weiterhin nicht abrufbar** – heute der **fünfundzwanzigste Lauf in Folge** mit demselben Befund. `kicker.de`, `bundesliga.com`, `transfermarkt.de`, `weltfussball.de`, `sportschau.de`, `ligainsider.de` und `fc.de` wurden um 21:16 UTC einzeln per curl geprüft und liefern alle den Rückgabewert `000` (kein Verbindungsaufbau). Die Proxy-Statusabfrage nennt für exakt diese Hosts und exakt diesen Zeitpunkt `connect_rejected / gateway answered 403 to CONNECT (policy denial or upstream failure)`. Ein **WebFetch auf `kicker.de/bundesliga/spieltag/2026-27/5`** ergab `EGRESS_BLOCKED`. Der Befund ist damit wie an den Vortagen über **zwei unabhängige Wege desselben Laufs** geprüft.

**Das ist eine Einstellung der Umgebung, keine Störung.** Die Netzwerkfreigabe dieser Sitzung verweigert die Hosts. Wer das ändern will, findet es in den Einstellungen der Cloud-Umgebung unter **Network access** (Menü der Umgebung in der Titelzeile der Sitzung, dann **Edit**) – entweder über eine weitere Zugriffsstufe oder durch Aufnahme dieser Hosts in die erlaubten Domains. Die Zugriffsstufen sind unter <https://code.claude.com/docs/en/claude-code-on-the-web> beschrieben. **Solange das so bleibt, gilt für dieses Repo: Alle Angaben unten stammen aus Suchergebnis-Zusammenfassungen, nicht von den Primärseiten.** Das ist der Grund, warum die **Datierung und die Vereinszuordnung** einer Meldung hier die Hauptarbeit sind und nicht das Finden.

### Methodisch neu: der Bundestrainer als Datumsstempel

Heute habe ich ein Werkzeug gewonnen, das diesem Repo bisher gefehlt hat. **Der Bundestrainer heißt Jürgen Klopp** – er wird in der heutigen Schlotterbeck-Berichterstattung wörtlich zitiert („Nico ist einfach umgeknickt – ohne Gegner- oder Mitspielereinwirkung"). **Jede Fundstelle, die Julian Nagelsmann als Bundestrainer führt, liegt damit vor Klopps Amtszeit und ist alt**, auch wenn sie undatiert erscheint und thematisch passt.

**Das hat heute sofort gegriffen und eine Tippänderung verhindert.** Eine Fundstelle nennt Chris Führich und Angelo Stiller als Stuttgarter Ausfälle; eine zweite, die das entkräften würde, berichtet von ihrer **Nachnominierung in den DFB-Kader** – und nennt dabei **Nagelsmann** als Bundestrainer. **Also ist auch die Entkräftung alt, und ich weiß über Führich und Stiller weiterhin nichts Belastbares.** Genau das hat mich davon abgehalten, Paderborn – Stuttgart auf eine Ausfallliste zu stellen, die ich nicht datieren kann (unten im Detail).

### Spielplan: heute erstmals vollständig und fehlerfrei bestätigt

**Die Spieltagszusammenfassung liefert heute alle neun Partien mit korrekter Tageszuordnung** – zum ersten Mal. **An den beiden Vortagen hatte dieselbe Abfrage sieben der neun Partien dem Freitag zugeordnet**, darunter fünf 15:30-Spiele, was es nicht gibt, und Paderborn – Stuttgart auf 18:30 gelegt. **Dieser Fehler ist heute weg.** Die Zuordnung deckt sich in allen neun Partien mit meinem Stand von gestern: ein Freitagsspiel, sechs am Samstag (fünf um 15:30, Leipzig um 18:30), zwei am Sonntag.

Zusätzlich einzeln bestätigt: **Dortmund – Werder** (Fr, 09.10., 20:30, Signal Iduna Park), **Union – Elversberg** (Sa, 10.10., 15:30, Alte Försterei – eine Fundstelle nennt `13:30 UTC`, was exakt 15:30 MESZ entspricht), **Mainz – Leverkusen** (Sa, 10.10., 15:30, MEWA Arena), **Hoffenheim – HSV** (Sa, 10.10., 15:30), **Leipzig – Frankfurt** (Sa, 10.10., 18:30), **Köln – Gladbach** (So, 11.10., 15:30) und **Freiburg – Schalke** (So, 11.10., 17:30). **Der Spielplan steht, und der Vorbehalt zum Kölner Termin bleibt zurückgenommen.**

*Zur Länderspielpause selbst:* Sie dauert **18 Tage ohne Bundesligaspiel**, und der Grund ist eine **Änderung des FIFA-Rahmenkalenders** – die Nationalspieler reisen nicht mehr zweimal für je zwei Spiele, sondern einmal für bis zu vier.

## Korrekturen am Vortagsstand

### 1. Manuel Baum ist Augsburgs Trainer – meine gestrige Verwerfung war im Ergebnis falsch

Gestern stand hier: „**Ich trage keinen Augsburger Trainernamen ein** – und halte fest, dass dieses Repo für Augsburg noch nie einen Trainer geführt hat." Verworfen hatte ich die Angabe „Sandro Wagner bis 01.12.2025, dann Interimstrainer Manuel Baum" mit der Begründung, sie betreffe die Saison 2025/26.

**Die Begründung war richtig, die Schlussfolgerung falsch.** Baum war damals Interimstrainer – **und wurde anschließend dauerhaft bestätigt.** **Manuel Baum ist Cheftrainer des FC Augsburg, Vertrag verlängert bis zum 30.06.2028.** Belegt über **`fcaugsburg.de` – die Vereinsseite selbst** („Manuel Baum bleibt Cheftrainer beim FCA") –, dazu **`kicker.de`** („Endgültige Dauerlösung: Baum bleibt FCA-Trainer – Bisheriger Interimstrainer unterschreibt für zwei Jahre"), **`sportschau.de`** („Offiziell: Manuel Baum bleibt Trainer des FC Augsburg"), eine **Trainerliste 2026/27** und der **Teamcheck 2026/27** auf `bundesliga.com`. Er übernahm Anfang Dezember 2025 auf einem Abstiegsplatz und führte den FCA auf **Platz 9 (43 Punkte, 45:61)**. Sein Trainerteam: **Alexander Frankenberger, Frank Fröhling, Felix Kling**, Analyst **Benedikt Brust**.

**Das ist exakt das Muster vom Vortag.** Gestern hatte ich den Kölner Trainer nach zwanzig Läufen gefunden und notiert: „Das war die richtige Entscheidung bei falscher Suche." **Hier dasselbe:** Ich habe nie nach „Baum Vertrag verlängert" gesucht, sondern nur nach „Augsburg Trainer 2026". **Eine Interimslösung ist kein Grund, einen Trainer zu verwerfen – sie ist ein Grund, nach der Dauerlösung zu suchen.** Das ist die Lehre, und sie hat heute zwei weitere Lücken geschlossen (Union, Schalke).

**Damit führt dieses Repo ab heute für alle 18 Vereine einen Trainer.** Die vollständige Liste steht unten.

### 2. Lerma und Ryerson sind Dortmunder – die Zuordnung ist aufgelöst

Gestern habe ich festgestellt, dass die Werder-Ausfallliste vom 29.09. **Julian Ryerson unter Werder führte**, obwohl er Dortmunder Außenverteidiger ist, und daraus geschlossen, die Liste sei in der Vereinszuordnung unzuverlässig. **Konsequenz gestern: Ich habe Justin Lerma von „Werder" auf „ungeklärt" gesetzt**, weil ich ihn am 29.09. allein auf diese Liste gestützt hatte.

**Heute ist beides aufgelöst, und zwar in dieselbe Richtung.** Eine **Dortmunder** Ausfallübersicht zum Spiel am 09.10. nennt **Justin Lerma mit Muskelverletzung** – neben **Emre Can (Kreuzbandriss)**, **Giannis Konstantelias** und **Filippo Mane**. **Lerma ist Dortmunder, nicht Bremer.** Und **Ryerson** ist über eine eigene Meldung bestätigt: **Er wurde im Nations-League-Spiel Norwegens gegen Portugal nach 66 Minuten ausgewechselt, nach einem Zusammenprall hat er Schmerzen im Rippenbereich**; eine Fundstelle spricht von einem **„erneuten Schlag auf die Rippen"**. Datiert über `ms-aktuell.de/…ryerson-verletzung-bvb-29-09-2026/` und `footy.de/2026/09/28/…`.

**Meine Umbuchung vom 29.09. war also falsch, meine Rücknahme von gestern richtig, und heute steht der ursprüngliche Stand wieder.** Was bleibt: **„Sieben gegen zwei" war nie korrekt** – zwei der sieben „Werder-Ausfälle" waren Dortmunder.

### 3. Die Werder-Ausfälle stehen heute auf einer anderen Liste – und sie ist in sich widersprüchlich

Nachdem die Liste vom 29.09. beschädigt ist, habe ich heute neu gesucht. **Eine partiebezogene Übersicht nennt vier Werder-Ausfälle: Jens Stage (Verletzung, muss operiert werden), Keke Topp (Kreuzbandriss, seit sechs Monaten), Salim Musah (Muskelverletzung Oberschenkel) und Justin Njinmah (langer Ausfall).**

**Diese Liste widerspricht sich selbst, und ich sage das, statt sie glatt zu übernehmen.** **Dieselbe Fundstelle nennt als voraussichtliche Werder-Aufstellung: „Backhaus – Agu, Pieper, Friedl, Deman – Lynen – Stage, Puertas – Njinmah, Schmid – Musah".** **Drei der vier als ausgefallen geführten Spieler stehen in der eigenen Startelf derselben Quelle** – Stage, Njinmah und Musah. **Das kann nicht beides stimmen.** Ich führe die vier als Ausfälle, weil die Diagnosen konkret sind (Operation, Kreuzbandriss, Oberschenkel), **aber ich stütze keinen Tipp auf die Aufstellung dieser Quelle.**

**Unabhängig bestätigt ist Felix Agu:** Zwei Bremer Quellen (`deichstube.de`, `weser-kurier.de`) berichten über **stockende Vertragsgespräche mit dem verletzten Felix Agu** – er habe sich **kurz nach der Rückkehr aus dem Zillertal-Trainingslager** verletzt, eine Rückkehr sei **„definitiv nicht unmittelbar"**. **Das ist die einzige heute doppelt belegte Werder-Personalie**, und sie bestätigt einen Namen, der schon am 29.09. auf der Liste stand. *Eine dieser Quellen nennt zudem Zahlen zur Lage:* **1.512 Ausfalltage und 184 verpasste Spiele** in dieser Saison, Ligaspitze.

**Was von „Kaba", „N'Diaye" und „Gyamerah" bleibt:** nichts Neues. **Moussa N'Diaye** taucht heute nur in einem Transferzusammenhang auf (Kaufoption „sehr, sehr gut"), **nicht als Verletzter**. **Kaba** findet heute keine Bestätigung. **Beide führe ich ab heute nicht mehr als Werder-Ausfälle**, sondern als unbelegt.

### 4. Schlotterbeck: DFB-bestätigt, eine Fundstelle sagt „Riss" – und der Vergleichsfall ist unangenehm

Gestern war der Stand: Außenbandverletzung im rechten Sprunggelenk, keine Operation nötig, Einsatz am 09.10. gefährdet, Ausfalldauer unbekannt. **Heute kommt dreierlei hinzu.**

**Erstens die Bestätigung.** Der **DFB** hat die **Außenbandverletzung** bestätigt; Schlotterbeck fehlt in den Spielen gegen **Serbien (01.10.)** und **Griechenland (04.10.)**. Belegt über Suchtreffer von **`kicker.de`** („Im Abschlusstraining verletzt: Schlotterbeck fällt für beide Länderspiele aus – Bestätigung vom DFB"), **`bundesliga.com`** und **`ran.joyn.de`** („Diagnose steht fest"). **Klopp selbst:** „Nico ist einfach umgeknickt – ohne Gegner- oder Mitspielereinwirkung. Es war einfach unglücklich."

**Zweitens die Verschärfung, und sie ist einfach belegt.** **Eine Fundstelle führt die Verletzung im Titel als `Außenbandriss`** (`neunzigplus.de`), nicht als Außenbandverletzung. **Alle übrigen – auch der DFB – sagen „Verletzung".** *Ich trage den Riss deshalb als Verdacht, nicht als Diagnose*, aber ich verschweige ihn nicht: **Es ist der Unterschied zwischen „vielleicht am 09.10. dabei" und „sicher nicht".**

**Drittens der Vergleichsfall, und er wiegt schwerer als beide.** **Dieselbe Verletzung am anderen Fuß hat er sich im zweiten WM-Gruppenspiel zugezogen – und sein Comeback für Dortmund war erst Mitte September.** **Seither hat er drei Spiele bestritten.** **Wenn der neue Fall dem alten gleicht, geht es nicht um ein Spiel, sondern um Monate.** Das ist keine Prognose, sondern eine Analogie – aber es ist die belastbarste Einordnung, die ich heute habe.

**Was ich ausdrücklich nicht verwende:** Die Suche liefert mehrere Expertenprognosen („Arzt gibt düstere Prognose", „Experte prognostiziert monatelange BVB-Pause", „operiert – halbes Jahr Pause"). **Die gehören alle zu anderen Verletzungen** – Einzelheiten unter „Verworfene Fundstellen".

### 5. Kade (Augsburg) arbeitet an der Rückkehr – gestern habe ich ihn als Ausfall geführt

Gestern stand bei Augsburg – Bayern: „**Augsburg verliert Kade, Breithaupt und Gregoritsch** (mit Diagnosen)", und darauf stützte ich die Aussage „drei Augsburger Offensivkräfte gegen einen Bayern-Offensivspieler".

**Heute steht dort das Gegenteil: Kade „arbeitet am Comeback gegen den FC Bayern".** Das ist kein gesicherter Einsatz, aber es ist auch kein Ausfall. **Aus drei Augsburger Offensivausfällen werden zwei plus ein Rückkehrkandidat**, und die Formulierung von gestern war damit zu scharf. **Bestätigt bleiben:** **Steve Mounié** (seit rund zwei Monaten, im Aufbautraining) und **Tim Breithaupt** (seit rund sechs Wochen). **Michael Gregoritsch** hat sich **im ersten Österreich-Länderspiel nach der WM am rechten Sprunggelenk verletzt**; ob er am 10.10. dabei ist, ist offen. **Mounié ist damit auch keine Unsicherheit mehr, sondern ein belegter Ausfall** – eine Lücke von gestern, die sich geschlossen hat.

### 6. Muslijas Kreuzbandriss ist nicht mehr widersprüchlich

Gestern: „**Muslijas Ausfallgrund bleibt widersprüchlich**, die Kreuzband-Lesart steht jetzt aber doppelt." **Heute nennt eine dritte, partiebezogene Fundstelle für Freiburg nur einen Ausfallgrund bei Florent Muslija: Kreuzbandriss.** Die Lesart ist damit dreifach belegt und ohne Gegenangabe. **Ich streiche den Widerspruch.**

### 7. Elversberg: die erste Überschneidung zweier Listen

Gestern: „**Drei Namen aus zwei Listen ohne jede Überschneidung: das ist keine geschlossene Lücke, das sind zwei unvollständige Listen.**" Am 29.09. standen dort **Luis Seifert** und **Jan Gyamerah**, gestern **nur Tom Zimmerschied**.

**Heute stehen Zimmerschied und Seifert gemeinsam auf den Fundstellen dieses Laufs** – Zimmerschied in der partiebezogenen Übersicht, Seifert in einer zweiten. **Das ist die erste Überschneidung, seit ich Elversberg führe**, und sie bestätigt beide Namen wechselseitig. **Gyamerah findet heute keine Bestätigung** und bleibt unbelegt. **Elversberg ist damit nicht mehr die dünnste Lage des Spieltags – das ist ab heute Frankfurt.**

### 8. Ouédraogos Ausfallgrund ist die Schulter, nicht „Verletzung"

Gestern: „Ouédraogo fällt bis Jahresende aus." **Heute präzisiert: Schulterverletzung, Rückkehr Ende Dezember 2026.** Dauer unverändert, Grund jetzt benannt.

## Nachrichtenlage in Kürze

**Es wird weiter nicht gespielt.** Seit dem 20.09. (4. Spieltag) gab es kein Pflichtspiel; die Tabelle unten ist deshalb unverändert. Die Vereine füllen die Pause mit Testspielen, Reisen und Sonderurlaub, und **genau daraus besteht die heutige Nachrichtenlage.**

**Die Trainerliste dieses Repos ist ab heute vollständig – alle 18:** Dortmund **Niko Kovač**, Bayern **Vincent Kompany**, Freiburg **Julian Schuster**, Augsburg **Manuel Baum** (heute belegt), Leverkusen (nicht benannt nötig – kein Wechsel berichtet), Mainz (dito), Elversberg (dito), Werder (dito), Leipzig (dito), Frankfurt **Adi Hütter** (heute belegt), Schalke **Miron Muslic** (heute belegt), Paderborn (dito), Köln **René Wagner**, Hoffenheim **Christian Ilzer**, Stuttgart **Sebastian Hoeneß**, HSV **Merlin Polzin**, Union **Mauro Lustrinelli** (heute belegt), Gladbach **Alexander Blessin**. *Die vier heute neu belegten im Detail:* **Baum** (oben), **Lustrinelli** – seit 01.07.2026, 50, Schweizer, zuvor Meister mit dem FC Thun, Assistenten Michel Renggli und Sascha Stauch, belegt über `kicker.de` (Trainerseite 2026/27 für Union), die Vereinsseite `fc-union-berlin.de`, `sportschau.de` und `sport1.de` –, **Muslic** – seit 01.07.2025, Vertrag bis 2028, Aufstieg mit Schalke als Zweitligameister zwei Spieltage vor Schluss – und **Hütter** bei Frankfurt, belegt über `hessenschau.de` und den Teamcheck 2026/27.

**Testspiele und Reisen, die heute belegt sind:**
- **Gladbach gewann das Blessin-Debüt 3:0 bei Sportfreunde Siegen** (Regionalliga), Tore **Robin Hack** und **Shuto Machino**. **Daiki Hashioka, Yukhym Konoplya und Zento Uno bestritten ihr erstes Spiel nach Verletzung**, **Kapitän Tim Kleindienst fehlte erkältet.** **Nächster Test: 03.10. beim FC St. Pauli am Millerntor**, Blessins Ex-Club.
- **Paderborn hat die fünftägige USA-Reise mit einem 1:0 bei D.C. United abgeschlossen** – **Gabriel Vidović** traf per Elfmeter, **knapp 10.000 Zuschauer im Audi Field.** **Damit ist die Lücke von gestern geschlossen** („Das Paderborner Testspielergebnis liegt nach diesem Lauf").
- **Hoffenheim** hat **zwei Testspiele** bestritten, **18 Profis** waren abgestellt. **Gegner und Termine sind weiterhin nicht belegt** (siehe Verworfene Fundstellen).
- **Freiburg** hat der Mannschaft **eine Woche Sonderurlaub** gegeben.
- **Frankfurt** arbeitet unter Hütter **mit reduziertem Kader** an der Intensität; **14 Profis** sind auf Länderspielreise.

**Europapokal-Belastung spielt für diesen Spieltag keine Rolle, aber sie beginnt unmittelbar danach:** **Stuttgart** spielt am **14.10. in der Champions League gegen Slovan Bratislava**, **Freiburg** am **15.10. in der Conference League gegen FK Jablonec**. **Beide Termine liegen nach dem 5. Spieltag** – ein Vorbelastungsargument gibt es also für keine der neun Partien. *Für Bayern kommt die Belastung danach massiv:* **neun Spiele in 29 Tagen**, darunter Arsenal, Atlético, Dortmund und Leipzig.

### Heute ausdrücklich verworfene Fundstellen

**1. Drei Schlotterbeck-Prognosen, die zu anderen Verletzungen gehören.** „Arzt gibt düstere Prognose … drei Monate", „Nicht maximal schwerwiegend" und „Experte prognostiziert monatelange BVB-Pause" **beschreiben einen Innenbandriss im linken Sprunggelenk gegen die Elfenbeinküste**, kommentiert von **Prof. Christian Lüring (Klinikum Dortmund)**, mit verpasster Vorbereitung, Supercup gegen Bayern und Saisonauftakt. **Das ist nicht die Verletzung von vorgestern** – anderer Fuß, anderes Band, anderer Anlass. Auffällig: **zwei verschiedene Überschriften tragen dieselbe Artikel-ID** (`bltd4acecfbf3fedd8a`). **Ebenfalls verworfen:** „Schlotterbeck operiert – halbes Jahr Pause" (**Meniskusriss im Knie**) und eine Fundstelle mit der Adresse `bvbwld.de/2026/06/25/…` (**Juni 2026, Knie**). **Keine dieser Quellen sagt etwas über die Ausfalldauer der aktuellen Verletzung.**

**2. Eine Hoffenheim-Aufstellung aus der Saison 2025/26.** Eine Abfrage zu Hoffenheim – HSV liefert vollständige Aufstellungen („Heuer Fernandes – Capaldo, Torunarigha … / Baumann – Coufal, Hranáč …") und den Satz, **bei Hoffenheim gebe es keine verletzten oder gesperrten Spieler.** **Die Adressen entlarven es:** `kicker.de/hsv-gegen-hoffenheim-…` – **falsche Richtung**, unsere Partie ist in Hoffenheim – und `bundesliga.com/…/matchday/2025-2026/31/hamburger-sv-vs-tsg-hoffenheim/liveticker` – **Saison 2025/26, 31. Spieltag.** Dazu ein Ticker mit Spielverlauf („Asllani und Lemperle belohnen Hoffenheim"). **Das erklärt auch, warum Grønbæk dort in der HSV-Startelf steht, obwohl er verletzt ist.** **Verworfen, inklusive der angeblich leeren Hoffenheimer Verletztenliste.**

**3. Eine Widmer-Angabe zur falschen Partie.** Eine Fundstelle meldet, **Silvan Widmer habe eine Ein-Spiel-Sperre abgesessen und kehre in die Startelf zurück**, wobei Mwene **„für die Reise in die BayArena"** auf die Bank rücke. **Unsere Partie ist in Mainz (MEWA Arena), nicht in Leverkusen** – und es ging um eine **Sperre**, während mein Stand eine **Patellasehnenverletzung** führt. **Falsches Spiel, verworfen.** Widmers Status bleibt damit so unsicher wie gestern.

**4. Eine Leipzig-Meldung zur falschen Richtung.** „RB Leipzig to make late calls on Orban and Lukeba **for Frankfurt trip**", Adresse `fotmob.com/matches/eintracht-frankfurt-vs-rb-leipzig`. **Unsere Partie ist in Leipzig.** *Teilweise gerettet:* Eine **zweite** Fundstelle behandelt ausdrücklich „**RB Leipzigs Hoffnungen und Sorgen vor dem Spiel gegen Frankfurt**" und nennt dieselbe Lukeba-Diagnose. **Die Diagnose übernehme ich aus der zweiten Quelle, nicht aus der ersten.**

**5. Ein Hoffenheimer Testspielgegner aus einer anderen Länderspielpause.** „Testspiel in der Länderspielpause: TSG trifft auf die SV Elversberg" – Adresse `tsg-hoffenheim.de/aktuelles/news/**2026/03**/…`. **März 2026, eine frühere Pause.** **Verworfen** – die Hoffenheimer Testspielgegner bleiben offen.

**6. Ein Ergebnis für ein Spiel, das noch nicht stattgefunden hat.** Eine Zusammenfassung zu Union – Elversberg schreibt: „**The match ended in a 0:0 draw.**" **Die Partie ist am 10.10., heute ist der 01.10.** Es handelt sich um eine Prognose oder ein fremdes Spiel. **Verworfen.** *Aus derselben Abfrage behalte ich nur die Trainerangabe Lustrinelli*, weil die unabhängig über `kicker.de` und die Vereinsseite belegt ist.

### Offen benannte Restlücken und Unsicherheiten

- **Schlotterbecks Ausfalldauer ist weiterhin unbekannt.** Belegt sind die Verletzung, der Ausfall für beide Länderspiele und die Gefährdung des 09.10.; „Riss" steht einfach, der Vergleichsfall deutet auf länger. **Das bleibt die wichtigste offene Frage des Spieltags.**
- **Ryersons Einsatz am 09.10. ist offen** (Rippen). Entscheidend ist, ob er nach den Nations-League-Spielen beschwerdefrei trainieren kann.
- **Die Werder-Ausfallliste widerspricht ihrer eigenen Aufstellung** (Stage, Njinmah, Musah). Nur **Agu** ist doppelt und bremisch belegt.
- **Über Führich und Stiller weiß ich nichts Belastbares** – die eine Fundstelle führt sie als verletzt, die entkräftende ist über „Nagelsmann" als alt entlarvt.
- **Die Stuttgarter Neunerliste ist nicht datierbar** und trägt keinen Tipp (unten im Detail). Belegt ist allein **Zagadou**.
- **Bei Sven Michel (Paderborn) widersprechen sich zwei Fundstellen desselben Laufs:** eine meldet sein **Comeback nach Muskelbündelriss**, eine zweite führt ihn als **Ausfall**. Ungeklärt.
- **Zentners Einsatz am 10.10. bleibt offen** – „Mainz hofft auf Zentner-Rückkehr gegen Leverkusen" ist eine Hoffnung, keine Zusage.
- **Widmers Status ist nach der Verwerfung von Punkt 3 unverändert unsicher.**
- **Dakas Ausfall ist weiterhin nicht vereinsbestätigt**, heute aber zweifach berichtet.
- **Kramarićs aktueller Zustand ist unklar:** „angeschlagen" ist belegt, die Leisten-Operation gehört in den Sommer nach der WM.
- **Gosens' Verfügbarkeit stützt sich nur darauf, dass er im Kader geführt wird** – ein schwaches Indiz, keine Meldung.
- **Gregoritsch, Kade und Mounié** – nur Mounié und Breithaupt sind klare Ausfälle; die anderen zwei sind offen.
- **Zu Frankfurt liegt heute kein einziger Verletzter vor.** Belegt sind nur ein reduzierter Kader, 14 Abstellungen, **Robin Koch nach Infekt zurück im Training**, **Dōan fit gemeldet**, **Aséko planmäßig geschont**. **Das ist ab heute die dünnste Personallage des Spieltags.**
- **Die dritte Leipziger Niederlage** aus „drei Niederlagen in vier Pflichtspielen" kann ich weiterhin keinem Wettbewerb zuordnen.
- **Die Tabelle ist aus den einzeln belegten Ergebnissen gerechnet**, weil keine Tabellenseite abrufbar ist. Seit dem 20.09. wurde kein Pflichtspiel ausgetragen, die Rechnung kann sich nicht verschoben haben.

### Tabelle nach dem 4. Spieltag (alle 36 Partien)

Aus den einzeln belegten Ergebnissen gerechnet. **Form = 1. bis 4. Spieltag von links nach rechts.** Werte unverändert zum Vortag – seit dem 20.09. wurde nicht gespielt.

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

**Heim- und Auswärtszahlen, die heute mehrere Tipps tragen:**

- **Dortmund zu Hause:** 2:0 gegen HSV, 3:0 gegen Paderborn – **zwei Spiele, zwei Zu-null.**
- **HSV auswärts:** 0:2 in Dortmund, 0:5 in Leipzig – **zwei Spiele, null Tore.** Beide HSV-Tore fielen zu Hause.
- **Leipzig zu Hause:** 3:0 gegen Gladbach, 5:0 gegen HSV – **zwei Spiele, 8:0, zwei Zu-null.**
- **Gladbach auswärts:** 0:3 in Leipzig, 0:5 in Freiburg – **null Tore, 0:8.**
- **Stuttgart auswärts:** 1:5 in München, 1:2 in Hoffenheim – **null Punkte, 2:7.**
- **Paderborn zu Hause:** 0:0 Mainz, 0:1 Freiburg, 3:1 Hoffenheim – **vier Punkte, zuletzt ein 3:1.**
- **Augsburg zu Hause:** 3:0 Schalke, 2:2 Leverkusen – **fünf Tore in zwei Spielen.**
- **Bayern:** 14:2 in vier Spielen – **nur zwei Gegentore in der ganzen Saison.**

## Warum heute kein Tipp geändert wird

**Das ist der erste Lauf dieses Repos ohne Änderung, und ich will nicht, dass er wie Trägheit aussieht.** Deshalb die Prüfung offen.

**Die Regel, an der ich mich seit Tagen messe, lautet: Ein Tipp ändert sich, wenn eine konkrete, datierbare neue Information ihn trägt – nicht, wenn ich alte Angaben umgewichte.** Heute gibt es **vier** neue Informationen von Gewicht, und keine von ihnen bewegt einen Tipp:

1. **Schlotterbeck ist DFB-bestätigt und möglicherweise ein Riss.** **Das stützt die Änderung von gestern (2:0 → 2:1), es verlangt keine neue.** Eine weitere Verschärfung auf 1:1 oder 2:2 wäre möglich – **dagegen steht, dass Dortmund mit Waldemar Anton einen erprobten Ersatz hat**, der schon während Schlotterbecks letztem Ausfall Innenverteidiger war, dazu **Joane Gadou**. **Und Werders Ausfälle treffen den Angriff** (Topp, Njinmah, Musah). **Beides zusammen hält mich bei 2:1.**
2. **Die drei HSV-Offensivausfälle sind einzeln bestätigt.** **Das stützt die zweite Änderung von gestern (2:1 → 2:0).** Mehr als ein Zu-null-Heimsieg lässt sich daraus nicht machen.
3. **Köln stützt Wagner öffentlich – und Gladbach gewinnt den Debüt-Test mit drei Rückkehrern.** **Diese zwei Fundstellen zeigen in entgegengesetzte Richtungen und heben sich auf.** Ausführlich unten beim Tipp.
4. **Die Stuttgarter Ausfallliste wäre die vierte Änderung gewesen – und sie hält nicht.** Ausführlich unten beim Tipp.

**Die Verteilung bleibt bei vier Heimsiegen, drei Auswärtssiegen, zwei Remis.** Nach einem Lauf mit zwei Änderungen in entgegengesetzte Richtungen und einer Rücknahme ist ein Lauf ohne Änderung **kein schlechtes Zeichen, sondern das erwartbare, wenn acht Tage vor dem Anpfiff nicht gespielt wird.** **Was sich heute verbessert hat, ist nicht die Trefferwahrscheinlichkeit, sondern die Belegdichte.**

---

## Die Tipps zum 5. Spieltag

### Borussia Dortmund – SV Werder Bremen
**Freitag, 09.10.2026, 20:30 Uhr** (Signal Iduna Park)
**Tipp: 2:1**
*unverändert*
***Die Änderung von gestern ist heute besser belegt als bei ihrer Vornahme – und das, obwohl eine ihrer zwei Säulen weggebrochen ist.*** Gestern stand die Änderung auf (a) Schlotterbeck und (b) der Werder-Liste mit „sieben gegen zwei". **(b) ist erledigt: zwei der sieben Namen waren Dortmunder** (Ryerson, Lerma – oben aufgelöst). **(a) ist dafür deutlich härter geworden:** **Der DFB hat die Außenbandverletzung im rechten Sprunggelenk bestätigt**, Schlotterbeck fehlt gegen Serbien und Griechenland, **eine Fundstelle führt sie als `Außenbandriss`**, und **die gleiche Verletzung am anderen Fuß hat ihn vom zweiten WM-Gruppenspiel bis Mitte September gekostet.** Seither hat er **drei Spiele** bestritten.
***Dortmunds Defensive ist die am stärksten betroffene Mannschaftsteil des Spieltags.*** Neben Schlotterbeck: **Julian Ryerson** (Rippen, nach 66 Minuten gegen Portugal ausgewechselt, Status offen) – und zu ihm heißt es ausdrücklich, **für die rechte Seite gebe es im Kader keine adäquate Alternative**; **Emre Can** (Kreuzbandriss), **Justin Lerma** (Muskelverletzung), **Filippo Mane**, **Giannis Konstantelias**. **Das sind bis zu fünf Ausfälle, vier davon defensiv.**
***Warum der Sieger trotzdem nicht wackelt.*** **Dortmund ist 4-0-0 mit 9:2 und hat beide Heimspiele zu null gewonnen** (2:0, 3:0). **Für Schlotterbeck steht Waldemar Anton bereit** – vier Bundesligaspiele in dieser Saison, **und schon während Schlotterbecks letztem Ausfall die Lösung in der Innenverteidigung** –, dazu **Joane Gadou**. **Ein Ausfall mit erprobtem Ersatz ist ein anderer Ausfall als einer ohne.**
***Und Werder kommt selbst beschädigt.*** **Keke Topp** (Kreuzbandriss, seit sechs Monaten), **Jens Stage** (muss operiert werden), **Salim Musah** (Oberschenkel), **Justin Njinmah** (langer Ausfall), **Felix Agu** (Rückkehr „definitiv nicht unmittelbar", bremisch doppelt belegt). **Drei dieser Namen sind Offensivspieler** – und Werder hat 8 Tore in 4 Spielen erzielt, aber auch 8 kassiert. *Die Einschränkung, die ich mitliefere:* **Dieselbe Quelle, die Stage, Njinmah und Musah als Ausfälle führt, stellt sie in ihre eigene Startelf.** **Ich stütze mich auf die Diagnosen, nicht auf die Aufstellung.**
***Das Fazit in einem Satz:*** **Dortmunds Abwehr ist angeschlagen, aber ersetzbar; Werders Angriff ist angeschlagen und reist zu einem Gegner, der zu Hause noch kein Tor zugelassen hat.** **2:1 – der Heimsieg steht, das Gegentor bleibt drin.**

### FC Augsburg – FC Bayern München
**Samstag, 10.10.2026, 15:30 Uhr** (WWK Arena)
**Tipp: 1:2**
*unverändert*
***Musiala fällt definitiv aus, und das ist heute keine Prognose mehr.*** **Muskelfaserriss im rechten Oberschenkel, zugezogen beim Aufwärmen vor dem Nations-League-Spiel gegen die Niederlande**, laut Sky **drei bis vier Wochen.** **Das Spiel in Augsburg kommt ausdrücklich zu früh.** **Kompany geht bei Muskelverletzungen kein Risiko ein**; als realistische Rückkehrtermine werden **Freiburg oder Magdeburg** genannt, **das eigentliche Ziel ist Dortmund am 31.10.**
***Auf Augsburger Seite muss ich meine gestrige Formulierung zurücknehmen.*** Gestern hieß es „Augsburg verliert Kade, Breithaupt und Gregoritsch". **Heute arbeitet Kade ausdrücklich am Comeback gegen den FC Bayern.** Belegt ausgefallen sind **Steve Mounié** (rund zwei Monate, im Aufbautraining) und **Tim Breithaupt** (rund sechs Wochen); **Michael Gregoritsch** hat sich **im ersten Österreich-Länderspiel nach der WM am rechten Sprunggelenk verletzt** und ist offen. **Aus drei Ausfällen werden zwei plus zwei Fragezeichen** – der Personalvorteil, den ich Bayern gestern zugeschrieben habe, ist kleiner als behauptet.
***Und der Trainer steht jetzt: Manuel Baum, Vertrag bis 30.06.2028*** – über die Vereinsseite belegt, Einzelheiten oben. **Baum hat den FCA im Dezember 2025 von einem Abstiegsplatz auf Platz 9 geführt**, und er kennt den Club aus einer ersten Amtszeit 2016–2019. **Für den Tipp ändert das nichts, aber es schließt die letzte Trainerlücke dieses Repos.**
***Warum 1:2 und nicht 0:2.*** **Augsburg hat in zwei Heimspielen fünf Tore erzielt** (3:0 gegen Schalke, 2:2 gegen Leverkusen) und steht mit 7 Punkten und 11:6 auf Platz 4. **Warum nicht 1:3:** **Bayern hat in vier Spielen nur zwei Gegentore kassiert** (14:2). **Ein Tor für Augsburg ist die Zahl, die zu beiden Reihen passt** – und Musialas Ausfall ist bei dieser Kaderdecke genau ein Tor wert, nicht mehr.

### TSG Hoffenheim – Hamburger SV
**Samstag, 10.10.2026, 15:30 Uhr** (SNP Arena)
**Tipp: 2:0**
*unverändert*
***Die Rücknahme von gestern war richtig, und heute ist sie dreifach einzeln belegt.*** Gestern hatte ich 2:1 auf 2:0 zurückgenommen, weil der HSV-Angriff ausfällt. **Heute steht jeder der drei Namen für sich:**
- **Albert Grønbæk: Muskelfaserriss im rechten Oberschenkel, zugezogen im Länderspiel mit Dänemark, Ausfall mindestens bis Mitte Oktober.** **Er ist der Topscorer des HSV.** Datiert über `ms-aktuell.de/…-26-09-2026/`, dazu `ligaportal.at` („Faserriss").
- **Terem Moffi: kommt für den 10.10. ausdrücklich zu spät** – **anhaltende Knieprobleme**, **er hat das Mannschaftstraining verpasst** und nur leichte Laufeinheiten auf dem Platz absolviert.
- **Patson Daka: Muskelverletzung**, er fehlte im sambischen Nationalmannschaftskader. **Und er ist derjenige, der stürmen soll, „wenn er fit ist"** – das ist der Satz, der die Lage beschreibt: **Der einzige verbleibende Angreifer ist selbst fraglich.**
***Dazu die Zahl, die ich vorgestern übersehen hatte und die hier alles trägt:*** **Der HSV hat in zwei Auswärtsspielen kein Tor erzielt** (0:2 in Dortmund, 0:5 in Leipzig). **Beide Saisontore fielen zu Hause.** **Ein Gegentor im Tipp würde vom HSV das erste Auswärtstor der Saison verlangen – mit einem Angriff, in dem zwei Spieler ausfallen und der dritte fraglich ist.** Trainer **Merlin Polzin** muss die Offensive in dieser Pause neu bauen.
***Die Einschränkung, und sie ist heute neu:*** **Erstmals liegt überhaupt eine Hoffenheimer Personalangabe vor – und sie ist keine gute.** **Vladimír Coufal und Andrej Kramarić sind für den 10.10. als „angeschlagen" geführt.** **Kramarić ist Hoffenheims wichtigster Offensivspieler**, und ein Leisteneingriff im Sommer nach der WM steht in seiner Vorgeschichte. *Ich löse das nicht auf:* „angeschlagen" ist kein Ausfall, und **die Lücke „aktuelle Hoffenheimer Verletztenliste" ist damit angekratzt, nicht geschlossen.** **Was ich ausdrücklich verwerfe, ist die Angabe, Hoffenheim habe keine Verletzten – sie stammt aus der Saison 2025/26** (oben begründet).
***Warum 2:0 trotzdem steht:*** **Hoffenheim ist mit 3 Punkten Vierzehnter und alles andere als stark** – aber **es hat zu Hause gegen Stuttgart 2:1 gewonnen** und in zwei Heimspielen vier Tore erzielt. **Gegen einen Gast, der auswärts noch nicht getroffen hat und dem die Stürmer fehlen, reicht das für zwei Tore und die Null.** Ein angeschlagener Kramarić ist das Risiko dieses Tipps, und ich benenne es als solches.

### 1. FSV Mainz 05 – Bayer 04 Leverkusen
**Samstag, 10.10.2026, 15:30 Uhr** (MEWA Arena)
**Tipp: 1:1**
*unverändert*
***Meine Änderungsbedingung von vorgestern ist endgültig erledigt, und zwar in beiden Hälften.*** Sie lautete: Widmer fällt über den 10.10. hinaus aus **und** Zentner wird nicht fit → 1:2. **Zu Zentner ist die Nachricht heute so gut wie bisher nie:** **„Mainz hofft auf Zentner-Rückkehr gegen Leverkusen"** – die Partie wird namentlich als Rückkehrspiel geführt. Seine **Handverletzung stammt aus dem 1:3 gegen Frankfurt** (3. Spieltag), Vertreter ist **Alexander Schwolow**. *Eine Hoffnung ist keine Zusage* – ich führe Zentner weiter als offen, **aber als Rückkehrkandidaten, nicht als Ausfall.** **Zu Widmer muss ich dagegen die positive Meldung von gestern entwerten:** Die heutige Fundstelle, die ihn in die Startelf zurückkehren lässt, **gehört zu einem Auswärtsspiel in der BayArena und zu einer Sperre** – **falsches Spiel** (oben verworfen). **Damit ist Widmer so unsicher wie am 29.09.**
***Neu und für beide Seiten symmetrisch: je zwei belegte Ausfälle.*** **Mainz: Dominik Kohr** (nach Operation) und **Silas** (**Schien- und Wadenbeinbruch** – ein schwerer Langzeitfall). **Leverkusen: Guéla Doué** (Wadenmuskelverletzung) und **Kennet Eichhorn** (Stoffwechselerkrankung). **Zwei gegen zwei ist kein Argument für eine Verschiebung in die eine oder andere Richtung.**
***Die Tabellenlage sagt dasselbe.*** **Mainz 7 Punkte, 10:6, Sechster. Leverkusen 7 Punkte, 10:5, Fünfter.** **Gleiche Punktzahl, fast gleiche Tore, ein Platz Unterschied.** Mainz hat zu Hause Paderborn 0:0 und Frankfurt 1:3 gespielt, Leverkusen auswärts bei Elversberg 2:3 verloren und in Augsburg 2:2 gespielt – **der Gast hat auswärts noch nicht gewonnen.** **1:1 ist bei dieser Gleichheit kein Ausweichen, sondern das Ergebnis.**
***Die neue Bedingung, die ich gestern angekündigt habe – und sie stellt ausschließlich auf Vereinsangaben ab:*** **Wenn Mainz bis zum 09.10. bestätigt, dass Zentner spielt, gehe ich auf 2:1.** **Wenn Mainz bestätigt, dass er nicht spielt, gehe ich auf 1:2.** **Aggregatorangaben lösen diese Bedingung nicht aus** – nach drei verworfenen Fundstellen zu dieser einen Partie in drei Läufen ist das die einzige Schwelle, die ich noch akzeptiere.

### 1. FC Union Berlin – SV 07 Elversberg
**Samstag, 10.10.2026, 15:30 Uhr** (Alte Försterei)
**Tipp: 1:2**
*unverändert*
***Die sieben Unioner Ausfälle stehen heute den zweiten Tag in Folge, und das ist für dieses Repo ungewöhnlich viel Stabilität.*** **Robert Skov**, **Marvin Friedrich**, **Andrej Ilić**, **Oliver Burke**, **Stanley Nsoki**, **Andrik Markgraf** und **Frederik Rønnow** – alle sieben erneut bestätigt. **Zwei Präzisierungen:** **Markgraf wird heute ausdrücklich mit Kreuzbandverletzung geführt** (gestern „Kreuzbandriss" – gleiche Lesart, zweiter Beleg), und **Rønnow steht mit Oberschenkelverletzung als „fraglich"**, nicht als sicherer Ausfall. **Das ist eine kleine Entschärfung gegenüber gestern**, und ich trage sie mit: **Unions Stammtorwart ist fraglich, nicht weg.**
***Trotzdem bleibt es die Personalie, die am direktesten auf das Ergebnis wirkt.*** **Union hat in vier Spielen 17 Gegentore kassiert** – 4:17, Platz 17, ein Punkt, kein Sieg. **Bei einer Mannschaft mit dieser Defensivbilanz ist ein fraglicher Torwart neben zwei fehlenden Innenverteidigern (Friedrich, Nsoki) die Zuspitzung eines Problems, das ohnehin das größte der Liga ist.**
***Auf Elversberger Seite ist heute die Lücke geschlossen, die ich seit drei Läufen offen führe.*** **Zimmerschied und Seifert stehen zum ersten Mal gemeinsam auf den Fundstellen eines Laufs** – Zimmerschied in der partiebezogenen Übersicht, **Luis Seifert** in einer zweiten. **Das ist die erste Überschneidung zweier Elversberg-Listen**, und sie bestätigt beide Namen wechselseitig. **Gyamerah bleibt unbelegt.** **Zwei belegte Gäste-Ausfälle gegen sieben beim Gastgeber.**
***Und der Unioner Trainer steht ab heute: Mauro Lustrinelli***, seit 01.07.2026, 50, Schweizer, zuvor Meister mit dem FC Thun, über `kicker.de`, die Vereinsseite und `sportschau.de` belegt. **Ein Trainer im ersten Jahr mit einem Punkt aus vier Spielen** – das ist Kontext, kein Tippargument, und ich baue nichts darauf.
***Die Abwägung:*** **Elversberg hat als Aufsteiger in Gladbach 4:3 und gegen Leverkusen 3:2 gewonnen – der Club trifft, und er trifft auswärts.** **7 Punkte gegen 1, 8:7 gegen 4:17, zwei Ausfälle gegen sieben.** **1:2 bleibt, und dieser Tipp ist nach wie vor der am besten belegte der neun.** *Was ich verwerfe:* die Zusammenfassung, die für diese Partie ein **0:0** nennt – **sie wird erst am 10.10. gespielt.**

### SC Paderborn 07 – VfB Stuttgart
**Samstag, 10.10.2026, 15:30 Uhr** (Home Deluxe Arena)
**Tipp: 1:2**
*unverändert* — **und das ist heute eine aktiv getroffene Entscheidung gegen eine Änderung, nicht ein Stehenlassen. Ich erkläre sie ausführlich, weil sie das Methodische dieses Laufs zeigt.**
***Die Änderung, die ich nicht vornehme.*** Eine Fundstelle liefert heute **neun Stuttgarter Ausfälle**: **Luca Jaquez** (Muskel), **Chris Führich** (Muskel, fraglich), **Nikolas Nartey** (Muskel), **Jeremy Arévalo** (Rücken), **Dan-Axel Zagadou** (Oberschenkelrückseite), **Lorenz Assignon** (Schulter), **Dennis Seimen** (Oberschenkelrückseite), **Justin Diehl** (Oberschenkel) und **Leo Sauer** (Oberschenkelrückseite). **Zusammen mit Stuttgarts Auswärtsbilanz – null Punkte, 2:7 – wäre das der Stoff für 1:1 gewesen**, und gestern stand hier ausdrücklich „1:2 bleibt, weiter mit kleinem Abstand zu 1:1".
***Warum die Liste nicht trägt.*** **Ich habe versucht, sie zu datieren, und bin an genau einem Namen gescheitert.** Zu **Führich** liefert die Gegenprobe eine Meldung, er sei **mit Stiller in den DFB-Kader nachnominiert** worden – was ihn gesund machen würde. **Diese Meldung nennt als Bundestrainer Julian Nagelsmann.** **Der Bundestrainer heißt Jürgen Klopp**, heute mehrfach wörtlich zitiert. **Also ist die Gegenprobe alt – und über Führich weiß ich damit nichts.** **Eine Liste, deren prominentesten Namen ich nicht datieren kann, ist keine Grundlage für eine Tippänderung.** **Dieses Repo hat in den letzten drei Läufen drei Aggregatorlisten verworfen** (Werder-Zuordnung, Hoffenheim-Aufstellung 2025/26, Widmer-Sperre). **Die vierte nehme ich nicht ungeprüft.**
***Was von Stuttgart belegt bleibt – und es ist genau ein Name.*** **Dan-Axel Zagadou: muskuläre Verletzung der Oberschenkelrückseite, zugezogen am 09.08.2026 im Testspiel gegen Everton (3:1), nach Klubangaben mehrere Wochen Ausfall** – und, für unsere Partie entscheidend: **er absolviert im Zusammenhang mit dem Paderborn-Spiel Individualprogramm auf dem Rasen.** **Das ist vereinsnah belegt und bedeutet: Zagadou spielt am 10.10. nicht.** Ein Innenverteidiger-Ausfall bei einer Mannschaft mit 9 Gegentoren in 4 Spielen. **Trainer ist Sebastian Hoeneß.**
***Auf Paderborner Seite ist heute die Lücke von gestern geschlossen – und eine neue aufgegangen.*** **Das Testspiel in den USA endete 1:0 für Paderborn gegen D.C. United**, **Gabriel Vidović** per Elfmeter, **knapp 10.000 Zuschauer im Audi Field**, Abschluss einer **fünftägigen Reise**. **Die neue Lücke ist eine Erkältungswelle:** **Laurin Curda und Raphael Obermair spielten im Abschlusstest gar nicht, Mattes Hansen und Tom Baack nur die zweite Hälfte**; **Curda, Obermair und Hansen fehlten am Dienstag im Training mit Erkältungssymptomen.** **Vier angeschlagene Spieler acht Tage vor dem Spiel.** *Und ein Widerspruch, den ich nicht auflöse:* **Eine Fundstelle meldet das Comeback von Sven Michel nach Muskelbündelriss, eine zweite führt ihn als Ausfall** – zusammen mit **Awortwie-Grant, Klaas und Gayret**.
***Die Abwägung, und sie ist eng.*** **Für 1:1 spricht: Stuttgart hat auswärts null Punkte und 2:7, Zagadou fehlt, und Paderborn hat zuletzt zu Hause 3:1 gegen Hoffenheim gewonnen.** **Für 1:2 spricht: Paderborn hat in drei Heimspielen vier Punkte und nur drei Tore in der ganzen Saison erzielt** (3:5 insgesamt – **die schwächste Offensive des Spieltags**), **die Erkältungswelle trifft vier Spieler, und Stuttgarts Neunerliste ist unbelegt, also darf ich sie auch nicht zu Stuttgarts Nachteil verwenden.** **Beides zusammen lässt den Abstand klein, aber es dreht ihn nicht.** **1:2 bleibt – und wenn sich die Stuttgarter Liste datieren lässt oder Stuttgart selbst Ausfälle bestätigt, ist das die wahrscheinlichste Änderung des nächsten Laufs.**

### RB Leipzig – Eintracht Frankfurt
**Samstag, 10.10.2026, 18:30 Uhr** (Red Bull Arena)
**Tipp: 2:1**
*unverändert* — **und dieser Tipp bleibt der wackligste der neun, aber aus einem anderen Grund als gestern.**
***Leipzigs Ausfallliste ist heute die zweitlängste des Spieltags.*** **Assan Ouédraogo** (**Schulterverletzung, Rückkehr Ende Dezember 2026** – gestern hatte ich nur „bis Jahresende"), **Brajan Gruda**, **Marc Guiu**, **Rocco Reitz** (Oberschenkel) und **Christoph Baumgartner** (Oberschenkel). **Dazu Castello Lukeba**, über den **kurzfristig entschieden wird** – **Adduktoren- bzw. Leistenverletzung**, er arbeitet sich an die Belastung heran. **Das bestätigt meine Angabe von gestern („Leistenprobleme") mit einem zweiten Beleg** und stammt aus einer Fundstelle, die **ausdrücklich unsere Partie behandelt** („vor dem Spiel gegen Frankfurt"); die anderslautende Meldung zur „Frankfurt trip" habe ich verworfen. **Fünf Ausfälle plus ein Fragezeichen, davon zwei zentrale Mittelfeldspieler.**
***Frankfurt dagegen ist heute die dünnste Lage des Spieltags – und das ist ausdrücklich ein Mangel meiner Recherche, kein Befund.*** **Ich habe zu Frankfurt keinen einzigen Verletzten.** Belegt ist nur: **Adi Hütter arbeitet mit reduziertem Kader an der Intensität**, **14 Profis sind auf Länderspielreise**, **Robin Koch ist nach einem Infekt ins Training zurückgekehrt**, **Ritsu Dōan hat sich bei seiner Nationalmannschaft fit gemeldet**, **Noël Aséko wurde in der U21 planmäßig geschont.** **Das sind drei positive und keine negativen Meldungen.** **Wenn Frankfurt tatsächlich vollständig ist, steht hier fünf gegen null – und dann ist 2:1 zu optimistisch.**
***Warum ich den Heimsieg trotzdem halte, und es ist eine einzige Zahl.*** **Leipzig hat beide Heimspiele zu null gewonnen: 3:0 gegen Gladbach, 5:0 gegen den HSV. 8:0 in zwei Spielen in der Red Bull Arena.** **Beide Leipziger Niederlagen fielen auswärts** (1:3 in Bremen, 0:2 in Leverkusen). **Das ist eine Mannschaft, die zu Hause eine andere ist als auswärts**, und die fünf Ausfälle treffen Mittelfeld und Angriff, nicht die Abwehr, die diese zwei Zu-null gehalten hat.
***Und Frankfurt bringt die Gegenzahl mit:*** **9:10 Tore, 5 Punkte, Platz 10 – die Eintracht hat in vier Spielen zehn Gegentore kassiert**, mehr als jede andere Mannschaft der oberen Tabellenhälfte, und auswärts bei Union 3:3 gespielt und gegen Augsburg 1:4 verloren. **Eine Mannschaft, die auswärts trifft und hinten offen ist, passt zu 2:1.**
***Was diesen Tipp kippen würde:*** **eine Frankfurter Ausfallliste, die zeigt, dass die Eintracht komplett ist** – dann geht es auf 1:1 –, **oder eine Leipziger Bestätigung, dass Lukeba ausfällt** – dann bleibt es bei 2:1, aber knapper. **Die fehlende Frankfurter Personallage ist ab heute die wichtigste Recherchelücke dieses Repos.**

### 1. FC Köln – Borussia Mönchengladbach
**Sonntag, 11.10.2026, 15:30 Uhr** (RheinEnergieStadion)
**Tipp: 1:1**
*unverändert* — **aber die Begründung wird heute zum zweiten Mal in zwei Läufen umgebaut, und das sage ich zuerst.**
***Der Stand der Begründungen, offen aufgeschrieben.*** Die Änderung auf 1:1 erfolgte am 29.09. und stand auf zwei Säulen: **(a) Blessin habe drei Wochen Vorbereitungszeit** und **(b) bei Köln trainierten nur zwölf Feldspieler.** **(a) habe ich gestern selbst widerlegt** („Gladbach-Dilemma: Warum die Länderspielpause für Blessin zum Problem wird" – kaum Verteidiger im Training). **An (a)s Stelle setzte ich gestern (c): Der Kölner Trainer stehe vor dem Derby zur Disposition. Heute fällt (c).**
***Was heute zu (c) steht – und es ist mit dem heutigen Datum in der Adresse belegt.*** **„Kein Trainer-Endspiel im Derby: Köln setzt weiter auf Wagner"** (`ms-aktuell.de/…wagner-koeln-trainer-**01-10-2026**/`). Inhalt: **Nach Sky Sport ist das Derby ausdrücklich kein Endspiel für René Wagner.** **Die sportliche Leitung und die zuständigen Gremien haben die Lage beraten und ihm das Vertrauen erneut ausgesprochen.** **Der Club hält an ihm fest, trotz des durchwachsenen Saisonstarts.** *Was bestehen bleibt:* **Bei einer Derby-Niederlage könnte es für ihn eng werden**, und **Horst Steffen (57, bis Februar 2026 bei Werder Bremen) wird weiter als Nachfolger genannt, mit dem man sich einig sei.** Ergänzend: **Wagner hat in elf Ligaspielen zwei Siege geholt.**
***Damit wäre der Weg zurück auf 2:1 frei – und er ist es nicht, weil heute eine zweite Fundstelle in die andere Richtung zeigt.*** **Gladbach hat das Blessin-Debüt gewonnen: 3:0 bei Sportfreunde Siegen**, Tore **Robin Hack** und **Shuto Machino**. **Und drei Spieler haben dort ihr erstes Spiel nach Verletzung bestritten: Daiki Hashioka, Yukhym Konoplya und Zento Uno.** **Das ist für zwei meiner offenen Fragen die Antwort:** **Konoplya** führte ich mit Innenband-Teilriss, **Uno** als „angeschlagen" mit zwei nicht auflösbaren Verletzungen – **beide haben gespielt.** **Kapitän Tim Kleindienst fehlte nur erkältet**, nicht verletzt. **Nächster Test: 03.10. bei St. Pauli.**
***Die Rechnung, die daraus folgt.*** **Gestern verlor Gladbach ein Argument (Vorbereitungszeit) und Köln bekam eines aufgebürdet (Trainerdebatte). Heute fällt Kölns Nachteil weg und Gladbach gewinnt drei Rückkehrer und ein Erfolgserlebnis.** **Die zwei neuen Fundstellen zeigen in entgegengesetzte Richtungen und sind etwa gleich schwer: eine mit heutigem Datum in der Adresse, eine mit einem belegten Spielergebnis.** **Sie heben sich auf.** **Was unverändert bleibt, ist die Säule (b)** – **bei Köln standen beim Wiedereinstieg nur zwölf Feldspieler zur Verfügung, die Abwehr war auf Borna Sosa, Sebastian Sebulonsen und Joel Schmied geschrumpft, acht U21-Talente mussten hochgezogen werden**, neun Profis sind auf Länderspielreise (**El Mala, Johannesson, Lochoshvili, Mensah, Okon-Engstler**), **Castro-Montes ist verletzt.**
***Und die Gegenrechnung, die mich bei 1:1 hält statt auf 1:2 zu gehen:*** **Gladbach hat in beiden Auswärtsspielen kein Tor erzielt** – **0:3 in Leipzig, 0:5 in Freiburg, 0:8** – und ist **Letzter mit 0 Punkten und 6:16.** **Ein 1:1 verlangt von Gladbach das erste Auswärtstor der Saison; ein Auswärtssieg verlangte zwei.** Weiter ausgefallen: **Enzo Leopold** (Kreuzbandriss, monatelang), **Nicolas Kühn** (mehrere Wochen), **Jens Castrop** (Schulter). Auf Kölner Seite bleibt die Offensive intakt: **Kamiński und El Mala waren an 21 Toren direkt beteiligt.**
***Warum 1:1 bleibt, in einem Satz:*** **Ein Gastgeber, dessen Trainerdebatte heute entschärft wurde, aber dessen Abwehr in dieser Pause nicht trainieren konnte, gegen einen Tabellenletzten, der auswärts noch nie getroffen hat, aber mit drei Rückkehrern und einem gewonnenen Test anreist.** **Ich habe diesen Tipp jetzt zweimal mit ausgetauschter Begründung gehalten. Wenn die dritte Begründung fällt, nehme ich ihn zurück und gehe auf 2:1 – das ist die Schwelle, die ich mir hiermit setze.**

### SC Freiburg – FC Schalke 04
**Sonntag, 11.10.2026, 17:30 Uhr** (Europa-Park-Stadion)
**Tipp: 2:0**
*unverändert*
***Freiburg ist die stabilste Mannschaft dieses Spieltags nach Dortmund:*** **10 Punkte, 12:3, Dritter, 3-1-0**, und **zu Hause 4:1 gegen Werder und 5:0 gegen Gladbach – zwei Heimspiele, neun Tore.** **Trainer ist Julian Schuster**, der die Länderspielnominierungen seiner Spieler ausdrücklich begrüßt hat; **die Mannschaft hat eine Woche Sonderurlaub bekommen.**
***Auf Freiburger Seite sind heute zwei Ausfälle belegt, die ich gestern nicht hatte:*** **Patrick Osterhage** (Knieprobleme) und **Max Rosenfelder** (Oberschenkelmuskel). **Dazu Florent Muslija, dessen Kreuzbandriss heute zum dritten Mal und ohne Gegenangabe belegt ist** – der Widerspruch von gestern ist damit gestrichen. **Drei Freiburger Ausfälle sind mehr als die zwei, von denen ich gestern ausging**, und das ist die einzige Bewegung gegen diesen Tipp.
***Auf Schalker Seite bleibt es bei zwei Langzeitfällen und einem Fragezeichen.*** **Justin Heekeren: Kreuzbandverletzung** – ein Torwartausfall, gestern mit „mindestens sechs Monaten" geführt. **Dejan Ljubičić** wird heute mit einer Ausfalldauer von **rund zwei Wochen und vier Tagen** geführt, **mit dem ausdrücklichen Zusatz, dass eine längere Pause droht** – **von heute an gerechnet endet das nach dem 11.10.**, sein Einsatz ist also weiter fraglich bis unwahrscheinlich. **Zu Robin Gosens habe ich heute erstmals ein Indiz, und es ist ein schwaches: Er wird im Kader für diese Partie geführt.** *Das ist keine Rückkehrmeldung*, und ich behandle es als Hinweis. **Trainer ist Miron Muslic** – seit 01.07.2025, Vertrag bis 2028, Aufstieg als Zweitligameister zwei Spieltage vor Schluss. **Damit ist auch diese Trainerlücke geschlossen.**
***Die Abwägung:*** **Schalke ist als Aufsteiger defensiv bemerkenswert – 3:4 Tore in vier Spielen, zwei Zu-null (0:0 gegen Bayern, 0:0 gegen Elversberg), nur vier Gegentore.** **Das ist das stärkste Gegenargument zu einem 2:0**, und es ist der Grund, warum ich bei zwei Toren bleibe und nicht höher gehe. **Dagegen steht die andere Hälfte derselben Bilanz: drei eigene Tore in vier Spielen, die schwächste Offensive der Liga.** **Eine Mannschaft, die kaum trifft, zu Gast bei einer, die zu Hause neun Tore in zwei Spielen erzielt hat und nur drei Gegentore in der ganzen Saison kassiert hat.** **2:0 bleibt: Freiburgs Heimstärke trägt die zwei Tore, Schalkes Offensivschwäche und der Torwartausfall tragen die Null.**

---

## Quellen

**Vorbemerkung:** Alle Quellen unten sind **Suchergebnis-Zusammenfassungen und -Titel**. Die Primärseiten waren aus dieser Umgebung nicht abrufbar (siehe Quellenlage). Wo eine Adresse ein Datum trägt, ist es mitgenannt, weil die Datierung in diesem Repo die Hauptarbeit ist.

**Spielplan und Länderspielpause**
- [anstosszeiten.de – 5. Spieltag Bundesliga 2026/27: Anstoßzeiten & alle 9 Spiele](https://anstosszeiten.de/bundesliga/spieltag-5/)
- [ruhrnachrichten.de – Länderspielpause: Dann geht es mit der Bundesliga weiter](https://www.ruhrnachrichten.de/service/bundesliga-fussball-fuenfter-spieltag-saison-2026-27-partien-mannschaften-uebertragung-w1251490-2002238953/)
- [sportschau.de – Darum dauert die Länderspielpause fast drei Wochen](https://www.sportschau.de/fussball/ab-montag-fast-drei-wochen-laenderspiele,laenderspiele-fenster-neu-100.html)
- [spox.com – Warum ist zwischen September und Oktober drei Wochen Länderspielpause?](https://www.spox.com/fussball/news/bundesliga-saison-2026-27-warum-ist-zwischen-september-und-oktober-drei-wochen-laenderspielpause/blt405fb3fe17574750)
- [zdfheute.de – Klopp hat nominiert – drei Wochen ohne Bundesliga: Was machen die Vereine?](https://www.zdfheute.de/sport/fussball-bundesliga/bundesliga-laenderspielpause-was-machen-die-klubs-100.html)
- [fussballnationalmannschaft.net (01.10.2026) – Fußball heute: Ergebnisse & Spiele am 1.10.2026](https://www.fussballnationalmannschaft.net/fussball-heute-am-1-10-2026-2-123300013.html)

**Schlotterbeck**
- [kicker.de – Im Abschlusstraining verletzt: Schlotterbeck fällt für beide Länderspiele aus – Bestätigung vom DFB](https://www.kicker.de/im-abschlusstraining-verletzt-schlotterbeck-faellt-fuer-beide-laenderspiele-aus-1257209/artikel)
- [bundesliga.com – Verletzung im Abschlusstraining: Schlotterbeck fehlt der DFB-Elf](https://www.bundesliga.com/de/bundesliga/news/dfb-schlotterbeck-nations-league-klopp-ausfall-verletzung-abschlusstraining-serbien-griechenland-39393)
- [neunzigplus.de – Schlotterbeck verletzt: Außenbandriss im Sprunggelenk, Aus für Serbien und Griechenland](https://neunzigplus.de/nationalmannschaften/umgeknickt-ohne-gegenspieler-schlotterbeck-faellt-aus-und-klopps-reha-plan-ist-endgueltig-gescheitert/)
- [ran.joyn.de – Diagnose steht fest: Schock um Nico Schlotterbeck](https://ran.joyn.de/sports/fussball/nations-league-a/nations-league-dfb-star-muss-nach-verletzung-im-abschlusstraining-abreisen-diagnose-steht-fest-194359)
- [ms-aktuell.de (30.09.2026) – Nico Schlotterbeck erneut verletzt: Sorge beim BVB nach DFB-Training](https://ms-aktuell.de/welt/schlotterbeck-verletzt-30-09-2026/)
- [sportschau.de – Schock für Klopp: Schlotterbeck fällt für beide Spiele aus](https://www.sportschau.de/fussball/nationalmannschaft/nico-schlotterbeck-faellt-womoeglich-wieder-aus,dfb-schlotterbeck-verletzt-100.html)
- [sport1.de – Schock um Schlotterbeck! BVB-Star reist von Nationalmannschaft ab](https://www.sport1.de/news/fussball/dfb-team/2026/09/dfb-team-bangt-um-einsatz-von-schlotterbeck)
- [fussballnationalmannschaft.net – DFB bestätigt Außenbandverletzung vor dem Serbien-Spiel](https://www.fussballnationalmannschaft.net/dfb-bangt-um-schlotterbeck-vor-serbien-spiel-2-123300481.html)
- [90min.de – Schlotterbeck-Schock beim BVB: Diese Alternativen hat Niko Kovac](https://www.90min.de/schlotterbeck-schock-beim-bvb-diese-alternativen-hat-niko-kovac)
- *Verworfen (andere Verletzungen):* [spox.com – „Damit muss man mindestens rechnen"](https://www.spox.com/fussball/listen/damit-muss-man-mindestens-rechnen-arzt-gibt-duestere-prognose-zur-ausfallzeit-von-nico-schlotterbeck-beim-bvb-ab/bltd4acecfbf3fedd8a) · [goal.com – „Nicht maximal schwerwiegend"](https://www.goal.com/de/listen/nicht-maximal-schwerwiegend-arzt-prognostiziert-genaue-ausfallzeit-von-nico-schlotterbeck-beim-bvb/bltd4acecfbf3fedd8a) · [fussballdaten.de – Experte prognostiziert monatelange BVB-Pause](https://www.fussballdaten.de/news/schlotterbeck-schock-experte-prognostiziert-monatelange-bvb-pause/) · [zdfheute.de – Schlotterbeck operiert, halbes Jahr Pause](https://www.zdfheute.de/sport/nico-schlotterbeck-verletzung-dortmund-100.html) · [bvbwld.de (25.06.2026) – Bittere Diagnose für den BVB](https://bvbwld.de/2026/06/25/bittere-diagnose-fuer-den-bvb-so-lange-faellt-schlotterbeck-wohl-aus/)

**Dortmund – Werder**
- [goal.com – Borussia Dortmund: Verletzungen, Sperren und die Aufstellung für das Spiel gegen Werder Bremen](https://www.goal.com/de/meldungen/borussia-dortmund-verletzungen-sperren-und-die-aufstellung-fuer-das-bundesligaspiel-gegen-werder-bremen/yveswfpnzjst16k7jfy54tu7k)
- [ran.joyn.de – Borussia Dortmund vs. Werder Bremen live: Alle Infos zum Bundesligaspiel am Freitagabend](https://ran.joyn.de/sports/fussball/bundesliga/borussia-dortmund-vs-werder-bremen-live-alle-infos-zum-bundesligaspiel-am-freitagabend-im-tv-livestream-und-ticker-192803)
- [ms-aktuell.de (29.09.2026) – BVB bangt um Ryerson nach erneutem Schlag auf die Rippen](https://ms-aktuell.de/welt/ryerson-verletzung-bvb-29-09-2026/)
- [footy.de (28.09.2026) – BVB bangt um Ryerson: Jetzt droht ein echtes Problem](https://footy.de/2026/09/28/bvb-bangt-um-ryerson-jetzt-droht-ein-echtes-problem)
- [fussballtransfers.com – Sorgen um Julian Ryerson](https://www.fussballtransfers.com/a613699149785842540-sorgen-um-ryerson)
- [deichstube.de – Vertragsgespräche stocken: Was wird aus aktuell verletztem Felix Agu?](https://www.deichstube.de/news/werder-bremen-vertragsgespraeche-stocken-was-wird-aus-felix-agu-bundesliga-transfers-vertrag-verhandlungen-zr-94442952.html)
- [weser-kurier.de – Werder Bremen: Vertragspoker um verletzten Felix Agu stockt](https://www.weser-kurier.de/werder/profis/werder-bremen-vertragspoker-um-verletzten-felix-agu-stockt-doc8757k5rzozthgd8238b)
- [deichstube.de – „Großes Risiko": Werder Bremens Verletzungssorgen in Zahlen](https://www.deichstube.de/news/werder-bremen-verletzungssorgen-gruende-umgang-konsequenzen-video-details-alarmierender-teufelskreis-zr-94240995.html)

**Augsburg – Bayern**
- [fcaugsburg.de – Manuel Baum bleibt Cheftrainer beim FCA](https://www.fcaugsburg.de/article/manuel-baum-bleibt-cheftrainer-beim-fca-23146)
- [kicker.de – Endgültige Dauerlösung: Baum bleibt FCA-Trainer](https://www.kicker.de/endgueltige-dauerloesung-baum-bleibt-fca-trainer-1218955/artikel)
- [sportschau.de – Offiziell: Manuel Baum bleibt Trainer des FC Augsburg](https://www.sportschau.de/regional/br/br-verkuendung-am-mittwochabend-baum-bleibt-fca-trainer-102.html)
- [ligaportal.at – Bis 2028: Baum bleibt Trainer in Augsburg](https://www.ligaportal.at/international/deutsche-bundesliga/90390-bis-2028-baum-bleibt-trainer-in-augsburg)
- [fcbinside.de (25.09.2026) – Verletzungsschock! Bayern muss wochenlang auf Musiala verzichten](https://fcbinside.de/2026/09/25/verletzungsschock-bayern-muss-wochenlang-auf-musiala-verzichten)
- [neunzigplus.de – Bayern-Spielplan Oktober: 9 Spiele, Musiala fehlt](https://neunzigplus.de/bundesliga/fc-bayern-oktober-spielplan-neun-spiele-musiala)
- [fussballdaten.de – Bayern bangt um Musiala: Reicht es bis zum BVB-Kracher?](https://www.fussballdaten.de/news/bayern-bangt-musiala-reicht-es-bvb-kracher/)
- [fussballdaten.de – Michael Gregoritsch ist verletzt: Bittere Nachricht für Augsburg](https://www.fussballdaten.de/news/bittere-nachricht-augsburg-gregoritsch-oesterreich-frueh-ausgewechselt/)

**Hoffenheim – HSV**
- [ms-aktuell.de (26.09.2026) – HSV muss mehrere Wochen auf Albert Grønbæk verzichten](https://ms-aktuell.de/welt/hsv-groenbaek-verletzung-26-09-2026/)
- [ligaportal.at – Faserriss: Hamburgs Topscorer Grönbaek fällt vorerst aus](https://www.ligaportal.at/international/deutsche-bundesliga/94138-faserriss-hamburgs-topscorer-groenbaek-faellt-vorerst-aus)
- [nurdieraute.de (30.09.2026) – Nächster Sturm-Ausfall? HSV-Profi verpasst Länderspiel verletzt](https://nurdieraute.de/2026/09/30/naechster-sturm-ausfall-hsv-profi-verpasst-laenderspiel-verletzt/)
- [footy.de (30.09.2026) – Nächster Sturm-Ausfall? HSV-Profi verpasst Länderspiel verletzt](https://footy.de/2026/09/30/naechster-sturm-ausfall-hsv-profi-verpasst-laenderspiel-verletzt)
- [90min.de – Engpass droht: Nächster HSV-Offensivspieler verletzt sich beim Nationalteam](https://www.90min.de/engpass-droht-nachster-hsv-offensivspieler-verletzt-sich-beim-nationalteam)
- [tsg-hoffenheim.de (09/2026) – Länderspiel-Update: Siege für Österreich-Duo und Kosovo-Trio](https://www.tsg-hoffenheim.de/aktuelles/news/2026/09/laenderspiel-update)
- [x.com/tsghoffenheim – Kramarić: kleiner operativer Eingriff im Leistenbereich](https://x.com/tsghoffenheim/status/2074770110737227954)
- *Verworfen (Saison 2025/26, falsche Richtung):* [kicker.de – HSV gegen Hoffenheim, Ticker](https://www.kicker.de/hsv-gegen-hoffenheim-2026-bundesliga-5051029/ticker) · [bundesliga.com – Hamburger SV vs. TSG Hoffenheim, Matchday 31, 2025/26](https://www.bundesliga.com/en/bundesliga/matchday/2025-2026/31/hamburger-sv-vs-tsg-hoffenheim/liveticker)
- *Verworfen (März 2026, frühere Pause):* [tsg-hoffenheim.de – Testspiel in der Länderspielpause: TSG trifft auf die SV Elversberg](https://www.tsg-hoffenheim.de/aktuelles/news/2026/03/testspiel-in-der-laenderspielpause-tsg-trifft-auf-die-sv-elversberg)

**Mainz – Leverkusen**
- [ligainsider.de – Mainz hofft auf Zentner-Rückkehr gegen Leverkusen](https://www.ligainsider.de/robin-zentner_3298/mainz-hofft-auf-zentner-rueckkehr-gegen-leverkusen-418162/)
- [sport1.de (09/2026) – Handverletzung: Mainz vorerst ohne Keeper Zentner](https://www.sport1.de/news/fussball/bundesliga/2026/09/handverletzung-mainz-vorerst-ohne-keeper-zentner)
- [fussballdaten.de – Mehrere Wochen Pause? Verletzungs-Update bei Mainz-Keeper Zentner](https://www.fussballdaten.de/news/mehrere-wochen-pause-verletzungs-update-mainz-keeper-zentner/)
- [torwart.de – FSV Mainz 05: Zentner fällt aus](https://www.torwart.de/magazin/torwartde-kompakt-25/26/bundesliga/fsv-mainz-05-zentner-faellt-aus.html)
- [spox.com – Mainz 05 v Bayer Leverkusen](https://www.spox.com/fussball/spiel/mainz-05-vs-bayer-leverkusen/194M9kHlhxVvu5vh1qSzt)

**Union – Elversberg**
- [kicker.de – Mauro Lustrinelli, Trainer, Bundesliga 2026/27, 1. FC Union Berlin](https://www.kicker.de/mauro-lustrinelli/trainer/bundesliga/2026-27/1-fc-union-berlin)
- [fc-union-berlin.de – Mauro Lustrinelli wird neuer Cheftrainer](https://www.fc-union-berlin.de/de/meldungen/meisterlicher-taktgeber-fuer-unions-maenner-mauro-lustrinelli-wird-neuer-cheftrainer-tCyufa)
- [sportschau.de – Schweizer Mauro Lustrinelli ist neuer Trainer des 1. FC Union](https://www.sportschau.de/regional/rbb/rbb-bundesliga-schweizer-mauro-lustrinelli-ist-neuer-trainer-des-1-fc-union-100.html)
- [fussballtransfers.com – Union Berlin vs. Elversberg, 5. Spieltag, Liveticker](https://www.fussballtransfers.com/spiel/6541569316757568931-1-fc-union-berlin-vs-sv-elversberg)
- [spox.com – Union Berlin v Elversberg](https://www.spox.com/fussball/spiel/union-berlin-vs-elversberg/reph0mesqzchHJAYAywE9)

**Paderborn – Stuttgart**
- [sport1.de (10/2026) – Paderborn siegt zum Abschluss der USA-Reise](https://www.sport1.de/news/fussball/bundesliga/2026/10/paderborn-siegt-zum-abschluss-der-usa-reise)
- [absolutfussball.com – Testspielsieg zum Abschluss: Was hinter dem besonderen USA-Trip des SC Paderborn steckt](https://www.absolutfussball.com/deutschland/sc-paderborn/sc-paderborn-laenderspiel-reise-usa-washington-dc-united-testspiel-werbetour-bundesliga-sieg-94519418.html)
- [ligainsider.de – Paderborn beendet USA-Reise mit Testspielsieg](https://www.ligainsider.de/sc-paderborn-07/1249/paderborn-beendet-usa-reise-mit-testspielsieg-418587/)
- [ligainsider.de – Erkältung bremst Paderborn-Quartett aus](https://www.ligainsider.de/laurin-curda_36261/erkaeltung-bremst-paderborn-quartett-aus-418599/)
- [scp07.de – Sportclub goes USA](https://www.scp07.de/Newsarchiv/Sportclub-goes-USA.html)
- [neunzigplus.de – VfB Stuttgart: Zagadou fällt nach Muskelverletzung mehrere Wochen aus](https://neunzigplus.de/bundesliga/vfb-stuttgart-zagadou-faellt-nach-muskelverletzung-mehrere-wochen-aus)
- [stuttgarter-nachrichten.de – VfB Stuttgart: Diagnose da, Dan-Axel Zagadou fällt aus](https://www.stuttgarter-nachrichten.de/sport/vfb-stuttgart-diagnose-da-dan-axel-zagadou-faellt-aus-79371608.html)
- *Als alt entlarvt (nennt Nagelsmann als Bundestrainer):* [stimme.de – VfB-Stars Stiller und Führich nachnominiert](https://www.stimme.de/sport/vfb-stuttgart/chris-fuehrich-angelo-stiller-nominierung-dfb-kader-verletzung-ausfall-nachruecker-bundestrainer-julian-nagelsmann-art-5154586)

**Leipzig – Frankfurt**
- [absolutfussball.com – Wer fehlt, wer kommt zurück? RB Leipzigs Hoffnungen und Sorgen vor dem Spiel gegen Frankfurt](https://www.absolutfussball.com/deutschland/rb-leipzig/rb-leipzig-personal-update-eintracht-frankfurt-rueckkehrer-verletzte-bundesliga-castello-lukeba-94519475.html)
- [rblive.de – RB Leipzigs lange Verletztenliste: Das sind die Gründe](https://rblive.de/spieler-trainer/rb-leipzigs-lange-verletztenliste-das-sind-die-gruende-3958868)
- [hessenschau.de – Eintracht Frankfurt in der Länderspielpause: Schwung holen für den Hütter-Fußball](https://www.hessenschau.de/sport/fussball/eintracht-frankfurt/eintracht-frankfurt-in-der-laenderspielpause-schwung-holen-fuer-den-huetter-fussball-v1,eintracht-laenderspielpause-104.html)
- [hessenschau.de – Eintracht-News-Ticker: 14 Profis auf Länderspielreise](https://hessenschau.de/sport/fussball/eintracht-frankfurt/eintracht-frankfurt-news-ticker-14-profis-auf-laenderspiel-reise,bundesliga-ticker-104.html)
- *Verworfen (falsche Richtung):* [onefootball.com – RB Leipzig to make late calls on Orban and Lukeba for Frankfurt trip](https://onefootball.com/de/news/rb-leipzig-to-make-late-calls-on-orban-and-lukeba-for-frankfurt-trip-42724526)

**Köln – Gladbach**
- [ms-aktuell.de (01.10.2026) – Kein Trainer-Endspiel im Derby: Köln setzt weiter auf Wagner](https://ms-aktuell.de/welt/wagner-koeln-trainer-01-10-2026/)
- [sportschau.de – Seit März im Amt: Entscheidung gefallen, Wagner bleibt Trainer des 1. FC Köln](https://www.sportschau.de/regional/wdr/wdr-entscheidung-gefallen-wagner-bleibt-trainer-des-1-fc-koeln-100.html)
- [gladbachtotal.de – Derby-Endspiel: Fliegt René Wagner bei Niederlage gegen Gladbach?](https://www.gladbachtotal.de/derby-endspiel-fliegt-rene-wagner-bei-niederlage-gegen-gladbach/)
- [koeln.t-online.de – 1. FC Köln: René Wagner vor Rauswurf? Trainer taucht am Geißbockheim auf](https://koeln.t-online.de/region/koeln/id_101425014/1-fc-koeln-rene-wagner-vor-rauswurf-trainer-taucht-am-geissbockheim-auf.html)
- [t-online.de – Borussia Mönchengladbach gewinnt Blessin-Debüt gegen Siegen](https://www.t-online.de/sport/fussball/bundesliga/id_101451798/borussia-moenchengladbach-gewinnt-blessin-debuet-gegen-siegen.html)
- [fohlen-hautnah.de – Borussia gewinnt Test in Siegen bei Blessin-Premiere](https://fohlen-hautnah.de/borussia-gewinnt-test-in-siegen-bei-blessin-premiere/)

**Freiburg – Schalke**
- [schwarzwaelder-bote.de – Erst Eintracht, dann Länderspielpause: Sechs Siege und vier Nationalspieler](https://www.schwarzwaelder-bote.de/sport/sc-freiburg/erst-eintracht-dann-laenderspielpause-sechs-siege-und-vier-nationalspieler-79478554.html)
- [schalketotal.de (23.09.2026) – Kuriose Maßnahme beim nächsten Schalke-Gegner: Freiburgs Belohnung vor dem S04-Duell](https://schalketotal.de/2026/09/23/kuriose-massnahme-beim-naechsten-schalke-gegner-freiburgs-belohnung-vor-dem-s04-duell/)
- [schalketotal.de (03.08.2026) – Schalke gibt Verletzungs-Update: So lange fehlen Gosens und Ljubicic](https://schalketotal.de/2026/08/03/schalke-gibt-verletzungs-update-so-lange-fehlen-gosens-und-ljubicic/)
- [fussballtransfers.com – Schalke bangt um Gosens & Ljubicic](https://www.fussballtransfers.com/a3289009428471900247-schalke-bangt-um-gosens)
- [zdfheute.de – Trainer der Fußball-Bundesliga 2026/27 im Überblick](https://www.zdfheute.de/sport/fussball-bundesliga-trainer-102.html)
- [kicker.de – Das sind die Bundesliga-Trainer der Saison 2026/27](https://www.kicker.de/das-sind-die-bundesliga-trainer-der-saison-2026-27-902978/slideshow)
