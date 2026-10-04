# Bundesliga-Tipps – 5. Spieltag 2026/27 (Stand: 04.10.2026)

**Ansetzung:** Freitag, 09.10. bis Sonntag, 11.10.2026. Der Vortagsstand (03.10.) betraf denselben Spieltag – **alle neun Tipps sind vergleichbar.**

**Vierzehnter und letzter voller Tag der Länderspielpause (21.09.–06.10.2026).** Bis zum Anpfiff sind es 5 Tage. **Die Nationalmannschaft hat heute in Thessaloniki 0:0 gegen Griechenland gespielt** – damit ist das Länderspielfenster für das DFB-Team beendet, die Vereine bekommen ihre Spieler ab Montag zurück. **Der FC Bayern nimmt das Mannschaftstraining ausdrücklich erst am 06.10. wieder auf.**

**Heute ändert sich ein Tipp: Köln – Gladbach von 1:1 auf 1:0.** Auslöser ist eine Vereinsmeldung, nicht eine Vorschau: **Franck Honorat hat sich im Training eine Muskelverletzung zugezogen, fällt „auf unbestimmte Zeit" aus und verpasst das Derby.** Sein nominaler Ersatz Nicolas Kühn ist weiter mit Muskelbündelriss außer Gefecht. **Ein Gast, der auswärts noch kein Tor erzielt hat, verliert vor dem Spiel den nächsten Offensivspieler** – Details und die Auflösung meiner selbstgesetzten Schwelle unten.

**Die zweite große Meldung des Tages bestätigt nur, was gestern schon stand, aber jetzt partiebezogen:** **Beide Kölner Mittelstürmer fallen für den 11.10. aus** – Dallinga mit Kreuzbandverletzung über Monate, Ache mit Oberschenkelverletzung „vorerst". **Voraussichtlich spielt Marius Bülter im Sturmzentrum.**

**Fünf meiner acht unveränderten Tipps sind heute besser belegt als gestern, zwei Schwellen sind erfüllt bzw. erledigt, und sechs heutige Fundstellen habe ich verworfen** – darunter eine komplette Leipziger Ausfallliste, die aus der Vorsaison stammt, und eine Anstoßzeiten-Liste, die in UTC rechnet.

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Die Primärseiten sind aus dieser Umgebung weiterhin nicht abrufbar.** Heute einzeln geprüft:

- **WebFetch** auf `bundesliga.com` und `anstosszeiten.de` → beide Male `EGRESS_BLOCKED` mit namentlicher Nennung der Domain.
- **Direkte Verbindungsprüfung** auf acht Sportdomains (`kicker.de`, `www.kicker.de`, `transfermarkt.de`, `weltfussball.de`, `anstosszeiten.de`, `ran.joyn.de`, `sport1.de`, `sportschau.de`) → **alle acht mit HTTP-Status `000`**, also kein Verbindungsaufbau.

**Der Agent-Proxy ist heute im Gegensatz zu gestern prüfbar und gesund:** Der Statusaufruf ist durchgelaufen, `enabled: true`, `recentRelayFailures: []`, `bundleCoversEveryHost: true`. **Das schließt einen TLS- oder Proxyfehler aus und bestätigt die Diagnose: Es ist die Netzwerk-Policy der Umgebung, die diese Domains sperrt.** Die Gegenprobe, die gestern fehlte, liegt damit wieder vor.

**Alles unten steht deshalb auf Suchergebnis-Zusammenfassungen und -Titeln, nicht auf gelesenen Artikeln.** Wo eine Adresse ein Datum trägt, nenne ich es mit, weil die Datierung in diesem Repo die Hauptarbeit ist. **Vereinsmeldungen kann ich weiterhin nicht im Volltext prüfen** – daran scheitert heute erneut die Zentner-Schwelle (Mainz – Leverkusen), und daran hängt die Unsicherheit bei der Kölner Sturmaufstellung.

## Korrekturen und Auflösungen am Vortagsstand

### 1. Ryerson: der Gegner-Widerspruch von gestern ist aufgelöst – es war keine Entweder-oder-Frage

Gestern stand hier als Korrektur 5: zwei datierte Adressen nennen Norwegens **1:2 gegen Wales** als das Spiel, in dem Ryerson in der 16. Minute ausgewechselt wurde; eine dritte nennt **Portugal**. Ich habe mich für Wales entschieden und den Widerspruch offen gelassen.

**Heute liegt die Kette in einer Fundstelle zusammen, und sie löst beide Varianten auf, statt eine zu verwerfen:** **Ryerson bekam den Schlag auf die Rippengegend im Nations-League-Spiel gegen Dänemark; im Spiel gegen Portugal wurde dieselbe Stelle bei einem Zusammenprall erneut getroffen; im 1:2 gegen Wales verstärkte ein Zweikampf früh in der Partie den Schmerz so, dass er nach rund 16 Minuten raus musste.** **Drei Spiele, eine Verletzung, keine widersprüchlichen Angaben – mein gestriger Widerspruch war ein Lesefehler meiner Seite, nicht ein Fehler der Quellen.**

**Und die eigentliche Neuigkeit ist eine Entwarnung mit Einschränkung:** **Nach kicker-Informationen ist bei der Rippenverletzung kein Langzeitausfall zu erwarten, sein Einsatz am Freitag gegen Werder ist aber unsicher.** **Das ist die erste belastbare Einordnung seit vier Läufen.** Eine Diagnose gibt es weiterhin nicht.

### 2. Maluze (Frankfurt): meine eigene Einschränkung von gestern hat sich als die richtige erwiesen

Gestern habe ich die Änderung auf 2:1 unter anderem darauf gestützt, dass **Maluze in einer taktischen Vorschau als eine von zwei Optionen für die rechte Position der Dreierkette genannt wurde** – und ausdrücklich dazugeschrieben: „**Das ist eine Nennung durch einen Berichterstatter in einer taktischen Vorschau, kein Hütter-Zitat zu Maluzes Gesundheit. Die Säule ist also nicht umgefallen, sie ist angeschlagen.**"

**Heute ist sie wieder aufgerichtet:** Eine Fundstelle zum Hütter-Personalgrübeln hält fest, **Maluze sei weiter im Reha-Training und damit nicht einsatzfähig** – er könne nicht um einen Startelfplatz neben Robin Koch und Lilian Brassier konkurrieren. **Maluze steht ab heute wieder als Ausfall.** **Für den Tipp ändert das nichts** (siehe unten), **aber es ist der zweite Tag in Folge, an dem eine Vorschau-Nennung von einer trainerbezogenen Fundstelle korrigiert wird.** Die Lehre ist dieselbe wie bei Sebulonsen und Tella: **Eine Namensnennung in einer Aufstellungsprognose ist kein Gesundheitsbefund.**

### 3. Vuskovic (HSV): ein Ausfall, den ich in fünf Läufen nie geführt habe – und der nichts ändert

Eine heutige Sperrenabfrage nennt **Mario Vuskovic (HSV) als gesperrt bis zum 15.11.2026**. Nachrecherche: **Der CAS hat die DFB-Sperre von zwei auf vier Jahre erhöht (EPO), rückdatiert auf die vorläufige Sperre vom 15.11.2022; damit endet sie am 15.11.2026.** **Er kann am 10.10. nicht spielen.**

**Ich schreibe es hin, weil es in meinen Läufen fehlte – und sage im gleichen Atemzug, dass es kein neuer Vorgang und für den Tipp ohne Gewicht ist:** Er stand in keinem Lauf als verfügbar in meiner Rechnung. **Ein Widerspruch bleibt offen:** eine t-online-Überschrift meldet ihn „zurück im HSV-Training: 1.404 Tage Dopingsperre enden". **1.404 Tage ab dem 15.11.2022 ergeben den 19.09.2026, nicht den 15.11.2026.** Die plausible Auflösung – Trainingserlaubnis vor Ablauf der Spielsperre – kann ich nicht belegen. **Spielberechtigt ist er am 10.10. nach beiden Lesarten nicht.**

### 4. Der Elversberg-Test bleibt beim 02.10. – heute zum zweiten Mal gegen eine Falschdatierung

Gestern habe ich eine Fundstelle verworfen, die das Elversberger 3:2 bei Hoffenheim auf „**Freitag, 3. Oktober 2026**" datiert, weil der 03.10.2026 ein Samstag ist. **Heute schreiben zwei weitere Fundstellen dasselbe Datum, eine davon die Vereinsseite in der Zusammenfassung.** **Die Rechnung bleibt dieselbe: Der 03.10.2026 ist ein Samstag, der 02.10.2026 ein Freitag.** Ich bleibe beim **02.10.** und zähle die Partie weiterhin einfach.

*Neu und unstrittig aus derselben Abfrage, und es deckt sich mit meinem Vortagsstand:* **Hoffenheims eigene Seite führt die Partie als verlorenen Test**, und die Einordnung „**gemischte Elf aus Erstliga- und U23-Spielern, 18 von 27 Profis abgestellt**" ist heute aus zwei Richtungen bestätigt.

## Heute ausdrücklich verworfene Fundstellen

**1. Die Leipziger Ausfallliste, die aus der Vorsaison stammt – und das ist die wichtigste Verwerfung des Tages.** Eine Vorschau-Zusammenfassung zu Leipzig – Frankfurt führt heute: **Kapitän Willi Orbán mit muskulären Problemen, Einsatz „mehr als fraglich"; Xaver Schlager gesperrt; Ezechiel Banzuzi mit Knieverletzung aus dem Training; Lukeba mit Adduktorenproblemen nicht verfügbar.** **Das wären vier Ausfälle in Abwehr und Zentrum und ein schwerer Schlag für meinen Tipp.**

**Die Quelle dieser Aufzählung ist ein Kaderupdate „ahead of #RBLFCU" – also vor einem Leipziger Spiel gegen Union Berlin.** **Leipzig hat in dieser Saison noch nicht gegen Union gespielt** (1.–4. Spieltag: Gladbach, Bremen, HSV, Leverkusen). **Die Liste gehört in die Vorsaison.** Das bestätigt sich aus ihrem eigenen Inhalt: In derselben Mitteilung steht **Orbán als „fully fit to play Union"** und **Schlager als „available again after serving his suspension"** – beides das Gegenteil dessen, was die Zusammenfassung daraus macht. **Verworfen, vollständig.**

*Zweite, unabhängige Gegenprobe:* **Orbán war in diesem Fenster bei der ungarischen Nationalmannschaft** – gestern belegt mit der Angabe, dass Raum, Orbán und Nusa erst zu Beginn der kommenden Woche zurückkehren. **Ein Spieler, der mit muskulären Problemen das Leipziger Training verpasst, ist nicht gleichzeitig abgestellt.**

**2. Laimer (Bayern), zum dritten Mal.** Eine heutige Fundstelle schreibt, **Laimer bleibe während der Pause in München, um sein individuelles Reha-Programm fortzusetzen.** **Dagegen stehen zwei datierte Fundstellen vom 28.09.: „voll fit und bereit", Rückkehr ins Mannschaftstraining, Reise zur Nationalmannschaft.** Auch die beiden Meldungen desselben Dienstes sind in dieser Reihenfolge lesbar: „Rehabbing at Säbener Straße during break" trägt die kleinere, „Returns to full training" die größere Meldungsnummer. **Ich führe Laimer weiter nicht als Ausfall** (so schon am 02.10. und 03.10.). **Das ist das dritte Mal, dass derselbe veraltete Stand in einer neuen Abfrage auftaucht.**

**3. Die Anstoßzeiten in UTC.** Eine Zusammenfassung nennt für **sechs Samstagsspiele 13:30 Uhr** und für **Leipzig – Frankfurt 16:30 Uhr**, lässt aber **Dortmund – Werder bei 20:30** und **Köln – Gladbach bei 15:30** stehen. **Das ist keine andere Ansetzung, das ist dieselbe in UTC, und zwar nur zur Hälfte umgerechnet** – 15:30 MESZ sind 13:30 UTC, 18:30 MESZ sind 16:30 UTC, und wären es echte Ortszeiten, müssten Köln und Dortmund mitwandern. **Verworfen.** **Vier heutige Fundstellen nennen unabhängig voneinander 15:30 für Mainz – Leverkusen, Union – Elversberg, Paderborn – Stuttgart und Köln – Gladbach, 18:30 für Leipzig – Frankfurt und 17:30 für Freiburg – Schalke.** Meine Zeiten bleiben.

**4. Die Schalker Ausfallliste, die zwei Spieler der gestrigen Startelf als verletzt führt.** Eine heutige Liste nennt für Schalke **Ljubičić, Gülasi, Lasme und Gantenbein** als Ausfälle. **Lasme und Gantenbein standen gestern in der namentlich belegten Startelf beim 1:0 in Austria Lustenau** (Karius – Gantenbein, Kurucay, V. Becker – Dina Ebimbe, Schallenberg, Vozar, Gosens – Lasme, Karaman – Sylla). **Nach meiner eigenen, am 02.10. gesetzten Regel schlägt der datierte Spielbericht den Listeneintrag.** **Lasme und Gantenbein bleiben verfügbar; Gülasi übernehme ich nicht als belegt.** **Das ist in fünf Läufen das fünfte Mal, dass ein Aggregator-Listeneintrag an einem Spielbericht zerbricht.**

**5. Die deutsche Niederlage gegen Griechenland.** In derselben Trefferliste wie das heutige 0:0 stehen zwei Überschriften, die eine **deutsche Niederlage** gegen Griechenland melden. **Der Spielbericht zum heutigen Abend nennt 0:0, ein in der 32. Minute zurückgenommenes Tor von Burkardt und fünf Punkte aus vier Gruppenspielen; eine weitere Fundstelle formuliert „Deutschland kann Griechenland erneut nicht knacken".** **Das „erneut" verweist auf das frühere Duell dieser Gruppe – dorthin gehören die Niederlagen-Überschriften.** **Ich verwende 0:0.**

**6. Die Mainzer und Leverkusener Listeneinträge, zum sechsten Lauf.** Für Mainz stehen erneut **Kohr (nach Operation)** und **Silas (Schien- und Wadenbeinbruch)**, für Leverkusen **Doué (Wadenmuskel)** und **Eichhorn (Stoffwechselerkrankung)** – **dieselben vier, seit Läufen stabil mit Diagnose, die übernehme ich.** **Katompa Mvumpa, Caci und Culbreath übernehme ich weiter nicht als belegt.**

## Offen benannte Restlücken und Unsicherheiten

- **Ryersons Diagnose ist weiter nicht veröffentlicht.** Neu ist die kicker-Einordnung „kein Langzeitausfall", neu ist auch „Einsatz am 09.10. unsicher". **Beides ist eine Einordnung, keine Diagnose.** Die Frage bleibt offen, aber sie ist kleiner als gestern.
- **Schlotterbecks Ausfalldauer ist weiterhin keine Vereinsangabe.** „Zwei bis drei Wochen" bleibt Ersteinschätzung; heute erneut bestätigt, dass **weder DFB noch BVB eine Dauer genannt haben** und der Einsatz am 09.10. gefährdet ist.
- **Aches Ausfalldauer ist unbekannt.** Der Verein sagt „vorerst". Belegt sind Diagnose (Oberschenkel-Muskelverletzung) und das Ausfallen für das Derby, nicht die Dauer.
- **Wer bei Köln am 11.10. im Sturmzentrum spielt, ist eine Prognose.** „Bülter voraussichtlich, Waldschmidt möglicherweise umgestellt" stammt aus Vorschauen, nicht vom Verein. **Das ist die Lücke, auf der meine heutige Änderung zur Hälfte ruht, und ich benenne sie als deren Schwachstelle.**
- **Zentner: dritter Lauf ohne Vereinsangabe – und heute ohne jede neue Fundstelle.** Gestern gab es wenigstens „weiter im Individualtraining"; heute nichts. **Meine Schwelle ist damit nicht ausgelöst, sondern unberührt.**
- **Kramarić und Coufal: heute keine neue partiebezogene Nennung gefunden.** Die „angeschlagen"-Angabe für den 10.10. ist damit einen Tag alt und unaktualisiert. Was heute auftauchte, ist ausdrücklich **Vorgeschichte** (Kramarićs Leisten-Operation nach der WM, Coufals Abstellungen) **und kein aktueller Stand – ich verwende es nicht.** **Hoffenheim bleibt die dünnste Informationslage des Spieltags.**
- **Unions Testspiel beim BAK 07: dritter Lauf, kein Ergebnis auffindbar.** Ob es stattgefunden hat, weiß ich weiterhin nicht.
- **Paderborns USA-Reise und das 1:0 bei D.C. United am 01.10. stehen nur auf Suchzusammenfassungen.** Die Vereinsseite ist nicht lesbar, das Datum habe ich nicht gegengeprüft. **Ich verwende es, weil es den seit zwei Läufen offenen Erkältungspunkt schließt, und markiere es als einfach belegt.**
- **Die dritte Leipziger Niederlage bleibt unzuordenbar – vierter Lauf mit derselben Lücke.** Heute kam dazu nichts Neues.
- **Leverkusens Trainername ist in zwei heutigen Fundstellen verschieden** (Hjulmand in einer älteren, „Carles Martínez" im Bericht zum 6:0). **Für keinen Tipp relevant, aber ungeklärt – ich nenne ihn deshalb unten nicht.**
- **Die Tabelle ist aus den einzeln belegten Ergebnissen gerechnet**, weil keine Tabellenseite abrufbar ist. Seit dem 20.09. wurde nicht gespielt. *Heute gegengeprüft:* **Eine Fundstelle führt Freiburg als Dritten und Schalke als Elften – beides stimmt mit meiner Rechnung.** Damit sind nach Paderborn, Stuttgart und der Leipzig-Zeile **fünf Zeilen extern bestätigt.** *Dieselbe Fundstelle schreibt allerdings „nach fünf Spieltagen ungeschlagen" – gespielt sind vier.* Die Platzierung übernehme ich, die Spieltagszahl nicht.

### Tabelle nach dem 4. Spieltag

Aus den einzeln belegten Ergebnissen gerechnet. **Form = 1. bis 4. Spieltag von links nach rechts.** Werte unverändert zum Vortag – seit dem 20.09. wurde nicht gespielt. **Heute erstmals gegengeprüft: Platz 3 (Freiburg) und Platz 11 (Schalke).**

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

**Heim- und Auswärtszahlen, die mehrere Tipps tragen:**

- **Dortmund zu Hause:** 2:0 gegen HSV, 3:0 gegen Paderborn – **zwei Spiele, zwei Zu-null, fünf Tore.**
- **Leipzig zu Hause:** 3:0 gegen Gladbach, 5:0 gegen HSV – **8:0 in zwei Spielen, zwei Zu-null; bei beiden stand Lukeba in der Startelf.**
- **Frankfurt auswärts:** 3:3 bei Union, 3:1 in Mainz – **vier Punkte, 6:4; auswärts besser als zu Hause, aber ohne Auswärtssieg.**
- **HSV auswärts:** 0:2 in Dortmund, 0:5 in Leipzig – **zwei Spiele, null Tore.** Beide HSV-Tore fielen zu Hause.
- **Gladbach auswärts:** 0:3 in Leipzig, 0:5 in Freiburg – **null Tore, 0:8.** **Das ist die Zahl, die meine heutige Änderung trägt.**
- **Köln zu Hause:** 3:2 gegen Hoffenheim, 1:1 gegen Werder – **vier Punkte, 4:3 in zwei Spielen.**
- **Stuttgart auswärts:** 1:5 in München, 1:2 in Hoffenheim – **null Punkte, 2:7.**
- **Paderborn zu Hause:** 0:0 Mainz, 0:1 Freiburg, 3:1 Hoffenheim – **vier Punkte, drei Saisontore insgesamt.**
- **Freiburg zu Hause:** 4:1 Werder, 5:0 Gladbach – **zwei Spiele, neun Tore.**
- **Mainz zu Hause:** 0:0 Paderborn, 1:3 Frankfurt – **ein Punkt, 1:3.** **Leverkusen auswärts:** 2:3 in Elversberg, 2:2 in Augsburg – **ein Punkt, 4:5, kein Auswärtssieg.**
- **Augsburg zu Hause:** 3:0 Schalke, 2:2 Leverkusen – **fünf Tore in zwei Spielen.**
- **Bayern:** 14:2 in vier Spielen – **zwei Gegentore in der ganzen Saison.**

---

## Die Tipps zum 5. Spieltag

### Borussia Dortmund – SV Werder Bremen
**Freitag, 09.10.2026, 20:30 Uhr** (Signal Iduna Park)
**Tipp: 3:1**
*unverändert*

***Die wichtigste heutige Information zu dieser Partie geht gegen meinen Tipp, und ich stelle sie voran.*** **Nach kicker-Informationen ist bei Ryersons Rippenverletzung kein Langzeitausfall zu erwarten** (Korrektur 1). **Das ist eine Entwarnung – aber eine halbe:** derselbe Stand nennt **seinen Einsatz am Freitag ausdrücklich unsicher**, und eine Diagnose ist weiterhin nicht veröffentlicht. **Für die rechte Abwehrseite gibt es im Kader keine adäquate Alternative; genau das war gestern der Grund, das Gegentor im Tipp zu lassen, und es ist es heute noch.**

***Dortmunds Ausfälle, unverändert, mit einem heute neuen Detail zur Innenverteidigung.*** **Nico Schlotterbeck: Außenbandverletzung im rechten Sprunggelenk, zugezogen am 30.09. im DFB-Training in Herzogenaurach, Ersteinschätzung zwei bis drei Wochen (nicht offiziell, heute erneut bestätigt als Einschätzung), Einsatz am 09.10. gefährdet.** **Dazu unverändert: Emre Can (Kreuzbandriss), Justin Lerma, Filippo Mane, Giannis Konstantelias.** **Die Innenverteidigung ist mit Waldemar Anton und Joane Gadou besetzt.**

*Neu und für genau diese Lücke relevant:* **Kauã Prates wurde bei Brasilien in der Innenverteidigung eingesetzt, Daniel Svensson bei Schweden auf der rechten Seite.** **Zwei Dortmunder Verteidiger haben in der Pause auf fremden Positionen gespielt – ausgerechnet auf den beiden, die durch Schlotterbeck und Ryerson offen sind.** **Das ist kein Ersatz, aber es verkleinert das Risiko, dass Kovač improvisieren muss, ohne eine Option gesehen zu haben.** **Einen BVB-Test in dieser Pause habe ich erneut nicht gefunden, und heute weiß ich, warum: 20 Profis waren abgestellt, in Dortmund blieben nur Beier, Sabitzer, Kaba und Ersatztorhüter; Kovač hat den Rest freigegeben und das Mannschaftstraining ausgesetzt.**

***Werders Lage, und sie ist heute im Wortlaut härter als gestern.*** Das 0:7 im Test bei Twente Enschede liegt jetzt mit Verlauf vor: **Twente führte nach einer Viertelstunde 3:0, zur Pause 6:0.** **Thiounes Satz dazu: „Ich habe dafür absolut kein Verständnis und null Akzeptanz."** **Der freie Tag wurde gestrichen, stattdessen gemeinsame Analyse.** *Das Gegenargument von gestern bleibt stehen und wird dadurch nicht kleiner:* **Ein Trainer, der so reagiert, erzeugt die Spannung, aus der Auswärtsüberraschungen entstehen** – und **Werder fehlten in Enschede 17 Akteure, es war keine Bundesliga-Elf.**

***Was Werder belegt fehlt, unverändert:*** **Jens Stage** (Oberschenkel, restliches Kalenderjahr), **Justin Njinmah** (Oberschenkelmuskelverletzung, monatelang), **Salim Musah** („ab dem neuen Jahr"), **Keke Topp** (Kreuzbandriss), **Senne Lynen**, **Moussa Ndiaye.** *Die zwei Gegenargumente ebenfalls unverändert, heute erneut belegt:* **Eren Dinkci ist nach Krankheit zurück im Mannschaftstraining**, **Felix Agu hat nur das Aufwärmen mitgemacht und danach individuell auf dem Nebenplatz trainiert – er könnte in Dortmund erstmals wieder im Kader stehen.** **Deshalb nicht 4:1 und nicht 3:0.**

***Warum 3:1 bleibt, in einem Satz:*** **Ein Tabellenführer mit zwei Heim-Zu-null und fünf Heimtoren gegen eine Mannschaft mit sechs belegten Ausfällen, drei davon in der Offensive, die gerade 0:7 verloren hat – und ein Gegentor, weil Dortmund rechts und zentral hinten improvisieren muss.**

***Die Schwelle für den nächsten Lauf:*** **Wird Ryerson belegt fit gemeldet oder Schlotterbecks Rückkehr vom Verein angekündigt, gehe ich auf 3:0. Fällt zusätzlich ein Dortmunder Innenverteidiger aus, gehe ich auf 2:1.**

### FC Augsburg – FC Bayern München
**Samstag, 10.10.2026, 15:30 Uhr** (WWK Arena)
**Tipp: 1:2**
*unverändert* — **und heute mit den ersten neuen Informationen zu dieser Partie seit zwei Läufen.**

***Gestern musste ich hinschreiben, dass es zu dieser Partie keine einzige neue, belastbare Information gab. Heute sind es zwei, und sie wirken gegeneinander.***

**Erstens, Augsburgs Test liegt jetzt mit Ergebnis vor: 2:2 gegen Hertha BSC am 02.10., 13:00 Uhr, auf dem Gelände der Paul-Renz-Akademie, unter Ausschluss der Öffentlichkeit.** **Augsburg führte nach einer starken Phase in der zweiten Halbzeit 2:0, dann glich Luca Schuler mit zwei Toren für den Zweitligisten aus.** **Der Trainer hat rotiert, vier Nachwuchsspieler standen im Kader (Adleff, Exner, Selimovic, Jäger).** *Für den Tipp lese ich das vorsichtig:* **Eine 2:0-Führung gegen einen Zweitligisten herzugeben, ist kein gutes Zeichen – aber bei Rotation und vier A-Jugendlichen im Kader ist es auch kein Befund über die Bundesliga-Elf.** **Es bestätigt immerhin, dass Augsburg zu Hause trifft, und das ist die eine Zahl, die mein Tipp von Augsburg verlangt.**

**Zweitens, Bayern nimmt das Mannschaftstraining erst am 06.10. wieder auf.** **Die offizielle Spielvorbereitung beginnt damit vier Tage vor dem Anpfiff**, weil ein großer Teil des Kaders bis zum Ende des Fensters abgestellt ist. *Das ist ein Argument gegen Bayern, und es ist auch eines für eine engere Partie – aber es ist kein neues: Diese Lage hat Bayern in jeder Länderspielpause.*

***Der Personalstand, unverändert.*** **Augsburg: Steve Mounié** (rund zwei Monate, im Aufbau), **Anton Kade fraglich** (leichter Muskelbündelriss in den Adduktoren, Individualprogramm; der Hertha-Test kam für ihn ausdrücklich zu früh – heute erneut als „fraglich" bestätigt), **Juma Bah offen**, **Gregoritsch verfügbar.** **Bayern: genau ein Ausfall – Jamal Musiala**, Muskelfaserriss im rechten Oberschenkel, nach Sky drei bis vier Wochen, **fehlt definitiv gegen Augsburg** (heute erneut bestätigt). **Konrad Laimer führe ich weiter nicht als Ausfall** (Verworfene Fundstellen, Punkt 2).

***Warum 1:2 und nicht 0:2, nicht 1:3, nicht 2:2 – unverändert.*** **Augsburg hat in zwei Heimspielen fünf Tore erzielt und steht mit 7 Punkten und 11:6 auf Platz 4** – ein Tor ist die Mindestzahl, die zu dieser Reihe passt. **Bayern hat in vier Spielen zwei Gegentore kassiert** – mehr als ein Tor ist gegen diese Abwehr nicht zu begründen. **Und Musialas Ausfall ist bei dieser Kaderdecke genau ein Tor wert.** **1:2 bleibt.**

***Die Schwelle für den nächsten Lauf:*** **Nur ein zweiter belegter Bayern-Ausfall mit Diagnose bewegt diesen Tipp auf 2:2. Eine Kade-Entwarnung bewegt ihn nicht, weil Augsburgs Tor im Tipp schon drin ist.**

### TSG Hoffenheim – Hamburger SV
**Samstag, 10.10.2026, 15:30 Uhr** (SNP Arena)
**Tipp: 2:0**
*unverändert* — **und der HSV-Test, auf dessen Ergebnis ich gestern ausdrücklich verwiesen habe, liegt heute vor. Er stützt den Tipp, statt ihn zu kippen.**

***Das Ergebnis zuerst, und dann die Minuten.*** **Der HSV hat heute 2:0 (0:0) gegen den FC Kopenhagen gewonnen, vor 55.067 Zuschauern im Volksparkstadion, unter Merlin Polzin.** **Kofi Amoako traf in der 83. Minute nach einer Hereingabe des eingewechselten Kelvin Ojo; Nicolai Remberg köpfte in der 89. oder 90. nach einem Freistoß von Bilal Nadir das 2:0** (die Fundstellen weichen in der Minute ab). **Die Fundstellen führen die Partie als „Test unter Freunden".**

**Das ist zwei Tore mehr, als der HSV in dieser Saison auswärts in der Liga erzielt hat – und genau deshalb ändert es den Tipp nicht:** **Beide Treffer fielen nach der 82. Minute, einer von einem Einwechselspieler, einer von einem Mittelfeldspieler nach Standard.** **Eine Mannschaft, die im Heim-Freundschaftsspiel bis zur 83. Minute gegen einen dänischen Erstligisten kein Tor erzielt, belegt meine Begründung, sie widerlegt sie nicht.**

***Die HSV-Sturmnot ist heute namentlich und zum vierten Mal bestätigt – und eine Fundstelle überschreibt sie direkt mit „Sturm-Not an der Elbe: HSV gehen vor Kopenhagen-Test die Angreifer aus".***
- **Patson Daka: Muskelfaserriss, Oberschenkel, mehrere Wochen**, zugezogen in Sambias 1:3 gegen Algerien am 02.10.
- **Albert Grønbæk: Muskelfaserriss rechter Oberschenkel, drei bis vier Wochen**, Hoffnung erst auf den 17.10. – **er ist der Topscorer des HSV.**
- **Terem Moffi: Knieprobleme, nicht voll belastbar**, hat heute gegen Kopenhagen gefehlt.
- **Mario Vuskovic: gesperrt bis 15.11.2026** (Korrektur 3) – **kein neuer Vorgang, aber jetzt belegt.**

***Und die eine Meldung, die heute gegen den Tipp hätte sprechen können, ist entschärft – vom Spieler selbst.*** **Yussuf Poulsen musste nach 20 Minuten raus, nach einem Schlag zwischen Knie und Wade, und hat selbst um die Auswechslung gebeten.** **Danach hat er Entwarnung gegeben: „Gegen Hoffenheim bin ich wieder dabei."** **Er konnte kurz vor der Auswechslung noch sprinten, was für eine Vorsichtsmaßnahme spricht; die kicker-Überschrift lautet „Poulsen muss raus und gibt Entwarnung".** **Ich führe ihn als verfügbar.** *Das heißt aber auch:* **Polzin hat nach aktuellem Stand zwei fitte Mittelstürmer, Poulsen und den jungen Otto Stange – und einer davon hat heute 20 Minuten gespielt und einen Schlag bekommen.**

***Die Gegenrechnung, und sie ist heute kleiner als gestern, weil sie nicht nachgeliefert wurde.*** **Kramarić und Coufal standen gestern zum dritten Mal als „angeschlagen" für den 10.10. – heute habe ich dazu keine neue partiebezogene Fundstelle gefunden.** **Keine Entwarnung, keine Verschärfung, keine Diagnose.** Was heute auftauchte, ist Vorgeschichte (Kramarićs Leisten-Operation, Coufals Abstellungen) und **kein aktueller Stand – ich verwende es nicht.** **Kramarić bleibt das Risiko dieses Tipps, und er ist es heute unverändert und unaktualisiert.** **Hoffenheims einziger Formdatenpunkt der Pause bleibt das 2:3 gegen Elversberg vom 02.10., entschärft durch die gemischte Elf und 18 abgestellte Profis** (Korrektur 4).

***Warum 2:0 bleibt, in einem Satz:*** **Ein Heimteam, das zu Hause vier Tore in zwei Spielen erzielt hat, gegen einen Gast, dem drei Angreifer namentlich und diagnostisch fehlen, der auswärts noch kein Tor erzielt hat und der heute im eigenen Stadion bis zur 83. Minute keines geschafft hat.**

***Die Schwelle für den nächsten Lauf:*** **Wird Kramarić oder Coufal belegt als Ausfall gemeldet, gehe ich auf 1:0. Kommt ein HSV-Angreifer belegt zurück oder fällt Poulsen doch aus, gehe ich auf 2:1 bzw. 3:0.**

### 1. FSV Mainz 05 – Bayer 04 Leverkusen
**Samstag, 10.10.2026, 15:30 Uhr** (MEWA Arena)
**Tipp: 1:1**
*unverändert* — **und heute aus dem einzigen Grund, der dazu übrig ist: Es gibt zu dieser Partie keine neue Information. Ich schreibe das hin, statt die gestrigen Argumente umzuformulieren.**

***Die Zentner-Schwelle vom 01.10. lautet wörtlich:*** „Wenn Mainz bis zum 09.10. bestätigt, dass Zentner spielt, gehe ich auf 2:1. Wenn Mainz bestätigt, dass er nicht spielt, gehe ich auf 1:2. **Aggregatorangaben lösen diese Bedingung nicht aus.**"

***Was heute dazu vorliegt: nichts.*** **Gestern gab es wenigstens die Aggregatorangabe „Zentner weiter im Individualtraining"; heute ist zu ihm keine Fundstelle aufgetaucht.** **Die Schwelle ist damit nicht ausgelöst, sondern unberührt.** Unverändert aus dem Vortagsstand: **Handverletzung aus dem Heimspiel gegen Frankfurt, mehrere Wochen, kein Rückkehrtermin, Rückkehr nach Vereinsangabe am „individuellen Heilungsverlauf", Vertreter Alexander Schwolow.**

***Die zweiteilige Schwelle von gestern, Teil (b), ist ebenfalls nicht ausgelöst – und das musste ich heute prüfen.*** (b) lautete: „Kommt zu Leverkusens heutiger Entwicklung ein weiterer belegter Rückkehrer oder eine Nebel-Absage hinzu, gehe ich auch ohne Zentner-Angabe auf 1:2." **Geprüft und nicht erfüllt:**
- **Zum 6:0 gegen Fortuna Köln vom 02.10. liegen heute mehr Details vor, aber kein neuer Rückkehrer von meiner Ausfallliste:** Terrier und Schick je zweimal, Tella, Gutiérrez per Freistoß; **Boniface und Ben Seghir kamen in der zweiten Halbzeit, dazu sechs U19-Spieler, weil neun Nationalspieler fehlten.** **Boniface stand in keinem meiner Läufe auf der Ausfallliste – seine Einwechslung ist kein Rückkehrer im Sinne meiner Schwelle**, und die eine Fundstelle, die von „Comeback nach der Rückkehr aus Bremen" spricht, beschreibt einen Vereinswechsel, keine Verletzung.
- **Zu Paul Nebel liegt keine Absage vor.** Sein voraussichtlicher Rückkehrtermin bleibt der **10.10.2026**, also der Spieltag selbst, bei noch nicht vollständigem Mannschaftstraining.

***Die Ausfallbilanz, unverändert bei sechs gegen drei.***
- **Mainz: Dominik Kohr** (nach Operation), **Silas** (Schien- und Wadenbeinbruch, sechs Monate), **Silvan Widmer** (Patellasehne linkes Knie, mehrere Wochen, konservativ, kein Termin – Kapitän), **Paul Nebel** (Adduktoren/Leiste, Rückkehr voraussichtlich 10.10.), **Katompa Mvumpa** und **Caci** (beide nur Listeneintrag). **Dazu Zentner als siebtes Fragezeichen.**
- **Leverkusen: Doué** (Wadenmuskel), **Eichhorn** (Stoffwechselerkrankung), **Culbreath** (nur Listeneintrag).
- **Die Pausenform, unverändert:** Mainz 3:0 beim Drittligisten SV Waldhof am 03.10. (Königsdörffer 25., Becker 28., Hollerbach 55., ohne Zuschauer), Leverkusen 6:0 gegen den Drittligisten Fortuna Köln am 02.10. **Zwei Siege gegen Drittligisten, einer davon mit U19-Aushilfe – das trennt nichts.**

***Warum 1:1 steht – und wo die Grenze liegt, unverändert.*** **Beide Mannschaften haben 7 Punkte** (Mainz 10:6, Leverkusen 10:5). **Die entscheidende Symmetrie ist eine Schwäche-Symmetrie: Mainz hat zu Hause einen Punkt aus zwei Spielen bei 1:3 Toren, Leverkusen auswärts einen Punkt aus zwei Spielen bei 4:5 Toren und keinen Auswärtssieg.** **Ein Heimteam, das zu Hause nicht trifft, gegen einen Gast, der auswärts nicht gewinnt – das ist 1:1 als Ergebnis, nicht als Ausweichen.**

***Die Schwelle für den nächsten Lauf, unverändert zweiteilig:*** **(a)** **Nur eine Mainzer Vereinsangabe zu Zentner bewegt diesen Tipp** – spielt er, 2:1; spielt er nicht, 1:2. **(b)** **Ein weiterer belegter Leverkusener Rückkehrer von meiner Ausfallliste oder eine Nebel-Absage bringt 1:2, auch ohne Zentner-Angabe.**

### 1. FC Union Berlin – SV 07 Elversberg
**Samstag, 10.10.2026, 15:30 Uhr** (Alte Försterei)
**Tipp: 1:2**
*unverändert* — **und zum fünften Lauf in Folge der bestbelegte der neun.**

***Die Unioner Ausfälle stehen heute den fünften Tag in Folge, namentlich identisch.*** **Robert Skov** (Muskelverletzung, Anfang September), **Marvin Friedrich** (Anfang September), **Andrej Ilić** (Krankheit), **Oliver Burke** (Achillessehne, Anfang September), **Stanley Nsoki** (Wade, Mitte September), **Andrik Markgraf** (Kreuzbandverletzung), **Frederik Rønnow** (Oberschenkel). **Sieben Namen, fünf Läufe, keine Abweichung.** **Zu Rønnow steht heute keine Qualifizierung – weder „fraglich" noch eine Entwarnung –, ich führe ihn weiter als fraglich und halte fest, dass die Darstellung nun dreimal unterschiedlich war, ohne dass eine Diagnose dazukam.**

***Zum Zimmerschied-Widerspruch gibt es heute eine Mehrheit, und ich sage, dass es nur eine Mehrheit ist.*** **Die heutige Liste führt Tom Zimmerschied als verletzt auf der Elversberger Seite.** **Damit steht es zwei zu eins für Elversberg** (02.10. Elversberg, 03.10. Union, 04.10. Elversberg). **Ich neige deshalb zu Elversberg, verwende ihn aber weiter auf keiner Seite als belegt, weil drei Listeneinträge ohne Spielbericht keine Entscheidung sind.** **Für den Tipp ist es gleichgültig: auf Unioner Seite stehen sieben Namen, auf Elversberger ein belegter.**

***Auf Elversberger Seite bleibt es bei einem belegten Ausfall.*** **Luis Seifert, seit über zwei Monaten verletzt**, als Langzeitfall eingeordnet. **Gyamerah bleibt unbelegt.** **Zum heutigen Stand: ein belegter Gäste-Ausfall gegen sechs sichere plus ein fragliches beim Gastgeber.**

***Zur Form in der Pause, mit einer heutigen Relativierung aus zwei Richtungen.*** **Elversberg hat am 02.10. 3:2 bei Hoffenheim gewonnen (0:1 zur Pause), unter Trainer Vincent Wagner** – **gegen eine gemischte Erstliga-/U23-Elf, bei der 18 von 27 TSG-Profis abgestellt waren.** **Diese Relativierung ist heute durch Hoffenheims eigene Darstellung bestätigt, und ich ziehe sie damit zum dritten Lauf ab.** **Von Union ist der Test beim BAK 07 weiterhin nur angekündigt, ein Ergebnis bleibt im dritten Lauf unauffindbar.** **Trainer: Mauro Lustrinelli (Union), Vincent Wagner (Elversberg).**

***Die Abwägung, unverändert:*** **Elversberg hat als Aufsteiger in Gladbach 4:3 und gegen Leverkusen 3:2 gewonnen – der Club trifft, und er trifft auswärts.** **7 Punkte gegen 1, 8:7 gegen 4:17, ein Ausfall gegen sechs.** **Union hat in vier Spielen 17 Gegentore kassiert, keinen Sieg und einen Punkt.** **1:2 bleibt.**

***Die Schwelle für den nächsten Lauf:*** **Nur eine belegte Rønnow-Entwarnung oder ein zweiter Elversberger Ausfall mit Diagnose bewegt diesen Tipp.**

### SC Paderborn 07 – VfB Stuttgart
**Samstag, 10.10.2026, 15:30 Uhr** (Home Deluxe Arena)
**Tipp: 1:2**
*unverändert* — **und das muss ich heute anders begründen als gestern, weil meine Schwelle ausgelöst worden ist.**

***Die Schwelle lautete:*** „**Nur eine belegte Aktualisierung zur Paderborner Erkältungswelle oder ein Stuttgarter Ausfall mit Diagnose bewegt diesen Tipp.**" **Die Aktualisierung ist heute da – nach zwei Läufen ohne eine. Ich habe den Tipp daraufhin neu geprüft und lasse ihn stehen; hier ist, warum.**

***Was zur Erkältungswelle vorliegt, und es sind zwei Dinge in entgegengesetzter Richtung.***
- **Pro Paderborn: Das Quartett ist wieder gesund.** **Curda, Obermair, Hansen und Baack waren bei der Platzbegehung dabei und werden als „wieder gesund" geführt. Hansen und Baack haben im Test Minuten bekommen, Curda und Obermair haben nicht gespielt.** **Damit ist der seit zwei Läufen offene Punkt geschlossen, und er ist besser ausgegangen, als ich annehmen musste.**
- **Contra Paderborn, und es ist mir vorher nicht bekannt gewesen: Der Test war ein 1:0 bei D.C. United am 01.10., zum Abschluss einer USA-Reise.** **Die Krankheitsfälle sind nach derselben Fundstelle während des Aufenthalts in den USA aufgetreten.** **Ein Bundesligist, der in der Länderspielpause nach Washington und zurück fliegt, hat eine Woche vor dem Heimspiel eine Transatlantikreise in den Beinen.** *Einschränkung: Das steht nur auf Suchzusammenfassungen, die Vereinsseite ist nicht lesbar, und ich habe das Datum nicht gegengeprüft.*

***Mein Schluss, offen hingeschrieben: Die beiden Punkte heben sich auf.*** **Die Gesundung ist eine Rückkehr zum Normalzustand, den ich nie als Ausfall eingerechnet hatte – sie macht Paderborn nicht stärker als in der Tabelle, sondern genau so stark.** **Die USA-Reise ist ein Belastungsfaktor, aber acht Tage Abstand zum Anpfiff entschärfen ihn.** **Die Schwelle ist damit ausgelöst, geprüft und erledigt; ich streiche sie und ersetze sie unten.**

***Und Stuttgart hat heute ebenfalls keinen neuen Ausfall – aber eine bessere Belegqualität bei den alten.*** **Es bleibt bei drei belegten Stuttgarter Ausfällen: Dan-Axel Zagadou** (muskuläre Verletzung der Oberschenkelrückseite; **heute neu: er trainiert individuell auf dem Platz, also im Aufbau**), **Justin Diehl** (heute als Langzeitverletzter geführt) und **Jarzinho Malanga** (**heute erstmals mit Diagnose: Bauchmuskelverletzung**). **Zwei von drei Einträgen sind damit heute präziser als gestern, aber kein vierter Name ist dazugekommen – die zweite Hälfte meiner Schwelle ist nicht erfüllt.** **Die Stuttgarter Neunerliste, die seit drei Läufen Dennis Seimen als Ausfall führt, obwohl er am 02.10. 71 Minuten im Tor gespielt hat, verwende ich weiter nicht.**

***Stuttgarts Pausenform, unverändert:*** **Zwei Testspiele, zwei Siege, acht Tore, kein Gegentor – 3:0 gegen Heidenheim und 5:0 gegen Greuther Fürth** (Großaspach, 3.876 Zuschauer; Undav zweimal, Prömel, van der Leij, Leweling). **Hoeneß war „sehr zufrieden".**

***Die Abwägung, unverändert:*** **Paderborn hat in drei Heimspielen vier Punkte und drei Saisontore insgesamt bei 3:5 – die schwächste Offensive des Spieltags neben Schalke.** **Dagegen ein Auswärtstabellenletzter mit 2:7, der in der Pause 8:0 testet, seinen Torwart zurückbekommt und dessen drei Ausfälle sich im Aufbau befinden.** **1:2 bleibt.**

***Die neue Schwelle:*** **Nur ein Stuttgarter Ausfall mit Diagnose oder ein belegter Paderborner Rückkehrer in der Offensive bewegt diesen Tipp.** **Die Erkältungswelle ist als Kriterium erledigt – ich nehme sie nicht noch einmal auf.**

### RB Leipzig – Eintracht Frankfurt
**Samstag, 10.10.2026, 18:30 Uhr** (Red Bull Arena)
**Tipp: 2:1**
*unverändert* — **und das ist heute das Ergebnis einer Schwelle, die ich gestern streng formuliert habe und die erfüllt worden ist.**

***Die Schwelle lautete wörtlich:*** „**Bringt der nächste Lauf keine Bestätigung, dass Lukeba im Mannschaftstraining ist, gehe ich auf 1:1 zurück und bleibe dort bis zum Anpfiff.**"

***Die Bestätigung liegt vor, aus zwei Fundstellen.*** **„Lukeba wieder beim Team: Entscheidung fällt kurzfristig."** Dazu eine zweite, partiebezogen: **Er wird für das Frankfurt-Spiel als voll verfügbar erwartet und ist bereits ins Mannschaftstraining zurückgekehrt.** **Die Schwelle ist damit erfüllt, und 2:1 bleibt – nicht aus Trägheit, sondern weil die Bedingung eingetreten ist, die ich mir vorher gesetzt habe.**

***Und die Einschränkung, die ich nicht unterschlagen will, steht in der Überschrift selbst:*** **„Entscheidung fällt kurzfristig" ist keine Einsatzgarantie.** **Ich führe Lukeba als im Mannschaftstraining und wahrscheinlich einsatzfähig, nicht als gesetzt.** **Was gestern dazu stand, bleibt gültig und ist nicht überholt: zurück in Leipzig, schrittweise Belastungssteigerung, vollständige Integration für diese Woche geplant, Frankfurt als ausdrückliches Ziel.**

***Die Zahl, die Lukebas Gewicht für genau diese Partie belegt, unverändert:*** **In beiden Bundesligaspielen mit Lukeba in der Startelf gewann Leipzig zu null – 3:0 gegen Gladbach, 5:0 gegen den HSV. Ohne ihn kamen die Niederlagen: 1:3 in Bremen, 0:2 in Leverkusen.** **Leipzigs Heimbilanz ist 8:0 mit zwei Zu-null, und sie ist seine Bilanz.**

***Was heute für Leipzig entscheidend ist, ist allerdings eine Verwerfung, nicht eine Meldung.*** **Eine heutige Vorschau nennt Orbán als „mehr als fraglich", Schlager als gesperrt, Banzuzi mit Knieverletzung und Lukeba als nicht verfügbar.** **Das wäre der schwerste Schlag gegen diesen Tipp seit vier Läufen – und es stammt vollständig aus einem Kaderupdate vor einem Leipziger Spiel gegen Union Berlin, das in dieser Saison nicht stattgefunden hat** (Verworfene Fundstellen, Punkt 1). **In derselben Mitteilung steht Orbán als „fully fit" und Schlager als nach abgesessener Sperre wieder verfügbar.** **Verworfen.** *Belegt bleibt für Leipzig:* **Reitz und Baumgartner brauchen weiter Zeit und fehlen gegen Frankfurt; Raum, Orbán und Nusa kehren erst zu Beginn der Woche von ihren Nationalmannschaften zurück; Demichelis steht nach 6 Punkten aus 4 Spielen unter Druck.**

***Auf Frankfurter Seite hat sich heute das Gegenteil von gestern ergeben, und es geht für meinen Tipp.*** **Maluze ist weiter im Reha-Training und nicht einsatzfähig** (Korrektur 2) – **die gestrige Nennung als Option für die rechte Position war eine Berichterstatter-Aufzählung, und meine eigene Einschränkung dazu war berechtigt.** **Frankfurts Dreierkette besteht damit nach aktuellem Stand aus Robin Koch im Zentrum, Nnamdi Collins rechts und Lilian Brassier links – ohne die Alternative, die Hütter gestern noch zugeschrieben wurde.** **Unverändert positiv für Frankfurt: Robin Koch nach Infekt zurück, Dōan fit, das 4:0 gegen Braunschweig am 02.10.** (Otávio 33., Eigentor Tempelmann 57., Knauff 68., Wünsch 79.) – **und heute bestätigt, dass Hütter mit dem Test zufrieden war und bei zwei Startelf-Kandidaten Fortschritte gesehen hat.**

***Das Argument gegen meinen Tipp, und es ist unverändert gut.*** **Frankfurt ist auswärts die bessere Hälfte seiner Saison: 3:3 bei Union, 3:1 in Mainz – vier Punkte, 6:4, während die Heimbilanz 1:4 gegen Augsburg und 2:2 gegen Freiburg lautet.** **Ein Gast, der auswärts trifft, gegen ein Heimteam mit 8:0 – das trägt ein Frankfurter Tor. Deshalb 2:1 und nicht 2:0.**

***Warum 2:1 bleibt, in einem Satz:*** **Leipzig zu Hause ist 8:0 mit zwei Zu-null, und der Innenverteidiger, der beide Spiele bestritten hat, ist heute belegt zurück im Mannschaftstraining; Frankfurt trifft auswärts, aber es gewinnt dort nicht, und seine Dreierkette hat heute die Option verloren, die sie gestern noch hatte.**

***Die Schwelle für den nächsten Lauf, unverändert streng:*** **Kommt eine Leipziger Vereinsangabe, dass Lukeba nicht spielt, gehe ich auf 1:1 und bleibe dort bis zum Anpfiff.** **Eine weitere Änderung nach oben mache ich nur gegen eine Vereinsangabe, nicht gegen eine Vorschau.**

### 1. FC Köln – Borussia Mönchengladbach
**Sonntag, 11.10.2026, 15:30 Uhr** (RheinEnergieStadion)
**Tipp: 1:0**
**Änderung gegenüber gestern: 1:1 → 1:0, weil Borussia Mönchengladbach heute mit Franck Honorat den nächsten Offensivspieler verloren hat – Muskelverletzung im Training, vom Verein bestätigt, Ausfall „auf unbestimmte Zeit", das Derby am 11.10. ausdrücklich verpasst – und weil sein nominaler Ersatz Nicolas Kühn weiter mit Muskelbündelriss fehlt. Das Tor, das mein 1:1 von einem Gast mit 0:8 und null Auswärtstoren verlangte, hat heute seinen plausibelsten Zubringer verloren.**

***Zuerst die Meldung, auf der die Änderung steht, mit allem, was dazu belegt ist.*** **Franck Honorat, 30, hat sich im Training eine Muskelverletzung zugezogen.** **Der Verein hat bekanntgegeben, dass er „auf unbestimmte Zeit" ausfällt.** **Er verpasst das Derby beim 1. FC Köln am 11.10., 15:30 Uhr**, und **nach Einschätzung der Rheinischen Post dürfte er auch für das darauffolgende Spiel gegen Hoffenheim fraglich sein.** **Entscheidend für den Tipp ist der zweite Teil: Nicolas Kühn, der in den Fundstellen ausdrücklich als Honorats nominaler Ersatz geführt wird, fehlt weiter mit Muskelbündelriss.** **Gladbach verliert also nicht einen Flügelspieler, sondern den Flügel.**

**Gladbachs belegte Ausfallliste wächst damit auf vier: Honorat** (Muskelverletzung, unbestimmt, neu), **Nicolas Kühn** (Muskelbündelriss), **Enzo Leopold** (Kreuzbandriss, monatelang), **Jens Castrop** (Schulter). **Drei Rückkehrer nach Verletzung bleiben: Hashioka, Konoplya, Uno.**

***Und jetzt die Kölner Seite, auf der heute die Schwelle von gestern beantwortet worden ist – teilweise.*** Die Schwelle lautete: „**Nur eine belegte Angabe dazu, wer bei Köln am 11.10. im Sturmzentrum spielt, bewegt diesen Tipp. Ist es ein Nachwuchsspieler oder ein umgestellter Flügelspieler, gehe ich auf 0:1. Verpflichtet oder reaktiviert Köln eine Alternative mit Bundesligaerfahrung, bleibt es bei 1:1.**"

**Was heute dazu vorliegt:**
- **Beide Mittelstürmer fallen für das Derby aus – das ist jetzt partiebezogen belegt, nicht mehr nur die Diagnose von gestern.** **Thijs Dallinga: Kreuzbandverletzung, Monate** (er verdrehte sich in der 34. Minute bei einem Torschussversuch das rechte Knie). **Ragnar Ache: Oberschenkel-Muskelverletzung, Verein sagt „vorerst", keine Dauer.** Die Vereinsseite überschreibt es mit „Ragnar Ache fällt aus".
- **Voraussichtlich spielt Marius Bülter im Sturmzentrum; Luca Waldschmidt könnte ebenfalls in die Mitte rücken.** Eine Fundstelle überschreibt die Lage mit „Rhein-Derby ohne Mittelstürmer?".
- **Köln prüft die Verpflichtung eines vereinslosen Stürmers, aber die Fundstellen halten das für zweifelhaft** – ein Profi nach monatelanger Pause ohne Mannschaftstraining sei keine Soforthilfe – **und nennen eine interne Lösung als wahrscheinlicher.**

***Warum ich daraus 1:0 mache und nicht 0:1, obwohl eine Lesart meiner Schwelle auf 0:1 führt. Das ist die Stelle, an der ich meine eigene Regel korrigieren muss, und ich sage warum.***

**Meine Schwelle hatte zwei Zweige, und Bülter erfüllt beide gleichzeitig: Er ist ein umgestellter Flügelspieler – und er ist eine Alternative mit Bundesligaerfahrung, die bereits im Kader steht.** **Er hat im Testspiel den Ausgleich geköpft und die Hereingabe zum ersten Tor vorbereitet, und er hat in einem früheren Derby als Mittelstürmer anstelle von Ache begonnen.** **Ein Zweig sagt 0:1, der andere 1:1. Die Schwelle trennt den Fall nicht, den sie treffen sollte.**

**Was sie außerdem nicht vorsehen konnte: Der Zielwert 0:1 setzt voraus, dass Gladbach trifft und gewinnt. Genau diese Voraussetzung ist heute von der Honorat-Meldung getroffen worden.** **Gladbach hat in zwei Auswärtsspielen 0:8 gespielt und kein Tor erzielt; es ist Letzter mit 0 Punkten und 6:16; und es verliert fünf Tage vor dem Derby den Offensivspieler, dessen Ersatz schon fehlt.** **Ein 0:1 verlangte von diesem Gast das erste Auswärtstor der Saison und zugleich den ersten Auswärtssieg. Das kann ich nicht tippen, während die Offensive des Gastes kleiner wird.**

***Warum Kölns Tor im Tipp bleibt, obwohl die Mitte fehlt.***
- **Gladbach hat in vier Spielen 16 Gegentore kassiert – 3, 4, 5, 4 –, die schlechteste Defensive der Liga, und keine Partie unter drei Gegentoren.** **Gegen diese Abwehr ein Kölner Tor zu Hause anzunehmen, verlangt keinen Mittelstürmer.**
- **Was Köln an Offensive bleibt, ist nicht wenig: Bülter mit Bundesliga-Torquote, dazu Kamiński und El Mala, die zusammen an 21 Toren direkt beteiligt waren und aus der Abstellung zurückkehren, sowie Waldschmidt und Maina als Umstellungsoptionen.**
- **Köln zu Hause: 3:2 gegen Hoffenheim, 1:1 gegen Werder – vier Punkte, 4:3 in zwei Spielen.**

***Und das Argument gegen meine Änderung – ich stelle es ausdrücklich hin, weil es gut ist.*** **Tim Kleindienst ist fit, Kapitän und trifft: Im Test bei St. Pauli (1:1, knapp 18.000 Zuschauer) hat er Gladbach per Kopfball nach einer Ecke in Führung gebracht; Ricky-Jade Jones glich in der 75. aus.** **Gladbach spielte dort ein 3-4-1-2 mit der Doppelspitze Kleindienst/Machino.** **Ein Mittelstürmer in Form und ein System mit zwei Spitzen sind genau das, was ein erstes Auswärtstor erzeugen kann – und sie sind der Grund, warum diese Änderung die schwächste der drei Änderungen dieser Woche ist.** **Für Blessin ist es außerdem das Ligadebüt als Nachfolger von Eugen Polanski**, nach zwei ungeschlagenen Tests (3:0 bei Sportfreunde Siegen, 1:1 bei St. Pauli).

***Zur Trainerfrage auf Kölner Seite, unverändert:*** **Nach Sky Sport will Köln mit René Wagner weitermachen, das Derby sei kein Endspiel; `bundesliga.com` führt „René Wagner bleibt Chefcoach".** **Bei einer Derby-Niederlage könnte es trotz Vertrag bis 2028 eng werden; Wagner hat in elf Ligaspielen zwei Siege geholt.** **Die Buchmacherquote zur ersten Entlassung bleibt ein Nullargument und wird nicht verwendet.**

***Warum 1:0, in einem Satz:*** **Ein Gastgeber, der seine beiden Mittelstürmer verloren hat, aber zu Hause gegen die schlechteste Defensive der Liga spielt und seine Flügel zurückbekommt, gegen einen Gast, der auswärts noch nie getroffen hat und heute den nächsten Offensivspieler verloren hat, dessen Ersatz schon fehlte.**

***Die neue Schwelle, und sie ist diesmal eindeutig formuliert, weil die letzte es nicht war:*** **Kommt eine Kölner Vereinsangabe, dass ein Nachwuchsspieler im Sturmzentrum beginnt, gehe ich auf 0:0. Verpflichtet Köln einen Stürmer mit Bundesligaerfahrung und wird er gemeldet, gehe ich auf 2:1. Kommt eine belegte Gladbacher Entwarnung zu Honorat oder Kühn, gehe ich auf 1:1 zurück.**

### SC Freiburg – FC Schalke 04
**Sonntag, 11.10.2026, 17:30 Uhr** (Europa-Park-Stadion)
**Tipp: 2:0**
*unverändert* — **und die Schwelle von gestern ist geprüft und nicht ausgelöst.**

***Die Schwelle lautete:*** „**Wird Ljubičić belegt fit gemeldet oder kommt ein weiterer Schalker Offensivspieler zurück, gehe ich auf 2:1.**"

***Geprüft und nicht erfüllt – und das Prüfen war heute die Arbeit.*** **Eine heutige Schalker Ausfallliste nennt Ljubičić, Gülasi, Lasme und Gantenbein.** **Zwei davon – Lasme und Gantenbein – standen gestern in der namentlich belegten Startelf beim 1:0 in Austria Lustenau** (Verworfene Fundstellen, Punkt 4). **Nach meiner eigenen Regel schlägt der datierte Spielbericht den Listeneintrag: Lasme und Gantenbein sind verfügbar, Gülasi übernehme ich nicht als belegt.** **Und zu Ljubičić steht das Gegenteil einer Fitmeldung: Er wird weiter als Ausfall geführt.** **Es ist also kein Offensivspieler belegt zurückgekommen, und der eine belegte Ausfall ist nicht entwarnt. Die Schwelle bleibt.**

***Was bei Schalke belegt ausfällt, unverändert:*** **Dejan Ljubičić, Verletzung am linken Knie, nach Bild ausdrücklich kein Kreuzbandriss, Ausfall voraussichtlich bis nach der Länderspielpause – partiebezogen: „Mit der Partie am 11. Oktober in Freiburg soll es für Ljubičić eng werden", frühestens am 17.10. gegen Mainz wieder verfügbar.** **Ich führe ihn für den 11.10. als Ausfall mit kleinem Restzweifel.** **Robin Gosens bleibt verfügbar** (Startelf und Vorarbeit in Lustenau, gestern belegt). **Dass Schalke vor dem Test neun Talente aus U19 und U23 zu den Profis hochgezogen hat, lese ich weiter als Hinweis auf fehlende Kaderbreite, nicht auf Tiefe.**

***Auf Freiburger Seite ist die Lage heute vollständiger als gestern, und sie ist dünn im besten Sinne.*** **Belegt fehlt genau ein Spieler: Florent Muslija mit Kreuzbandverletzung.** **Zum Test gegen den FC Luzern (4:2, Trainingsgelände, nicht öffentlich) liegen heute auch die Gegentore vor: Lars Villiger (18., abgelenkter Schuss) und Adrian Grbic in der zweiten Halbzeit; für Freiburg Grifo (11.), Höler (26., 62.), Ginter (44.).** **Schusters Einordnung: Die Mannschaft habe umgesetzt, was im Training über Kombinationen und hohe Ballgewinne besprochen worden sei.** *Zur Datierung:* **Eine heutige Fundstelle datiert ihren Bericht auf den 04.10., mein Vortagsstand ordnet die Partie dem 03.10. zu.** **Einen zweiten Freiburg-Luzern-Test habe ich heute nicht gefunden; ich lasse die Frage offen, weil Ergebnis und Torschützen in allen Fundstellen übereinstimmen und der Tipp davon nicht abhängt.**

***Der Formvergleich aus derselben Pause, unverändert:*** **Freiburg 4:2 gegen einen Schweizer Erstligisten – Schalke 1:0 bei einem österreichischen Zweitligisten, der in der ersten Halbzeit die besseren Chancen hatte.** **Das ist derselbe Unterschied, den die Tabelle zeigt: 12:3 gegen 3:4.** **Heute ist diese Tabellenlage erstmals extern gegengeprüft: Freiburg Dritter, Schalke Elfter.**

***Warum 2:0 bleibt.*** **Das Argument gegen ein höheres Ergebnis ist Schalkes Defensive: 3:4 Tore in vier Spielen, zwei Zu-null (0:0 gegen Bayern, 0:0 gegen Elversberg), nur vier Gegentore als Aufsteiger.** **Das Argument für die Null ist die andere Hälfte derselben Bilanz: drei eigene Tore in vier Spielen, die schwächste Offensive der Liga – und ein einziges Tor gegen einen Zweitligisten.** **Dagegen Freiburg: 10 Punkte, 12:3, zu Hause neun Tore in zwei Spielen, ein belegter Ausfall.**

***In einem Satz:*** **Eine Mannschaft mit neun Heimtoren in zwei Spielen und einem einzigen Ausfall gegen die schwächste Offensive der Liga, deren einziger belegter Ausfall ein Mittelfeldspieler ist, für den es „eng" wird.**

***Die Schwelle für den nächsten Lauf, unverändert:*** **Wird Ljubičić belegt fit gemeldet oder kommt ein Schalker Offensivspieler belegt zurück, gehe ich auf 2:1. Ein Freiburger Ausfall mit Diagnose bringt 1:0.**

---

## Verteilung und Selbstkontrolle

**Die neun Tipps im Überblick:**

| Partie | Anstoß | Tipp | Status |
|---|---|---|---|
| Borussia Dortmund – SV Werder Bremen | Fr 09.10., 20:30 | **3:1** | unverändert |
| FC Augsburg – FC Bayern München | Sa 10.10., 15:30 | **1:2** | unverändert |
| TSG Hoffenheim – Hamburger SV | Sa 10.10., 15:30 | **2:0** | unverändert |
| 1. FSV Mainz 05 – Bayer 04 Leverkusen | Sa 10.10., 15:30 | **1:1** | unverändert |
| 1. FC Union Berlin – SV 07 Elversberg | Sa 10.10., 15:30 | **1:2** | unverändert |
| SC Paderborn 07 – VfB Stuttgart | Sa 10.10., 15:30 | **1:2** | unverändert (Schwelle ausgelöst, geprüft, erledigt) |
| RB Leipzig – Eintracht Frankfurt | Sa 10.10., 18:30 | **2:1** | unverändert (Schwelle erfüllt) |
| 1. FC Köln – Bor. Mönchengladbach | So 11.10., 15:30 | **1:0** | **geändert von 1:1** |
| SC Freiburg – FC Schalke 04 | So 11.10., 17:30 | **2:0** | unverändert |

**Verteilung:** 5 Heimsiege (Dortmund, Hoffenheim, Leipzig, Köln, Freiburg), 3 Auswärtssiege (Bayern, Elversberg, Stuttgart), 1 Unentschieden (Mainz – Leverkusen). **Tore: 13 Heim, 9 Gast, 22 insgesamt, Schnitt 2,44.** **Die Änderung des Tages senkt den Schnitt leicht; das ist eine Folge, kein Ziel.**

**Selbstkontrolle zu den Änderungen dieser Woche.** **An vier aufeinanderfolgenden Läufen habe ich je genau einen Tipp geändert** (01.10.: Dortmund – Werder auf 3:1; 02.10.: Leipzig – Frankfurt auf 1:1; 03.10.: Leipzig – Frankfurt zurück auf 2:1; 04.10.: Köln – Gladbach auf 1:0). **Nur eine dieser Änderungen war eine Rücknahme, und sie ist als solche begründet worden.** **Die heutige steht auf einer Vereinsmeldung mit Namen, Diagnose und Partiebezug – das ist die beste Quellenkategorie, die in diesem Repo überhaupt erreichbar ist.** **Was ich mir vorhalten muss: Die Kölner Schwelle von gestern war schlecht formuliert, weil ihre beiden Zweige denselben Spieler treffen. Ich habe sie oben ersetzt, und die neue Fassung nennt Vereinsangaben statt Spielertypen.**

**Was heute gegen die Tipps spricht, in drei Zeilen, damit es nicht in den Begründungen verschwindet:** **Ryerson ist wahrscheinlich kein Langzeitausfall** (gegen Dortmund 3:1); **Paderborns Erkältungswelle ist überwunden** (gegen Paderborn 1:2); **Kleindienst ist in Form und Gladbach spielt mit Doppelspitze** (gegen Köln 1:0).

---

## Quellen

**Vorbemerkung:** Keine dieser Adressen war aus dieser Umgebung abrufbar. Was unten steht, ist die Adresse zu einem Suchergebnis, dessen Titel und Zusammenfassung ich verwendet habe – **nicht ein von mir gelesener Artikel.** Wo das Datum aus der Adresse hervorgeht, nenne ich es.

**Spieltag, Ansetzungen und Anstoßzeiten**
- [anstosszeiten.de – 5. Spieltag Bundesliga 2026/27](https://anstosszeiten.de/bundesliga/spieltag-5/) *(nicht abrufbar, EGRESS_BLOCKED)*
- [bundesliga.com – Exakte Termine für alle Spiele bis Ende November](https://www.bundesliga.com/de/bundesliga/news/ansetzungen-spieltage-termine-zeitgenau-fans-24024) *(nicht abrufbar)*
- [werkself.de – 5. Spieltag: Mainz 05 – Leverkusen, Sa 10.10.2026, Anstoß 15.30 Uhr](https://www.werkself.de/forum/thread/44694-bundesliga-2026-27-5-spieltag-1-fsv-mainz-05-bayer-04-leverkusen-samstag-10-10-2/) – **Gegenprobe zur Anstoßzeit**
- [ruhrnachrichten.de – Länderspielpause: Dann geht es mit der Bundesliga weiter](https://www.ruhrnachrichten.de/service/bundesliga-fussball-fuenfter-spieltag-saison-2026-27-partien-mannschaften-uebertragung-w1251490-2002238953/)

**Dortmund – Werder**
- [kicker.de – Dortmunds Außenverteidiger: Säule und Sorgen (Ryerson)](https://www.kicker.de/dortmunds-aussenverteidiger-saeule-und-sorgen-1258205/artikel) – **kein Langzeitausfall erwartet, Einsatz gegen Werder unsicher**
- [sport1.de – BVB-Profi Ryerson kehrt verletzt von Nationalteam zurück](https://www.sport1.de/news/fussball/bundesliga/2026/10/bvb-profi-ryerson-kehrt-verletzt-von-nationalteam-zurueck)
- [footy.de (02.10.2026) – BVB bangt um Ryerson: Norwegen-Coach gibt Verletzungs-Update](https://footy.de/2026/10/02/bvb-bangt-um-ryerson-norwegen-coach-gibt-verletzungs-update)
- [bet365-Nachrichten (01.10.2026) – Nico Schlotterbeck Verletzungsupdate](https://news.bet365.de/de-de/article/nico-schlotterbeck-verletzungsupdate-das-sind-die-neuesten-infos/2026100109165482896)
- [ruhrnachrichten.de – Wie die Länderspielpause zum Problem für Dortmund wird](https://www.ruhrnachrichten.de/bvb/borussia-dortmund-laenderspielpause-trainingsausfall-homeoffice-niko-kovac-herausforderung-w-2002230828/) – **20 Abstellungen, Trainingsbetrieb ausgesetzt**
- [bvbwld.de (04.10.2026) – Alarm vor BVB-Spiel: Werder-Trainer Thioune platzt der Kragen](https://bvbwld.de/2026/10/04/alarm-vor-bvb-spiel-werder-trainer-thioune-platzt-der-kragen/) – **Thioune im Wortlaut, Spielverlauf 0:7**
- [weser-kurier.de – Eren Dinkci kehrt ins Mannschaftstraining zurück](https://www.weser-kurier.de/werder/profis/werder-bremen-eren-dinkci-kehrt-ins-mannschaftstraining-zurueck-doc87tpnhpm5ti19nssdhid)

**Augsburg – Bayern**
- [fcaugsburg.de – FCA trennt sich im Testspiel gegen Hertha BSC 2:2](https://www.fcaugsburg.de/article/fca-trennt-sich-im-testspiel-gegen-hertha-bsc-2-2-23515)
- [herthabsc.com (10/2026) – Nach Zwei-Tore-Rückstand: Unentschieden in Augsburg](https://www.herthabsc.com/de/nachrichten/2026/10/spielbericht-fcabsc-2627)
- [bavarianfootballworks.com – FC Bayern halt team training until October 6](https://www.bavarianfootballworks.com/bayern-munich-bundesliga/260854/bayern-munich-training-sabener-strasse-quiet-international-break-germany)
- [fcbinside.de (28.09.2026) – Laimer meldet sich zurück, „voll fit und bereit"](https://fcbinside.de/2026/09/28/nach-verletzung-bayern-star-laimer-reist-zur-nationalmannschaft/) – **Grundlage für die Verwerfung des Laimer-Ausfalls**
- [sport1.de (09/2026) – Gute Nachricht für Bayern: Laimer meldet sich bei Österreich zurück](https://www.sport1.de/news/fussball/uefa-nations-league/2026/09/gute-nachricht-fuer-bayern-laimer-zurueck)
- [neunzigplus.de – Bayern-Spielplan Oktober: 9 Spiele, Musiala fehlt](https://neunzigplus.de/bundesliga/fc-bayern-oktober-spielplan-neun-spiele-musiala)

**Hoffenheim – HSV**
- [hsv.de – 2:0! HSV gewinnt Test unter Freunden](https://www.hsv.de/news/hsv-gewinnt-test-unter-freunden)
- [kicker.de – Poulsen muss raus und gibt Entwarnung: HSV schlägt Kopenhagen mit 2:0](https://www.kicker.de/poulsen-muss-raus-und-gibt-entwarnung-1258341/artikel) – **„Gegen Hoffenheim bin ich wieder dabei"**
- [bundesliga.com – HSV entscheidet Duell der Freunde](https://www.bundesliga.com/de/bundesliga/news/hsv-entscheidet-duell-der-freunde-39419)
- [nurdieraute.de (04.10.2026) – HSV schlägt Kopenhagen: Späte Tore überstrahlen Poulsen-Sorge](https://nurdieraute.de/2026/10/04/hsv-schlaegt-kopenhagen-spaete-tore-ueberschatten-poulsen-sorge/)
- [absolutfussball.com – Sturm-Not an der Elbe: HSV gehen vor Kopenhagen-Test die Angreifer aus](https://www.absolutfussball.com/deutschland/hamburger-sv/hamburger-sv-sturm-not-personal-sorgen-hsv-stuermer-verletzt-testspiel-fc-kopenhagen-bundesliga-94520200.html)
- [bundesliga.com – CAS sperrt Mario Vuskovic für vier Jahre](https://www.bundesliga.com/de/2bundesliga/news/hamburger-sv-mario-vuskovic-sperre-28669) · [hsv.de – dieselbe Meldung](https://www.hsv.de/news/cas-sperrt-mario-vuskovic-fuer-vier-jahre)
- [t-online.de – Vuskovic zurück im HSV-Training: 1.404 Tage Dopingsperre enden](https://hamburg.t-online.de/region/hamburg/id_101436096/mario-vuskovic-ist-zurueck-im-hsv-training-1404-tage-dopingsperre-enden.html) – **Widerspruch zur Sperrdauer, oben benannt**
- [tsg-hoffenheim.de (10/2026) – TSG verliert Test gegen Elversberg](https://www.tsg-hoffenheim.de/aktuelles/news/2026/10/tsg-verliert-test-gegen-elversberg)
- [rnz.de – „Hoffe" verliert geheimen Test gegen Elversberg](https://rnz.de/sport/sportregional_artikel,-TSG-Hoffenheim-Hoffe-verliert-geheimen-Test-gegen-Elversberg-_arid,2446433.html) – **gemischte Erstliga-/U23-Elf**

**Mainz – Leverkusen**
- [bayer04.de – 6:0 gegen Fortuna Köln](https://www.bayer04.de/de-de/news/bayer04/6-0-gegen-fortuna-koeln-werkself-gewinnt-trainingsspiel-gegen-drittligisten)
- [ligainsider.de – Leverkusen feiert klaren Testsieg gegen Fortuna Köln](https://www.ligainsider.de/bayer-04-leverkusen/4/leverkusen-feiert-klaren-testsieg-gegen-fortuna-koeln-418638/)
- [sportschau.de – Königsdörffer und Becker treffen: Mainz 05 gewinnt Testspiel in Mannheim](https://www.sportschau.de/regional/swr/swr-koenigsdoerffer-und-becker-treffen-mainz-05-gewinnt-testspiel-in-mannheim-100.html)
- [sky.de – Robin Zentner fällt bei Mainz 05 mit Handverletzung mehrere Wochen aus](https://sport.sky.de/fussball/artikel/robin-zentner-faellt-bei-mainz-05-mit-handverletzung-mehrere-wochen-aus/13586103/34130)
- [ligainsider.de – Verletzte und gesperrte Spieler der 1. Bundesliga 2026/27](https://www.ligainsider.de/bundesliga/verletzte-und-gesperrte-spieler/) – **Aggregator, nur mit Gegenprobe verwendet**

**Union – Elversberg**
- [ligainsider.de – 1. FC Union Berlin, voraussichtliche Aufstellung 2026/27](https://www.ligainsider.de/1-fc-union-berlin/1246/) *(Aggregator; sieben Unioner Ausfälle, Zimmerschied heute bei Elversberg)*
- [sv07elversberg.de – 3:2-Sieg im Testspiel gegen die TSG Hoffenheim](https://sv07elversberg.de/32-sieg-im-testspiel-gegen-die-tsg-hoffenheim/) – **datiert dort „3. Oktober", von mir auf den 02.10. korrigiert**
- [fc-union-berlin.de – Testspiel in der Länderspielpause: Union gastiert beim BAK 07](https://www.fc-union-berlin.de/de/meldungen/testspiel-in-der-laenderspielpause-union-gastiert-beim-bak-07-rICEHy) – **Ankündigung, kein Ergebnis auffindbar**

**Paderborn – Stuttgart**
- [ligainsider.de – Erkältung bremst Paderborn-Quartett aus](https://www.ligainsider.de/laurin-curda_36261/erkaeltung-bremst-paderborn-quartett-aus-418599/) – **Curda, Obermair, Hansen, Baack; Gesundung und Testeinsätze**
- [scp07.de – Newsarchiv](https://www.scp07.de/Newsarchiv/Alle-im-Einsatz.html) *(nicht abrufbar; USA-Reise und 1:0 bei D.C. United nur über Suchzusammenfassung)*
- [ligainsider.de – VfB Stuttgart, voraussichtliche Aufstellung 2026/27](https://www.ligainsider.de/vfb-stuttgart/12/) – **Zagadou Individualtraining, Malanga Bauchmuskelverletzung, Diehl Langzeitverletzter**

**Leipzig – Frankfurt**
- [ligainsider.de – Lukeba wieder beim Team: Entscheidung fällt kurzfristig](https://www.ligainsider.de/castello-lukeba_27079/lukeba-wieder-beim-team-entscheidung-faellt-kurzfristig-412614/) – **Schwellenbestätigung**
- [absolutfussball.com – Wer fehlt, wer kommt zurück? RB Leipzigs Hoffnungen und Sorgen vor dem Spiel gegen Frankfurt](https://www.absolutfussball.com/deutschland/rb-leipzig/rb-leipzig-personal-update-eintracht-frankfurt-rueckkehrer-verletzte-bundesliga-castello-lukeba-94519475.html)
- [rblive.de – RB Leipzig: Gegen Frankfurt droht noch ein Ausfall in der Defensive](https://rblive.de/news/rb-leipzig-gegen-frankfurt-droht-noch-ein-ausfall-in-der-defensive-4233273) – **Grundlage der Orbán-/Schlager-/Banzuzi-Angaben, von mir als Vorsaison verworfen**
- [sportschau.de – „Das wird meine Herausforderung": Hütters komplexe Bastelarbeiten](https://www.sportschau.de/regional/hr/hr-das-wird-meine-herausforderung-huetters-komplexe-bastelarbeiten-100.html) – **Maluze weiter im Reha-Training**

**Köln – Gladbach**
- [sport1.de (10/2026) – Nächster Gladbach-Rückschlag: Honorat fällt vorerst aus](https://www.sport1.de/news/fussball/bundesliga/2026/10/naechster-gladbach-rueckschlag-honorat-faellt-vorerst-aus) – **Grundlage der heutigen Änderung**
- [gladbachlive.de – Derby-Schock für Gladbach: Offensiv-Star fehlt gegen Köln](https://www.gladbachlive.de/news/derby-schock-fuer-gladbach-offensiv-star-fehlt-gegen-koeln-1387989)
- [gladbachtotal.de – Franck Honorat fällt verletzt aus und verpasst das Rheinderby gegen Köln](https://www.gladbachtotal.de/franck-honorat-faellt-verletzt-aus-und-verpasst-das-rheinderby-gegen-koeln/)
- [neunzigplus.de – Rheinderby: Köln verliert Dallinga und Ache, Gladbach muss auf Honorat verzichten](https://neunzigplus.de/bundesliga/rheinderby-koeln-verliert-dallinga-und-ache-gladbach-muss-auf-honorat-verzichten/)
- [fc.de – Ragnar Ache fällt aus](https://fc.de/aktuelles/news/ragnar-ache-faellt-aus) · [bundesliga.com – Doppel-Schock für Köln](https://www.bundesliga.com/de/bundesliga/news/1-fc-koln-ausfall-thijs-dallinga-ragnar-ache-verletzung-39415)
- [fussballdaten.de – Verletzungshorror in Köln: Rhein-Derby ohne Mittelstürmer?](https://www.fussballdaten.de/news/verletzungshorror-koeln-rhein-derby-ohne-mittelstuermer/) – **Bülter voraussichtlich im Zentrum, Waldschmidt als Option**
- [geissblog.koeln (10/2026) – Nach Kreuzband-Schock: Holt der FC einen vereinslosen Stürmer?](https://geissblog.koeln/2026/10/nach-kreuzband-schock-holt-der-fc-einen-vereinslosen-stuermer)
- [sky.de – Gladbach kommt bei Blessins Rückkehr nach St. Pauli nicht über ein Remis hinaus](https://sport.sky.de/fussball/artikel/borussia-moenchengladbach-kommt-bei-alexander-blessins-rueckkehr-nach-st-pauli-nicht-ueber-ein-remis-hinaus/13594718/34943) – **3-4-1-2 mit Kleindienst/Machino**

**Freiburg – Schalke**
- [badische-zeitung.de – Der SC Freiburg gewinnt sein Testspiel gegen den FC Luzern mit 4:2](https://www.badische-zeitung.de/der-sc-freiburg-gewinnt-sein-testspiel-gegen-den-fc-luzern-mit-4-2)
- [regiofussball.ch (04.10.2026) – FCL unterliegt Freiburg nach engagierter Leistung mit 2:4](https://regiofussball.ch/2026/10/04/fcl-unterliegt-freiburg-nach-engagierter-leistung-mit-24/) – **Luzerns Torschützen; Datierung weicht von meinem Vortagsstand ab**
- [sportschau.de – Sieg im Testspiel gegen Luzern: SC Freiburg weiter im Flow](https://www.sportschau.de/regional/swr/swr-sieg-im-testspiel-gegen-luzern-sc-freiburg-weiter-im-flow-100.html)
- [schalketotal.de (04.10.2026) – Schalke aufgepasst: Freiburg schießt sich für S04 warm](https://schalketotal.de/2026/10/04/schalke-aufgepasst-freiburg-schiesst-sich-fuer-s04-warm/) – **Freiburg Dritter, Schalke Elfter (Tabellengegenprobe)**
- [ligainsider.de – FC Schalke 04, voraussichtliche Aufstellung 2026/27](https://www.ligainsider.de/fc-schalke-04/13/) – **Liste mit Lasme und Gantenbein, von mir verworfen**

**Nationalmannschaft**
- [sportschau.de – Remis gegen Griechenland: Deutschland glänzt nur eine Halbzeit](https://www.sportschau.de/fussball/nationalmannschaft/deutschland-glaenzt-nur-eine-halbzeit-in-griechenland,spielbericht-nl-griechenland-deutschland-100.html)
- [spox.com – Deutschland kann Griechenland erneut nicht knacken](https://www.spox.com/fussball/live/dfb-team-live-griechenland-vs-deutschland-mit-juergen-klopp-heute-im-liveticker/blt2758f898b413f6e7)
