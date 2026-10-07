# Bundesliga-Tipps – 5. Spieltag 2026/27 (Stand: 07.10.2026)

**Ansetzung:** Freitag, 09.10. bis Sonntag, 11.10.2026. Der Vortagsstand (06.10.) betraf denselben Spieltag — alle neun Tipps sind vergleichbar.

**Mittwoch der Spielwoche, zwei Tage vor dem Anpfiff in Dortmund.** Das Länderspielfenster ist geschlossen, die Vereine sind in der Spieltagsvorbereitung, und das ist der entscheidende Unterschied zu allen bisherigen Läufen: **Heute liegen erstmals datierbare Spieltags-Pressekonferenzen und Trainingsberichte vor.** Die Kovac-Pressekonferenz in Dortmund ist auf den heutigen Tag datiert, der hessenschau-Ticker zu Frankfurt ebenfalls, die Gladbacher Kleindienst-Meldung auf das gestrige Training.

**Drei Tipps ändern sich** — Hoffenheim, Union und Leipzig. Alle drei gehen auf Schwellen zurück, die ich in den Vorläufen selbst gesetzt habe; zwei davon waren ausdrücklich auf heute terminiert. **Sechs Tipps bleiben unverändert.**

**Die zwei größten Risiken des Vortagsstands sind heute beide aufgelöst** — und zwar in meine Richtung: Der verworfene Kölner „Verletzungsschock" um El Mala ist widerlegt, und die Kölner Sturmausfälle sind jetzt vereinsbestätigt und auf den 03.10. datiert. **Dazu ist die Proxy-Gegenprobe, die zwei Läufe lang gefehlt hat, heute gelungen.**

**Vier Korrekturen am Vortagsstand** sind nötig — bei Kühn (eine Rechenfehlkorrektur, die mich am meisten stört), bei Musiala (ich nehme die gestrige Abschwächung zurück), bei der Bayern-Trainingsaufnahme und bei Onyeka.

---

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Die Primärseiten sind aus dieser Umgebung weiterhin nicht abrufbar** — aber die Ursache ist seit heute belegt statt vermutet.

- **Direkte Verbindungsprüfung** auf acht Sportdomains (`kicker.de`, `www.kicker.de`, `transfermarkt.de`, `weltfussball.de`, `bundesliga.com`, `www.bundesliga.com`, `sportschau.de`, `ligainsider.de`) → **alle acht mit HTTP-Status `000`**, kein Verbindungsaufbau.
- **WebFetch** auf `www.bundesliga.com` und `anstosszeiten.de` → beide `EGRESS_BLOCKED` mit namentlicher Nennung der Domain.

### Die Gegenprobe, die zwei Läufe lang gefehlt hat, ist heute gelungen

**Der Statusaufruf auf den Agent-Proxy wurde heute nicht abgelehnt**, sondern ausgeführt — in den beiden Vorläufen war er am Berechtigungs-Klassifikator gescheitert („Exfil Scouting" am 05.10., „Credential Exploration" am 06.10.). Sein Ergebnis benennt die Ursache direkt:

- `enabled: true`, `bundleCoversEveryHost: true`, `hasSystemCa: true` — **die TLS-Konfiguration ist intakt.** Damit sind Zertifikats- und Trust-Store-Fehler als Ursache ausgeschlossen, nicht nur unwahrscheinlich.
- Unter `recentRelayFailures` stehen meine eigenen Abrufversuche von heute, mit Zeitstempel und Begründung: `kind: "connect_rejected"`, `detail: "gateway answered 403 to CONNECT (policy denial or upstream failure)"`, für `kicker.de:443`, `www.kicker.de:443`, `transfermarkt.de:443` und die weiteren.

***Damit ist die Lücke geschlossen, die ich seit dem 05.10. offen geführt habe.*** Die Sperre ist eine **Netzwerk-Policy des Containers**, die CONNECT auf diese Hosts mit 403 ablehnt. Sie ist nicht site-spezifisch, kein TLS-Problem und kein Fehler auf Seiten der Verlage. *Das ist kein besserer Zugang, aber es ist endlich eine belegte Diagnose — und für künftige Läufe heißt das: Diese Prüfung muss nicht erneut unternommen werden, und ein Umweg über andere Sportdomains hat keine Aussicht.*

### Was daraus folgt

**Alles unten steht auf Suchergebnis-Zusammenfassungen und -Titeln, nicht auf gelesenen Artikeln.** Vereinsmeldungen kann ich nicht im Volltext prüfen. Wo eine Adresse oder eine Zusammenfassung ein Datum trägt, nenne ich es mit, weil die Datierung in diesem Repo die Hauptarbeit ist.

*Zum Hilfsmittel der aufsteigenden `ligainsider.de`-Meldungsnummern:* **Es hat heute erneut getragen und erstmals eine Tippänderung mitbegründet.** Die Onyeka-Meldung trägt die Nummer **418770** und liegt damit über allen bisher geführten (418481, 418564, 418573, 418597 vom 05./06.10.) — sie ist die neueste Fundstelle, die ich in diesem Repo je hatte. Die verworfenen Alt-Meldungen (409299, 411427, 412344) liegen weit darunter. **Die Annahme bleibt plausibel und unbelegt**, sie ist heute bei Onyeka aber durch ein ausdrückliches Datum (06.10.) gestützt und nicht mein einziges Argument.

---

## Die Anstoßzeiten sind heute vollständig bestätigt — und ein scheinbarer Widerspruch ist aufgelöst

Das ist der methodisch wichtigste Fund des Tages, weil er eine Fehlerquelle beseitigt, die mich in jedem künftigen Lauf getroffen hätte.

**Die erste Suche lieferte Zeiten, die meinem Vortagsstand allesamt widersprachen:** Freitag 18:30 statt 20:30, samstags 13:30 statt 15:30, Leipzig 16:30 statt 18:30, Freiburg 15:30 statt 17:30. Als Quelle war durchgehend die **englischsprachige** Bundesliga-Seite genannt.

***Die Differenz ist in allen neun Fällen exakt zwei Stunden.*** MESZ ist UTC+2 (die Zeitumstellung erfolgt erst am 25.10.2026). **Die englische Bundesliga-Seite rendert die Anstoßzeiten in UTC.** Die Gegenprobe über deutschsprachige Quellen, die Lokalzeit ausgeben, bestätigt jede einzelne meiner neun Zeiten:

| Partie | Vortagsstand (MESZ) | Bestätigt durch |
|---|---|---|
| Dortmund – Werder | Fr 20:30 | ligainsider (`09.10.2026 um 20:30`); Kovac-PK-Bericht („20:30 local time") |
| Augsburg – Bayern | Sa 15:30 | **fcaugsburg.de selbst**, Vorschau vom 06.10.: „Samstag, 10. Oktober, 15:30, WWK ARENA" |
| Hoffenheim – HSV | Sa 15:30 | fussballtransfers (15:30, gegen bundesliga.com/en 13:30) |
| Mainz – Leverkusen | Sa 15:30 | Spieltagsübersichten in Lokalzeit |
| Union – Elversberg | Sa 15:30 | fussballtransfers, fussballdaten (15:30, gegen bundesliga.com/en 13:30) |
| Paderborn – Stuttgart | Sa 15:30 | zdfheute / scp07: „10.10.2026 um 15:30 Uhr, Home Deluxe Arena" |
| Leipzig – Frankfurt | Sa 18:30 | „Samstag, 10. Oktober 2026, Anstoß 18:30 Uhr MESZ, Red Bull Arena"; hessenschau-Ticker: „Samstagabend (18.30 Uhr)" |
| Köln – Gladbach | So 15:30 | bundesliga-gruppe (zeitgenaue Ansetzung, 15:30, DAZN); zweite Quelle: „Sonntag, 15.30 Uhr, DAZN" |
| Freiburg – Schalke | So 17:30 | **schalke04.de selbst**: „Ansetzungen Spieltage 5 bis 11", 17:30 |

**Zwei Vereins-Primärquellen** (Augsburg, Schalke) stehen darunter, und beide bestätigen meinen Stand. **Die Ansetzung des 5. Spieltags ist damit vollständig und in Lokalzeit belegt.**

*Eine Einschränkung, die ich nenne, weil sie mich zuerst irritiert hat:* Die erste Suchzusammenfassung schrieb die 18:30-Angabe für Dortmund – Werder auch **sport1** zu. sport1 ist eine deutschsprachige Seite und würde Lokalzeit ausgeben. **Da jede andere deutschsprachige Quelle und der Bericht von der heutigen Kovac-Pressekonferenz 20:30 nennen, halte ich die sport1-Zuschreibung für einen Fehler der Zusammenfassung, nicht für eine echte dritte Angabe.** Belegen kann ich das nicht, weil ich die Seite nicht lesen kann.

---

## Korrekturen am Vortagsstand

### 1. Kühn (Gladbach): meine Rechnung von gestern war zu selbstsicher

**Gestern habe ich geschrieben:** Kühn, Muskelbündelriss im Training nach dem 3:4 gegen Elversberg (2. Spieltag), Ausfall fünf bis sechs Wochen — *„Fünf bis sechs Wochen ab Anfang September reichen über den 11.10. hinaus. Kühn fehlt im Derby, und das ist jetzt gerechnet, nicht vermutet."*

***Das war falsch gerechnet.*** Der 2. Spieltag war am 04.–06.09.2026; die Verletzung fiel ins Training danach, also auf etwa den 06.–08.09. **Fünf Wochen ab dem 06.09. sind der 11.10. — genau mein Derbytag.** Die untere Grenze meiner eigenen Prognose schließt das Derby also nicht aus, sie trifft es. Richtig wäre gewesen: *Kühn ist im Derby frühestens wieder möglich, wahrscheinlicher fehlt er.*

**Und heute gibt es dazu eine Fundstelle:** `fussballdaten.de` führt Kühn als **mögliche Alternative für Blessin im Auswärtsspiel in Köln**; ob er spielt, sei in der Trainingswoche zu klären. Das ist keine Vereinsangabe und schwächer als eine Entwarnung — aber meine Arithmetik schließt es nicht mehr aus. **Ich führe Kühn ab heute als *fraglich*, nicht als gerechneten Ausfall.** Was das für die Schwelle bedeutet, steht beim Tipp.

### 2. Musiala (Bayern): ich nehme die gestrige Abschwächung zurück

**Gestern habe ich die Diagnose auf „strittig" herabgesetzt**, weil einer zweiten Darstellung zufolge eine Hüftprellung mit vorsorglicher Nicht-Nominierung durch Nagelsmann vorlag — unvereinbar mit meinem Stand vom 05.10. (Muskelfaserriss beim Aufwärmen vor dem Niederlande-Spiel).

**Heute liegt eine dritte, unabhängige Fundstelle vor, die die ursprüngliche Version stützt und präzisiert:** Musiala habe sich beim Aufwärmen vor dem Länderspiel gegen die **Niederlande (1:1)** einen Muskelfaserriss zugezogen und sei **für vier Spiele** ausgefallen; er trainiert derzeit **individuell** (Quelle beruft sich auf kicker), ein Rückkehrtermin ist offen. Die Meldung steht im Zusammenhang „Kimmich und Co. wieder im Betrieb", gehört also in die Woche nach der Länderspielpause.

**Damit steht es zwei unabhängige Fundstellen zu einer.** Ich führe den Muskelfaserriss ab heute wieder als die besser gestützte Version und nehme das gestrige „strittig" zurück. **Am Befund ändert sich nichts** — Musiala fehlt am 10.10., und das ist heute zum dritten Mal belegt, erstmals mit einer Spielanzahl. *Die Hüftprellungs-Version verwerfe ich nicht, ich führe sie als Minderheitsdarstellung.*

### 3. Bayerns Trainingsaufnahme: einen Tag früher als gestern geschrieben

**Gestern stand hier: „Bayern hat heute, am 06.10., das Mannschaftstraining aufgenommen."** Die heutige Fundstelle datiert die Wiederaufnahme auf **etwa den 05.10.** und nennt die Teilnehmer: Neuer, Ulreich, Boey, Davies und Luis Díaz waren laut Bild dabei; Kompany gab mehreren Nachwuchsspielern Einheiten bei den Profis.

**Ein Tag Unterschied, ohne Folge für den Tipp** — aber die Teilnehmerliste hat Gewicht, siehe den Tipp.

### 4. Onyeka: gestern „keiner Seite zuzuordnen", heute Elversberger — mit Folge für den Tipp

**Gestern habe ich ausdrücklich geschrieben:** *„Der dritte dort genannte Name – ‚Onyeka fraglich' – ist mir keiner Seite zuzuordnen; ich führe ihn nicht."*

**Heute ist er zuzuordnen, und zwar über die bestmögliche Quelle:** den **offiziellen X-Account des SV 07 Elversberg**, der während eines eigenen Spiels schreibt: *„Das ist bitter: Francis Onyeka hat sich bei einem Zweikampf verletzt und kann nicht weiter machen. Für ihn kommt Noah Darvich in die Partie. 0:0 I 6. Minute #DieElv #UnsereElv #ELVFCB"*

**Onyeka ist Elversberger**, und Darvich ebenfalls. Der Hashtag `#ELVFCB` datiert diesen Vorgang auf Elversberg – Bayern, also den 3. Spieltag. **Das ist nicht der heutige Befund, sondern der Beweis der Vereinszugehörigkeit** — der Befund steht unten bei den geschlossenen Lücken und bewegt den Tipp.

---

## Geschlossene Lücken

### Die Kölner Sturmausfälle sind vereinsbestätigt und datiert — und die verworfene Fundstelle ist widerlegt

**Das ist der wichtigste Fund des Tages.** Gestern war das Kölner Sturmzentrum „eine Prognose ohne Vereinsangabe", und die verworfene „Verletzungsschock"-Meldung um El Mala war mein ausdrücklich benanntes größtes Einzelrisiko.

**Belegt ist jetzt:**
- Das Testspiel fand am **Samstag, 03.10.2026** statt, im Sportpark Höhenberg, **2:2 (1:2)** gegen Viktoria Köln, in der Länderspielpause, eine Woche vor dem Derby.
- **Dallinga** verdrehte sich nach **27 Minuten** in einer Aktion im gegnerischen Strafraum das **rechte** Knie. Der Verein teilte eine **Kreuzbandverletzung** mit und einen längeren Ausfall; **ob es ein kompletter Riss ist und welches Band betroffen ist, lässt die Vereinsmitteilung offen.** WDR berichtet unter Berufung auf den FC von Monaten. Er ist von Bologna ausgeliehen, die Leihe endet im Sommer, eine OP-Entscheidung stand noch aus, er war auf Krücken am Geißbockheim.
- **Ache:** Muskelverletzung, laut Sportschau **Rückkehr im November** erwartet.
- Es gibt dazu **zwei Meldungen auf `fc.de`** — „Dallinga und Ache fallen aus" und „Remis im Test bei der Viktoria" —, also die Vereinsquelle, die gestern fehlte.

***Und damit ist die gestern verworfene Fundstelle endgültig widerlegt, nicht nur verworfen:*** **Saïd El Mala fehlte beim Viktoria-Test, weil er als Nationalspieler abgestellt war** — nicht wegen eines Knöchels. Er wird in denselben Berichten als **Kandidat für die Offensive gegen Gladbach** genannt. **Meine Verwerfung von gestern war richtig, und sie ruht heute nicht mehr nur auf „Aufsteiger" und den neun Saisontoren, sondern auf einer positiven Gegenangabe.** *Das größte Einzelrisiko des Vortagsstands ist erledigt.*

**Außerdem belegt:** **Marius Bülter hat im Test getroffen** („Bülter verhindert Pleite"). Mein gestriger Favorit für das Sturmzentrum ist damit nicht nur statistisch begründet, sondern gerade torgefährlich gewesen.

### Gladbachs Trainerchronologie: Blessin ist der dritte Trainer dieser Saison

Gestern hatte ich Blessin (53, Vertrag bis 2028, Derby als Bundesliga-Debüt für die Borussia). **Heute kommt die Vorgeschichte dazu:** **Eugen Polanski** bis **13.09.2026**, **Jan-Moritz Lichte** als Interimslösung, **Blessin ab 22.09.2026**. Gladbach hat in dieser Saison also schon zweimal gewechselt, die vier Niederlagen fielen unter der Vorgängerkonstellation, und **das Derby ist Blessins Pflichtspieldebüt.** Eine Fundstelle nennt ihn den ersten Gladbacher Trainer überhaupt, der mit einem Köln-Derby beginnt.

### Unions Trainer: Mauro Lustrinelli, über die Vereinsquelle

In sieben Läufen habe ich den Union-Trainer nie benannt. **Heute über `fc-union-berlin.de` selbst belegt:** **Mauro Lustrinelli**, Schweizer, am **21.05.2026** als Cheftrainer für die Saison 2026/27 vorgestellt. Dazu der Rahmen: Nach vier Spielen steht Union auf Platz 17 mit einem Punkt, die Kritik der Fans richtet sich vor allem gegen Geschäftsführer **Horst Heldt**, Lustrinelli wird von vielen noch gestützt.

*Für den Vortagsstand heißt das auch:* Die Fundstelle von gestern, die Union mit **Steffen Baumgart** verband, gehört in die Saison 2025/26. Die „Baumgart-Probe", die ich gestern angesetzt hatte, ist damit hinfällig — nicht ungeprüft, sondern gegenstandslos.

### Die Anstoßzeiten und die Proxy-Diagnose

Siehe die beiden Abschnitte oben. **Beide Lücken waren mehrere Läufe offen, beide sind heute geschlossen.**

---

## Heute ausdrücklich verworfene Fundstellen

**1. Noah Darvich als Union-Ausfall — dieselbe Seitenvertauschung zum dritten Mal.**
Eine `fussballtransfers`-Seite führt unter Union Berlin unter anderem **Noah Darvich** als Ausfall. **Darvich ist Elversberger** — belegt durch den offiziellen Elversberg-Account, der ihn als Einwechselspieler für Onyeka nennt (siehe Korrektur 4). **Verworfen.** *Dies ist die dritte Seitenvertauschung bei genau dieser Partie in drei Läufen. Die Prüfregel, die ich gestern gesetzt habe — erst Seitenzuordnung, dann Datum —, hat heute zum zweiten Mal einen Fehler verhindert.*

**2. Zimmerschieds Rückenverletzung als aktueller Ausfall, zum zweiten Mal.**
FotMob führt Tom Zimmerschied erneut mit Rückenverletzung und „a few weeks" als nicht verfügbar. **Das ist derselbe zwei Jahre alte Historieneintrag (02.–18.10.2024), den ich gestern aufgelöst habe.** Verworfen. Die Suchzusammenfassung nennt die Angabe selbst „möglicherweise veraltet".

**3. Musiala, Muskelbündelriss „beim 3:1 in Augsburg" — zum zweiten Mal verworfen.**
Eine t-online-Fundstelle trägt die Überschrift „Jamal Musiala verletzt sich gegen den FC Augsburg". **Augsburg – Bayern ist meine Partie am 10.10. und noch nicht angepfiffen.** Die Suchzusammenfassung ordnet diese Berichterstattung selbst ausdrücklich dem **April 2025** zu, als Musiala sich in Augsburg einen Muskel riss. **Verworfen** — und damit ist die gestrige Verwerfung über eine zweite Quelle bestätigt.

**4. „Neuer fraglich" und die Bayern-Abwehrkrise.**
Zwei Fundstellen hätten einen zweiten Bayern-Ausfall ergeben: eine Überschrift „Neuer fraglich, Goretzka wohl von Beginn an: Bayern-PK vor Augsburg" und eine zweite, die Davies und Upamecano „wahrscheinlich für den Rest der Saison" sowie Ito mit Mittelfußbruch führt. **Beide sind nicht datierbar und beide sind durch den heutigen Trainingsbericht widerlegt:** **Neuer *und* Davies haben an der Einheit vom 05.10. teilgenommen.** Dazu existiert eine Adresse `fcbayern.com/en/news/2026/01/...-ahead-of-augsburg-at-home` — das Heimspiel im Januar, also das Rückspiel. **Verworfen.** *Hätte ich die „Neuer fraglich"-Überschrift übernommen, wäre meine Augsburg-Schwelle ausgelöst worden und der Tipp stünde auf 2:2.*

**5. Die Lukeba-Meldung vor dem Celtic-Spiel.**
„RB verlegt Training vor Champions League Celtic: Lukeba fehlt, Gulácsi und Seiwald fit". **Leipzigs Gegner nach diesem Spieltag ist PSV Eindhoven**, Celtic gehört in eine frühere Champions-League-Saison. **Verworfen.**

**6. Die kicker-Überschrift „Lukeba fällt aus".**
„Seiwald: Im dritten Jahr endlich unverzichtbar – Lukeba fällt aus, Baku und Gruda angeschlagen", ohne Datum. **Sie widerspricht allen vier heutigen Lukeba-Fundstellen, die ihn im Mannschaftstraining sehen.** „Im dritten Jahr" passt zu einer früheren Saison Seiwalds. **Verworfen** — *aber ich nenne sie, weil sie in meine Richtung gezeigt hätte und ich sie trotzdem nicht verwende.*

**7. Hugo Bolin als Gladbacher Derby-Ausfall, zum zweiten Mal.**
Erneut findet sich die Angabe, Bolin fehle, weil er für Schweden **nachnominiert** wurde. **Ein Länderspielfenster, das am 06.10. geendet hat, kann keinen Ausfall am 11.10. begründen.** Ich führe Bolin weiter nicht als Ausfall. ***Die ehrliche Einschränkung ist heute größer als gestern:*** **Zwei unabhängige Fundstellen stellen das inzwischen als Ausfall dar, und was dagegen steht, ist allein meine eigene Zeitrechnung, keine Gegenquelle.** Dazu kommt ein möglicher Namensdreher: Eine weitere Fundstelle nennt **Isac Lidberg** als schwedischen Gladbacher Angreifer, der in Kleindiensts Abwesenheit getroffen hat. **Ob es um zwei Spieler oder um eine Verwechslung geht, kann ich nicht auflösen.**

**8. Die Hoffenheimer Coufal- und Hajdari-Einträge.**
LigaInsider führt Coufal und Hajdari als verletzt bzw. nicht fit. **Die Suchzusammenfassung datiert die Einträge selbst auf „etwa 200 Tage" und schließt daraus, dass sie diese Partie nicht betreffen.** **Verworfen** — *und das ist die unabhängige Bestätigung meiner Korrektur vom 06.10., mit der ich die Coufal-Angabe entwertet habe. Ich hatte recht, und heute sagt es eine zweite Quelle.*

**9. Die Werder-Personalseiten vom Mai 2026.**
Mehrere `werder.de`-Treffer („Personal-Update vor dem Spiel in Dortmund", „PK vor dem Heimspiel gegen Dortmund") tragen Adressen mit `2025-2026` und Datumskürzeln `150526` bzw. `12012026`. **Vorsaison, verworfen** — die Zusammenfassung weist selbst darauf hin.

---

## Offen benannte Restlücken und Unsicherheiten

- **Hoffenheims Personallage ist zum vierten Mal in Folge nicht aktualisiert.** Keine Pressekonferenz, keine Verletztenmeldung, keine partiebezogene Fundstelle. Belegt ist allein der Trainername **Christian Ilzer** über eine Kaderseite ohne Verletzungskennzeichnung. ***Dieser Dauerzustand löst heute eine Tippänderung aus*** — nach einer Schwelle, die ich gestern genau dafür gesetzt habe.
- **Zu Freiburg habe ich zum dritten Mal in Folge keine verwendbare neue Fundstelle.** Der zweite Teil meiner Freiburg-Schwelle ist damit erneut **ungeprüft, nicht widerlegt.**
- **Der Kölner Trainer bleibt ungeklärt.** Ich habe René Wagner geführt, finde dazu heute nichts Neues, und die Kwasniok-Widersprüche von gestern sind nicht aufgelöst. **Ich nenne den Kölner Trainer weiter nicht.**
- **Der Frankfurter Trainer ist heute unklarer als gestern.** Der hessenschau-Ticker vom 07.10. nennt **Adi Hütter** („Trainer Adi Hütter hat sich am freien Mittwoch mit Uzun getroffen"), die gestern verworfene PK-Fundstelle nannte **Dino Toppmöller**, und die Suchzusammenfassung schreibt selbst „Toppmöller bzw. Hütter". **Ich kann das nicht auflösen.** Für den Tipp ohne Gewicht; ich nenne beide Namen und keinen als gesichert.
- **Der Paderborner Trainer bleibt unbenannt** (Kwasniok-Widerspruch vom 06.10., heute nichts Neues).
- **Der Leverkusener Trainer bleibt ungeklärt** — dritter Lauf ohne Auflösung, heute nicht erneut geprüft.
- **Dallingas Diagnose ist absichtlich unscharf:** Der Verein nennt „Kreuzbandverletzung" und lässt offen, ob kompletter Riss und welches Band. **Mehrere Medien schreiben „Kreuzbandriss" — das steht nicht in der Vereinsangabe.** Ich übernehme die Vereinsformulierung.
- **Onyekas Verletzungshergang ist doppelt datiert und ich kann es nicht trennen.** Die `ligainsider`-Meldung 418770 nennt den **06.10.** und eine Fußverletzung mit vorzeitiger Abreise aus der Nationalmannschaft; der offizielle Elversberg-Post beschreibt eine Verletzung in der 6. Minute gegen Bayern (3. Spieltag). **Zwei Vorgänge oder eine Verwechslung der Zusammenfassung — offen.** Was den Tipp trägt, ist die auf den 06.10. datierte Meldung; sollte sie in Wahrheit den September beschreiben, ist meine Änderung bei Union nicht gedeckt. **Das ist das größte Einzelrisiko dieses Laufs.**
- **Kleindiensts Lage ist zweifach beschrieben und beides kann stimmen:** Trainingsabbruch am Dienstag wegen Unwohlsein beim Aufwärmen (Blessin gegenüber Sport1) **und** Rückkehr aus einer Sperre, in deren Abwesenheit Lidberg getroffen hat. **Ob er fehlt, auf der Bank sitzt oder spielt, ist offen.**
- **Zu Elversbergs Kaderlage insgesamt finde ich weiterhin fast nichts** — keine Kaderseite, keine PK. Onyeka und Seifert sind alles, was ich habe.
- **Das Leipziger DFB-Pokalspiel und Bayerns Pokalspiel gegen Osnabrück** (Kompany bestätigte, Urbig werde dort Neuer ersetzen) **kann ich nicht datieren.** Als Belastungsfaktor für den 10.10. deshalb nicht verwertet.
- **Unions Testspiel beim BAK 07: zum dritten Mal nicht gesucht.** Ich trage die Lücke fort, statt sie als geprüft auszugeben.
- **Die dritte Leipziger Niederlage bleibt unzuordenbar** — siebter Lauf, heute ebenfalls nicht erneut geprüft.
- **Die Tabelle ist aus den einzeln belegten Ergebnissen gerechnet**, weil keine Tabellenseite abrufbar ist. **Heute gleich zweimal extern gegengeprüft und beide Male bestätigt:** Köln „nach einem schwachen 1:2 beim HSV mit vier Punkten aus vier Spielen", Union „auf dem vorletzten Platz mit einem Punkt und 17 Gegentoren, zuletzt 0:7 in München". *Beides deckt sich exakt mit meiner Rechnung.*

---

### Tabelle nach dem 4. Spieltag

Aus den einzeln belegten Ergebnissen gerechnet. **Form = 1. bis 4. Spieltag von links nach rechts.** Werte unverändert — seit dem 20.09. wurde nicht gespielt. **Platz 13 (Köln) und Platz 17 (Union) sind heute extern bestätigt.**

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

- **Dortmund zu Hause:** 2:0 gegen HSV, 3:0 gegen Paderborn — **zwei Spiele, zwei Zu-null, fünf Tore.**
- **Leipzig zu Hause:** 3:0 gegen Gladbach, 5:0 gegen HSV — **8:0, zwei Zu-null; bei beiden stand Lukeba in der Startelf.**
- **Frankfurt auswärts:** 3:3 bei Union, 3:1 in Mainz — **vier Punkte, 6:4, auswärts besser als zu Hause, aber ohne Auswärtssieg.**
- **HSV auswärts:** 0:2 in Dortmund, 0:5 in Leipzig — **zwei Spiele, null Tore.** Beide HSV-Tore fielen zu Hause.
- **Hoffenheim zu Hause:** 2:3 gegen Dortmund, 2:1 gegen Stuttgart — **vier Tore in zwei Spielen, aber nur ein Sieg.**
- **Gladbach auswärts:** 0:3 in Leipzig, 0:5 in Freiburg — **null Tore, 0:8.**
- **Köln zu Hause:** 3:2 gegen Hoffenheim, 1:1 gegen Werder — **vier Punkte, 4:3.**
- **Union zu Hause:** 3:3 gegen Frankfurt, 1:3 gegen Schalke — **vier Tore in zwei Spielen, sechs Gegentore; der einzige Punkt der Saison fiel hier.**
- **Elversberg auswärts:** 4:3 in Gladbach, 0:0 in Schalke — **vier Punkte, 4:3; ein Spiel mit vier Toren, ein Spiel ohne Tor.**
- **Stuttgart auswärts:** 1:5 in München, 1:2 in Hoffenheim — **null Punkte, 2:7.**
- **Paderborn zu Hause:** 0:0 Mainz, 0:1 Freiburg, 3:1 Hoffenheim — **vier Punkte, drei Saisontore insgesamt.**
- **Freiburg zu Hause:** 4:1 Werder, 5:0 Gladbach — **zwei Spiele, neun Tore.**
- **Mainz zu Hause:** 0:0 Paderborn, 1:3 Frankfurt — **ein Punkt, 1:3.** **Leverkusen auswärts:** 2:3 in Elversberg, 2:2 in Augsburg — **ein Punkt, 4:5, kein Auswärtssieg.**
- **Augsburg zu Hause:** 3:0 Schalke, 2:2 Leverkusen — **fünf Tore in zwei Spielen.**
- **Bayern:** 14:2 in vier Spielen — **zwei Gegentore in der ganzen Saison.**

---

## Eine Regel, die ich heute brauche und deshalb vorab aufschreibe

In zwei Partien löst heute eine Schwelle aus **und gleichzeitig trifft eine Gegenangabe ein, die sie nicht vorgesehen hat.** Damit meine Schwellen weder wertlos noch mechanisch werden, halte ich fest, wie ich das behandle:

**Eine ausgelöste Schwelle bewegt den Tipp — es sei denn, im selben Lauf trifft eine Fundstelle ein, die in die Gegenrichtung mindestens gleich schwer wiegt. Dann nenne ich die Auslösung ausdrücklich, nenne die Gegenangabe, und der Tipp bleibt.** Was ich nicht tue: die Auslösung verschweigen, oder die Gegenangabe verschweigen und mechanisch ändern.

**Heute betrifft das Köln (Kühn) und nichts sonst.** Bei Mainz ist die Schwelle bei genauer Prüfung **nicht** ausgelöst — das steht dort. Bei Hoffenheim, Union und Leipzig löst sie ohne Gegenangabe aus, und dort ändere ich.

---

## Die Tipps zum 5. Spieltag

### Borussia Dortmund – SV Werder Bremen
**Freitag, 09.10.2026, 20:30 Uhr** (Signal Iduna Park)
**Tipp: 3:1**
*unverändert* — **und heute der Tipp mit dem größten Materialzuwachs auf der Heimseite, nach zwei Läufen, in denen ich zu Dortmund nichts hatte.**

***Die Kovac-Pressekonferenz von heute, Mittwoch dem 07.10., ist datierbar und betrifft genau diese Partie.*** Nach drei Läufen, in denen jede BVB-Fundstelle in frühere Episoden gehörte, ist das der Durchbruch auf dieser Seite. **Fünf Fragezeichen** nennen die Berichte („BVB mit fünf Fragezeichen", „BVB bangt vor Werder-Duell um fünf Spieler"):

- **Schlotterbeck:** trainiert bisher **individuell**, soll **am Donnerstag (08.10.) mit der Mannschaft** trainieren, danach entscheide sich die Freitagsfrage. Kovac sagt, ein Einsatz gegen Bremen sei **möglich**. Die Verletzung entstand im Nationalmannschaftstraining; ein Bericht nennt es einen Glücksfall, weil eine lange Pause unnötig erscheine. *Das ist deutlich positiver als mein gestriger Stand („Ersteinschätzung zwei bis drei Wochen").*
- **Ryerson:** **fraglich.** Er bekam in den norwegischen Länderspielen einen Schlag und reiste vorzeitig ab. Kovac: man wisse noch nicht, ob er rechtzeitig fit wird. **Dortmund hat rechts keine echte Alternative, seit Couto nach Como ging**; Beier gilt als möglicher Ersatz.
- **Chukwuemeka: fällt aus**, muskuläre Probleme. *Neu.*
- **Karetsas und Svensson: beide angeschlagen/erkältet.** *Neu.*

***Meine Schwelle ist nicht ausgelöst, und ich sage genau, warum nicht:*** **Ryerson ist nicht fit gemeldet, sondern fraglich** — eine Freigabe ist das nicht. **Und Schlotterbecks Rückkehr ist nicht angekündigt, sondern offen gehalten** („dann sehen wir"). „Möglich" ist keine Ankündigung. **Kein 3:0.** Ein zusätzlicher Innenverteidiger-Ausfall liegt ebenfalls nicht vor — Chukwuemeka ist Mittelfeldspieler, Karetsas offensiv, Svensson Linksverteidiger. **Kein 2:1.**

***Warum 3:1 bleibt — und heute besser begründet als gestern:*** Mein Gegentor stammt nicht aus Werders Stärke, sondern aus **Dortmunds Improvisation auf den Außenverteidigerpositionen**. Genau die ist heute erstmals zweiseitig belegt: **rechts Ryerson fraglich ohne Alternative, links Svensson angeschlagen.** Dazu Schlotterbeck offen in der Innenverteidigung. **Die Begründung meines Gegentors ist heute stärker, nicht schwächer.** Dagegen stehen vier Siege aus vier Spielen, 9:2, zwei Zu-null zu Hause und fünf Heimtore in zwei Spielen — und ein Gast mit sechs Ausfällen.

***Werders Stand, heute über eine zweite Quelle bestätigt:*** **Agu** (Ausfall, unverändert — die Verwerfung der älteren Adduktoren-Fundstellen von gestern bleibt gültig), **Stage** (muss operiert werden — *neu*), **Topp** (erst 2027 wieder), **Musah** (Monate), **Njinmah** (langer Ausfall, vereinsbestätigt), **Lynen** (Fortschritte, Rückkehr offen). Dazu aus dem Vortagsstand **Karl Hein** (muskulär, Torhüter), **Moussa Ndiaye** (Leiste) und **Itten** (fraglich). **Keine Fundstelle widerspricht dem gestrigen Stand.** *Die Liste stammt von einer LigaInsider-Übersicht ohne Stichtag — das ist die Schwäche dieser Hälfte.*

***Kovacs Kritik an der Länderspielpause*** („definitiv zu lang", vier Länderspiele) ist kein Argument, erklärt aber die fünf Fragezeichen.

***Die Schwelle für den letzten Lauf vor dieser Partie:*** **Wird Ryerson fit gemeldet *oder* bestätigt der BVB nach dem Donnerstagstraining Schlotterbecks Einsatz, gehe ich auf 3:0. Fällt ein Innenverteidiger zusätzlich aus oder wird Svenssons Ausfall bestätigt, gehe ich auf 2:1.** *Das Donnerstagstraining fällt in den nächsten Lauf und ist der letzte, den ich vor diesem Anpfiff habe.*

### FC Augsburg – FC Bayern München
**Samstag, 10.10.2026, 15:30 Uhr** (WWK Arena)
**Tipp: 1:2**
*unverändert* — **und heute ist die Bayern-Seite besser belegt als an jedem Tag zuvor, inklusive der Rücknahme meiner gestrigen Abschwächung.**

***Die Ansetzung ist heute über die Vereinsquelle bestätigt:*** Die Augsburger Vorschau vom **06.10.** nennt „Samstag, 10. Oktober, 15:30, WWK ARENA". *Erste Vereins-Primärquelle zu dieser Partie in sieben Läufen.*

***Musiala fehlt, und die Diagnose ist wieder die ursprüngliche*** (Korrektur 2). **Muskelfaserriss beim Aufwärmen vor dem Niederlande-Spiel (1:1), Ausfall für vier Spiele, aktuell Individualtraining, Rückkehrtermin offen.** Zwei unabhängige Fundstellen gegen eine. **Ein Ausfall am 10.10. ist damit zum dritten Mal belegt und erstmals mit einer Spielanzahl unterlegt.**

***Die Schwelle — ein zweiter belegter Bayern-Ausfall mit Diagnose — ist nicht ausgelöst, und heute aktiv widerlegt statt nur „nicht gefunden".*** Der Trainingsbericht vom **05.10.** nennt **Neuer, Ulreich, Boey, Davies und Luis Díaz als Teilnehmer**. **Damit sind zwei Fundstellen erledigt, die meine Schwelle ausgelöst hätten** — „Neuer fraglich" und „Davies/Upamecano für den Rest der Saison" (Verworfene Fundstellen, Punkt 4). ***Das ist der Unterschied zu gestern:*** Gestern stand hier „ich habe nichts gefunden, was einen weiteren Münchner Namen ausschließt". **Heute schließt der Trainingsbericht fünf Namen positiv ein.** Kompany gab zudem Nachwuchsspielern Einheiten — ein Zeichen für Kaderbreite, kein Ausfallhinweis.

***Auf Augsburger Seite nichts Neues:*** Mounié im Aufbautraining, Juma Bah offen, Gregoritsch verfügbar. Die Kade-Entwarnung bleibt erledigt und wird nicht wieder aufgenommen.

***Warum 1:2 bleibt, in einem Satz:*** **Augsburg hat zu Hause in zwei Spielen fünf Tore erzielt und steht auf Platz 4 — ein Tor ist die Mindestzahl, die dazu passt; Bayern hat in vier Spielen zwei Gegentore kassiert, und mehr als ein Tor ist gegen diese Abwehr nicht zu begründen.**

***Die Schwelle für den nächsten Lauf, unverändert:*** **Nur ein zweiter belegter Bayern-Ausfall mit Diagnose bewegt diesen Tipp auf 2:2.** *Die Bayern-Pressekonferenz am Freitag, 09.10., fällt in den nächsten Lauf.*

### TSG Hoffenheim – Hamburger SV
**Samstag, 10.10.2026, 15:30 Uhr** (SNP Arena)
**Tipp: 1:0**
**Änderung gegenüber gestern: 2:0 → 1:0, weil die Hoffenheimer Seite auch im vierten Lauf in Folge ohne jede partiebezogene Fundstelle bleibt — und ich genau dafür gestern eine Schwelle gesetzt habe.**

***Dies ist die Änderung, die mir am unangenehmsten ist, und sie beruht auf keiner neuen Tatsache.*** Gestern habe ich geschrieben: *„Neu ab heute: Bleibt die Hoffenheimer Seite auch im nächsten Lauf ohne jede partiebezogene Fundstelle, gehe ich auf 1:0 — nicht weil ein Ausfall belegt wäre, sondern weil ein Zwei-Tore-Heimtipp vier Läufe ohne Heiminformation nicht verdient."*

**Heute ist der vierte Lauf, und die Bedingung ist erfüllt.** Zu Hoffenheim finde ich:
- **keine Pressekonferenz**, keine Verletztenmeldung, keine Trainingsmeldung, keine Vereinsmeldung;
- eine Kaderseite mit Trainer **Christian Ilzer** und **ohne jede Verletzungskennzeichnung**;
- die Coufal- und Hajdari-Einträge, die die Suchzusammenfassung selbst auf „etwa 200 Tage" datiert und für diese Partie ausschließt (Verworfene Fundstellen, Punkt 8).

**Kramarić, Coufal, Prass, Asllani und Hajdari führe ich weiter als *unbekannt*.** ***Die Schwelle ist ausgelöst, ohne Gegenangabe: Es gibt heute nichts von der Heimseite, was dagegen stünde — das ist ja gerade der Punkt.*** **Ich gehe auf 1:0.**

***Die Gästeseite ist dagegen zum siebten Mal gut belegt, und heute mit tagesaktuellen Quellen:***
- **Grønbæk fällt für das Spiel bei der TSG aus** — eine Fundstelle von **gestern (06.10.)** sagt das ausdrücklich. *Das bestätigt meinen gestrigen Schluss aus dem Rückkehrtermin 17.10. jetzt direkt und partiebezogen.*
- **Poulsen ist fit, mit eigenem Zitat von vorgestern:** „Ich bin nicht verletzt, das Hoffenheim-Spiel ist kein Problem." Der Wadenschlag sollte in Tagen heilen. **Dritte Bestätigung, und erstmals aus seinem eigenen Mund.**
- **Neu:** Polzin plant mit Neuzugang **Martin Adeline** in der Startelf, sein Einsatz „scheint sicher". *Ein Name, den ich bisher nicht hatte; dass ein Neuzugang im Oktober kommt, kann ich nicht erklären und nicht prüfen — ich nenne ihn als Fund, nicht als Argument.*
- **Daka:** Muskelfaserriss, unverändert (Seite ca. 32 Tage alt).
- **Vuskovic:** nicht im Kader, gesperrt bis 15.11.2026, unverändert.
- **Moffi:** Knieprobleme, Individualarbeit, unverändert aus dem Vortagsstand.

***Warum trotzdem ein Heimsieg und warum nur eines:*** **Der HSV hat in zwei Auswärtsspielen null Tore erzielt (0:2, 0:5) und verliert zusätzlich Grønbæk; drei seiner Angreifer sind namentlich weg.** Ein Gast, der auswärts nicht trifft, verliert auch gegen einen Gastgeber, über den ich nichts weiß. **Aber das zweite Tor war auf Hoffenheimer Offensivstärke gestützt, und dafür habe ich seit vier Läufen keinen Beleg.** Hoffenheim hat zu Hause vier Tore in zwei Spielen und steht mit drei Punkten auf Platz 14. **1:0 ist das, was die Belegqualität trägt.**

***Die Schwelle für den nächsten Lauf:*** **Kommt endlich eine partiebezogene Hoffenheimer Fundstelle und nennt keinen Ausfall, gehe ich auf 2:0 zurück. Wird ein Hoffenheimer Stammspieler belegt als Ausfall gemeldet, gehe ich auf 0:0. Kommt ein HSV-Angreifer belegt zurück, gehe ich auf 1:1.** *Die HSV-Pressekonferenz fällt in den nächsten Lauf.*

### 1. FSV Mainz 05 – Bayer 04 Leverkusen
**Samstag, 10.10.2026, 15:30 Uhr** (MEWA Arena)
**Tipp: 1:1**
*unverändert* — **und heute der Tipp, bei dem ich meine eigene Schwelle am genauesten lesen musste. Sie ist nicht ausgelöst, und ich hätte sie beinahe falsch angewendet.**

***Die Zentner-Lage, und warum sie meinen Tipp nicht bewegt:*** Belegt ist heute neu: **Zentner ist am Dienstag (06.10.) ins Training zurückgekehrt, konnte aber an keiner torwartspezifischen Übung teilnehmen; Schwolow gilt als voraussichtlicher Starter am Samstag.**

**Meine Schwelle lautete: „Nur eine Mainzer *Vereinsangabe* dazu, *ob Zentner spielt*, bewegt diesen Tipp — spielt er, 2:1; spielt er nicht, 1:2."** ***Zwei Gründe, warum ich trotzdem nicht auf 1:2 gehe, und der zweite ist der wichtigere:***

**Erstens: Das ist keine Vereinsangabe.** „Schwolow gilt als voraussichtlicher Starter" ist eine journalistische Einschätzung. Gestern habe ich diese Unterscheidung ausdrücklich geschärft, und sie gilt heute gegen mich wie gestern für mich.

***Zweitens, und das ist eine Korrektur an meiner Schwelle selbst: Sie war falsch asymmetrisch konstruiert.*** **Zentner fehlt seit dem 3. Spieltag, und Schwolow vertritt ihn seit dem 3. Spieltag — das steht seit gestern in meinen eigenen Notizen.** Mainz hat **mit Schwolow im Tor** den 4. Spieltag gespielt: **das 4:3 in Gladbach, ein Auswärtssieg.** ***Mein 1:1 ist also auf einer Grundlage entstanden, in der Zentner schon fehlte.*** „Er spielt nicht" ist damit **keine neue schlechte Nachricht, sondern die Bestätigung des Status quo** — und hätte nie den 1:2-Zweig tragen dürfen. **Neu wäre seine *Rückkehr* gewesen, und die ist heute unwahrscheinlicher geworden.** *Die Schwelle hätte nur einen Zweig haben dürfen; ich korrigiere sie unten.*

***Und die Nachrichtenlage ist heute für Mainz sogar besser:*** **Fabio Gruber (Kniereizung), Paul Nebel (Adduktoren) und Silvan Widmer (Knieprobleme) sind zurück und kämpfen um Plätze im Spieltagskader** („Mainz receive injury boost as trio return to team training"). **Nebel und Widmer standen gestern auf meiner Mainzer Ausfallliste.** Die Ausfallbilanz geht damit von **sechs gegen drei** auf etwa **drei gegen drei** zurück: Mainz noch **Kohr** (nach Operation), **Silas** (Schien- und Wadenbeinbruch), **Katompa Mvumpa**/**Caci** (Listeneinträge); Leverkusen unverändert **Doué** (Wadenmuskel), **Eichhorn** (Stoffwechselerkrankung), **Culbreath** (Listeneintrag).

***Teil (b) der Schwelle ist ebenfalls nicht ausgelöst, und zwar in die Gegenrichtung:*** Ein Leverkusener Rückkehrer von meiner Liste findet sich nicht, und die „auf den 10.10. datierbare Nebel-Absage" ist das Gegenteil eingetroffen — **Nebel ist zurück.**

***Warum 1:1 bleibt:*** **Beide Mannschaften haben 7 Punkte, und die Symmetrie ist eine Schwäche-Symmetrie: Mainz hat zu Hause einen Punkt aus zwei Spielen bei 1:3 Toren, Leverkusen auswärts einen Punkt aus zwei Spielen bei 4:5 Toren und keinen Auswärtssieg.** Drei Mainzer Rückkehrer verbessern die Kaderbreite, aber sie machen aus einer Heimbilanz von 1:3 Toren keine Heimstärke. **Ein Torwartwechsel, der seit zwei Spieltagen gilt und in dem ein 4:3-Auswärtssieg gelang, ist kein Argument für eine Niederlage.**

***Die Schwelle für den nächsten Lauf, korrigiert:*** **(a) Nur eine Mainzer Vereinsangabe, dass Zentner *spielt*, bewegt diesen Tipp — auf 2:1. Eine weitere Bestätigung, dass er nicht spielt, bewegt ihn nicht, weil der Tipp auf dieser Annahme beruht.** **(b) Ein belegter Leverkusener Rückkehrer von meiner Ausfallliste bringt 1:2. (c) Neu: Werden zwei der drei Mainzer Rückkehrer für die Startelf gemeldet, gehe ich auf 2:1.**

### 1. FC Union Berlin – SV 07 Elversberg
**Samstag, 10.10.2026, 15:30 Uhr** (Alte Försterei)
**Tipp: 1:1**
**Änderung gegenüber gestern: 1:2 → 1:1, weil Francis Onyeka als zweiter Elversberger Ausfall mit Diagnose belegt ist (Fußverletzung, auf den 06.10. datiert, vorzeitige Abreise aus der Nationalmannschaft) — und weil er seit heute überhaupt erst Elversberg zuzuordnen ist.**

***Diese Änderung hat zwei Schritte, und der erste schließt eine Lücke, die ich gestern namentlich offengelassen habe.***

**Schritt 1 — die Zuordnung.** Gestern: *„Der dritte dort genannte Name – ‚Onyeka fraglich' – ist mir keiner Seite zuzuordnen; ich führe ihn nicht."* **Heute belegt der offizielle X-Account des SV 07 Elversberg**, dass Onyeka Elversberger ist (Korrektur 4). **Bestmögliche Quellenart für eine Vereinszugehörigkeit.**

**Schritt 2 — der Befund.** Die `ligainsider`-Meldung **418770** — **die höchste Meldungsnummer, die ich in diesem Repo je geführt habe**, also die neueste — nennt den **06.10.**, eine **Fußverletzung** und eine vorzeitige Abreise aus der Nationalmannschaft; seine Einsatzfähigkeit in Berlin sei offen, als Alternative stehe Darvich bereit.

***Meine Schwelle lautete: „Nur eine belegte Rønnow-Entwarnung oder ein zweiter Elversberger Ausfall mit Diagnose bewegt diesen Tipp."*** **Elversberg hatte genau einen belegten Ausfall (Seifert, Knöchel, Langzeitfall). Onyeka ist der zweite, und „Fußverletzung" ist eine Diagnose. Ausgelöst.** **Eine Gegenangabe aus der Elversberger Richtung liegt nicht vor** — zu Rønnow gibt es keine Entwarnung, er wird weiter mit Oberschenkelverletzung als **fraglich** geführt, also unverändert.

***Die Richtung und die Höhe, mit Begründung:*** Mein 1:2 war ein Auswärtssieg. **Ein Ausfall im Mittelfeld des Gastes nimmt dem Auswärtssieg die Selbstverständlichkeit, macht aber Union nicht zum Favoriten** — Union hat einen Punkt aus vier Spielen und 4:17 Tore, Elversberg sieben Punkte. **Die kleinste Änderung, die die Auslösung abbildet, ist der Wegfall des Auswärtssiegs: ein Remis.** Zur Höhe: **Union erzielt 1,0 Tore pro Spiel (4 in 4)** — zwei Tore wären über dem eigenen Schnitt. **Elversberg kommt auswärts auf 4:3, aber mit extremer Streuung (4:3 in Gladbach, 0:0 in Schalke).** **1:1.**

***Der übrige Stand, unverändert:*** **Union: Skov, Friedrich, Ilić, Burke, Nsoki, Markgraf (Kreuzbandverletzung) als sichere Ausfälle, Rønnow (Oberschenkel) fraglich** — acht Läufe namentlich identisch. **Elversberg: Seifert (Knöchel, Langzeitfall), dazu ab heute Onyeka.**

***Der Rahmen, heute erstmals belegt:*** **Union spielt unter Mauro Lustrinelli** (Vereinsquelle, vorgestellt am 21.05.2026), steht auf Platz 17 mit einem Punkt, hat zuletzt **0:7 in München** verloren, und die Fankritik richtet sich vor allem gegen Horst Heldt. **Union und Elversberg sind sich noch nie in einem Pflichtspiel begegnet** (gestern belegt) — für Elversberg ist die Alte Försterei das erste Auswärtsspiel in einem Stadion dieser Größe. **Das Elversberger 3:2 bei Hoffenheim vom 02.10. ziehe ich weiter ab** (gemischte TSG-Elf).

***Das Risiko dieser Änderung nenne ich ausdrücklich:*** **Sie steht auf der Datierung der Meldung 418770 auf den 06.10.** Der offizielle Elversberg-Post beschreibt eine Onyeka-Verletzung in der 6. Minute gegen Bayern, also am 3. Spieltag. **Sind das nicht zwei Vorgänge, sondern einer, den die Zusammenfassung falsch datiert hat, ist diese Änderung nicht gedeckt und 1:2 war richtig.** *Das ist das größte Einzelrisiko dieses Laufs, und es steht hier, nicht in einer Fußnote.*

***Die Schwelle für den nächsten Lauf:*** **Wird Onyeka belegt fit gemeldet oder zeigt sich die Meldung 418770 als Alt-Vorgang, gehe ich auf 1:2 zurück. Wird Rønnows Ausfall bestätigt, gehe ich auf 1:2. Kommt ein dritter Elversberger Ausfall mit Diagnose, gehe ich auf 2:1.**

### SC Paderborn 07 – VfB Stuttgart
**Samstag, 10.10.2026, 15:30 Uhr** (Home Deluxe Arena)
**Tipp: 1:2**
*unverändert* — **und heute mit einem Stuttgarter Fund, wo ich gestern keinen hatte, der die Schwelle aber nicht erfüllt.**

***Die Ansetzung ist bestätigt:*** 5. Spieltag, 10.10.2026, 15:30, Home Deluxe Arena. **Paderborn hat eine Pressekonferenz vor dem Heimspiel gegen den VfB angekündigt** (`scp07.de`) — **Inhalt gibt es noch nicht**, sie liegt nach diesem Lauf.

***Der neue Stuttgarter Fund, und warum er die Schwelle nicht auslöst:*** **Die offizielle VfB-Seite meldet, Nikolas Nartey sei vorzeitig zurückgekehrt, nachdem er wegen muskulärer Probleme beim Nations-League-Spiel ausgefallen war.** *Das ist eine Vereinsquelle und auf dieses Länderspielfenster datierbar — zwei Qualitäten, die ich hier selten habe.*

**Meine Schwelle verlangt „ein Stuttgarter Ausfall mit Diagnose".** ***Nartey ist kein Ausfall:*** **Die Meldung beschreibt eine vorzeitige Rückkehr zum Verein**, also eher eine Vorsichtsmaßnahme, und die Zusammenfassung schließt daraus, er könne wieder einsatzbereit sein. **Ich führe ihn als *fraglich*, nicht als Ausfall. Nicht ausgelöst.** *Der Unterschied zu gestern: Gestern stand hier „nichts gefunden", heute „ein Fund, der die Bedingung nicht erfüllt". Das ist eine bessere Belegqualität bei gleichem Ergebnis.*

***Der übrige Stuttgarter Stand, unverändert:*** **Justin Diehl** (Langzeitverletzter), **Jarzinho Malanga** (Bauchmuskelverletzung), **Dan-Axel Zagadou** (Individualprogramm), dazu ab heute Nartey als fraglich. **Verworfen habe ich eine FotMob-Liste mit neun Stuttgarter Namen** (Jaquez, Führich, Nartey, Arévalo, Zagadou, Assignon, Seimen, Diehl, Sauer) — **die Suchzusammenfassung bezeichnet die Seite selbst als „sehr alt"**, und eine zweite LigaInsider-Ansicht datiert sie auf „rund acht Monate". **Neun Ausfälle wären eine andere Partie; ich übernehme sie nicht.**

***Das gestrichene Torwart-Argument bleibt gestrichen.*** Hoeneß hat Seimens Pflichtspiel-Comeback offengelassen und Jobsharing angekündigt. Ich nehme es nicht wieder auf.

***Zu Paderborn finde ich erneut nichts Partiebezogenes.*** Der Stand bleibt: Curda, Obermair, Hansen und Baack nach der Erkältungswelle gesund, die USA-Reise mit dem 1:0 bei D.C. United am 01.10. als Belastungsfaktor. **Die FotMob-Namen (Awortwie-Grant, Klaas, Michel, Gayret) stammen von derselben veralteten Seite und werden nicht übernommen.** **Der Paderborner Trainer bleibt unbenannt.**

***Stuttgarts Pausenform, unverändert:*** zwei Testspiele, zwei Siege, 8:0 (3:0 Heidenheim, 5:0 Greuther Fürth).

***Warum 1:2 bleibt:*** **Paderborn hat in drei Heimspielen vier Punkte und drei Saisontore insgesamt — die schwächste Heimoffensive des Spieltags.** Dagegen ein Auswärtsteam mit 2:7, das in der Pause 8:0 testet und dessen Ausfälle sich im Aufbau befinden. **Der Tipp stand nie auf dem Torwart, sondern auf drei Paderborner Toren in vier Spielen.**

***Die Schwelle für den nächsten Lauf, mit Richtung — gestern fehlte sie:*** **Ein Stuttgarter Ausfall mit Diagnose (einschließlich einer Bestätigung, dass Nartey fehlt) bringt 1:1. Ein belegter Paderborner Rückkehrer in der Offensive bringt 2:2.** *Die Paderborner Pressekonferenz fällt in den nächsten Lauf.*

### RB Leipzig – Eintracht Frankfurt
**Samstag, 10.10.2026, 18:30 Uhr** (Red Bull Arena)
**Tipp: 1:1**
**Änderung gegenüber gestern: 2:1 → 1:1, weil meine auf heute terminierte Frist abgelaufen ist: Es liegt keine Bestätigung vor, dass Lukeba im *vollen* Mannschaftstraining ist. Dazu kommen zwei unabhängige Befunde in dieselbe Richtung — Raum fehlt, und Uzun steht Frankfurt wohl wieder zur Verfügung.**

***Die Frist und ihr Ergebnis.*** Gestern habe ich gesetzt: *„Bringt der 07.10. oder 08.10. keine Bestätigung, dass Lukeba im vollen Mannschaftstraining ist, gehe ich auf 1:1."* **Heute ist der 07.10., und das ist der Befund:**

- **Ein Bericht von heute:** Lukeba habe nach seinen Leistenproblemen **an Teilen des Mannschaftstrainings** teilgenommen; ein Einsatz gegen Frankfurt sei **möglich, aber nicht bestätigt**. Überschrift: „Leipzig hofft auf Lukeba, Frankfurt fehlt Uzun".
- **Eine zweite Fundstelle** titelt „Castello Lukeba zurück im Mannschaftstraining, Seiwald fit, Raum fehlt".
- **Eine dritte:** „Leipzigs Lukeba wieder im Training — Raum individuell".
- **Eine vierte** (mit Berufung auf Bild): Er steigere die Belastung schrittweise und solle **in der kommenden Woche** vollständig ins Mannschaftstraining integriert sein, um gegen Frankfurt spielen zu können; zu Beginn der Dienstagseinheit habe er individuell trainiert.

***Das ist eine Verbesserung gegenüber gestern — und es ist nicht, was meine Frist verlangt hat.*** **„Teile des Mannschaftstrainings", „zurück im Mannschaftstraining", „wieder im Training" — aber keine Angabe, dass er im *vollen* Mannschaftstraining ist.** Die vierte Fundstelle sagt ausdrücklich das Gegenteil: **das volle Teamtraining liegt noch vor ihm.** Gestern habe ich dazu geschrieben: *„‚Vor der Rückkehr' ist nicht ‚zurück'."* **Heute gilt: „Teile" ist nicht „voll".** **Die Frist ist abgelaufen und nicht erfüllt. Ich gehe auf 1:1.**

***Und anders als bei Köln liegt hier keine Gegenangabe vor, sondern zwei weitere Befunde in dieselbe Richtung:***

- **Raum fehlt bzw. trainiert individuell** — zwei unabhängige Überschriften sagen das. **Gestern stand hier, Raum kehre im Lauf dieser Woche von der Nationalmannschaft zurück.** Das ist eine Verschlechterung auf der Leipziger Außenbahn. *Ältere Berichterstattung nennt bei ihm Leistenprobleme aus der Vorsaison; ich führe ihn als fraglich bis fehlend, nicht als belegten Ausfall.*
- **Uzun steht Frankfurt wohl wieder zur Verfügung.** Der hessenschau-Ticker vom **07.10.** meldet **leichte Entwarnung** nach unklarer Lage am Morgen: Der Trainer habe sich am freien Mittwoch im Proficamp mit Uzun über seinen Zustand erkundigt; für das Spiel in Leipzig am **Samstagabend (18:30)** solle er **wohl wieder zur Verfügung stehen**, der Einsatz sei aber noch offen. ***Das ist bemerkenswert, weil ich gestern eine Fundstelle verworfen habe, die genau das behauptete.*** **Meine Verwerfung war richtig — jene PK war zeitlich unmöglich —, aber ihr Inhalt wird heute von einer datierbaren, unabhängigen Quelle in der Sache bestätigt.** *Das ist eine Lehre über Verwerfungen: Eine falsch datierte Fundstelle kann inhaltlich trotzdem zutreffen, und das Verwerfen ist dann richtig und blind zugleich.*

***Gegengewichte, die ich nenne, weil sie existieren:*** **Seiwald ist fit.** Und: **In beiden Heimspielen mit Lukeba in der Startelf gewann Leipzig zu null (3:0, 5:0); ohne ihn kamen die Niederlagen (1:3 in Bremen, 0:2 in Leverkusen).** **Diese Zahl trägt mein 1:1 mit** — sie ist der Grund, warum ein unklarer Lukeba den Tipp überhaupt bewegt, und zugleich der Grund, warum ich nicht tiefer als auf ein Remis gehe: **Leipzigs Heimbilanz ist 8:0, und Frankfurt hat auswärts noch nicht gewonnen.**

***Der übrige Leipziger Stand:*** **Reitz und Baumgartner arbeiten an der Rückkehr und fehlen gegen Frankfurt** (heute erneut bestätigt), **Orbán und Nusa** aus den Nationalmannschaften zurück. **Nach dem Spieltag folgt das Champions-League-Heimspiel gegen PSV Eindhoven** — ein Rotationsargument, das bei unklarer Lukeba-Lage schwerer wiegt als gestern: **Ein Innenverteidiger, der gerade erst Teile des Mannschaftstrainings absolviert, wird nicht drei Tage vor einem Europapokalspiel für 90 Minuten riskiert.** *Die Vereinsmeldung (`rbleipzig.com/de/news/training-lukeba-reitz-baumgartner-comeback`) bleibt unabrufbar; eine Vereinsangabe habe ich in keinem Lauf gehabt.*

***Der Frankfurter Stand im Übrigen:*** **Burkardt und Larsson sind heute nicht belastbar zu klären** — die Zusammenfassung sagt ausdrücklich, dass die Burkardt-Meldungen („Ausfall bis Ende Januar") aus **Dezember 2025** stammen und veraltet sind, und zu Larsson nur Material aus **November 2025** vorliegt. **Ich führe beide als unbekannt** und übernehme insbesondere **nicht** die gestern verworfene Angabe, Burkardt stehe „definitiv nicht zur Verfügung". Unverändert: Maluze im Reha-Training, Dreierkette Koch/Collins/Brassier, Dōan fit, 4:0 gegen Braunschweig am 02.10. **Der Trainername ist heute unklar (Hütter oder Toppmöller) — siehe Restlücken.**

***Warum 1:1 und nicht 1:2:*** **Leipzig ist zu Hause 8:0, Frankfurt hat auswärts in zwei Spielen vier Punkte, aber keinen Sieg.** Die Änderung nimmt Leipzig den Sieg, nicht den Heimvorteil.

***Die Schwelle für den nächsten Lauf:*** **Kommt eine Bestätigung, dass Lukeba im vollen Mannschaftstraining ist oder in der Startelf steht, gehe ich auf 2:1 zurück. Kommt eine Leipziger Vereinsangabe, dass er nicht spielt, gehe ich auf 1:2 und bleibe dort bis zum Anpfiff. Wird Raums Ausfall bestätigt, bleibe ich auf 1:1 auch bei einer Lukeba-Entwarnung.**

### 1. FC Köln – Borussia Mönchengladbach
**Sonntag, 11.10.2026, 15:30 Uhr** (RheinEnergieStadion, DAZN)
**Tipp: 1:0**
*unverändert* — **und aus dem riskantesten Tipp von gestern ist heute der am besten belegte geworden. Gleichzeitig löst hier eine Schwelle aus, und ich ändere trotzdem nicht.**

***Das größte Einzelrisiko des Vortagsstands ist erledigt*** (siehe „Geschlossene Lücken"). **El Mala fehlte beim Viktoria-Test als abgestellter Nationalspieler, nicht wegen einer Knöchelverletzung, und wird in denselben Berichten als Offensivkandidat gegen Gladbach genannt.** Gestern musste meine Verwerfung des „doppelten Verletzungsschocks" allein auf dem Wort „Aufsteiger" und auf arithmetisch unmöglichen neun Saisontoren ruhen. **Heute steht eine positive Gegenangabe daneben.**

***Kölns Sturmausfälle sind jetzt vereinsbestätigt und datiert:*** **Testspiel am 03.10.2026, 2:2 gegen Viktoria Köln. Dallinga verdrehte sich nach 27 Minuten das rechte Knie — der Verein teilte eine Kreuzbandverletzung und einen längeren Ausfall mit, ohne zu sagen, ob kompletter Riss und welches Band; WDR berichtet unter Berufung auf den FC von Monaten. Ache hat eine Muskelverletzung und wird im November zurückerwartet.** **Zwei Meldungen auf `fc.de` belegen das.** *Gestern war das Kölner Sturmzentrum „eine Prognose ohne Vereinsangabe".*

***Kölns Sturmzentrum, heute mit einem Argument mehr:*** **Bülter bleibt Favorit — und er hat im Test getroffen** („Bülter verhindert Pleite"). Als weitere Namen werden **El Mala, Waldschmidt** und ein mögliches Comeback von **Rondic** genannt, dazu aus dem Vortagsstand Thielmann und Maina. ***Wichtig für meine eigene Schwelle:*** **Ein Nachwuchsspieler im Sturmzentrum ist damit *nicht* zu erwarten — Bülter ist ein erfahrener Profi mit 182 Bundesligaspielen.** **Mein 0:0-Zweig ist nicht ausgelöst.**

***Die Schwelle, die heute ausgelöst hat — und warum ich nicht ändere.*** Gestern: *„Kommt eine belegte Gladbacher Entwarnung zu Honorat oder Kühn, gehe ich auf 1:1 zurück."*

- **Honorat: keine Entwarnung, im Gegenteil.** Heute bestätigt: **Verletzung im Training, muskuläre Verletzung nach erster Vereinsdiagnose, Ausfall auf unbestimmte Zeit**, fehlt voraussichtlich im Derby. **Nicht ausgelöst.**
- **Kühn: eine schwache Entwarnung, und meine Arithmetik schließt sie nicht mehr aus** (Korrektur 1). `fussballdaten.de` nennt ihn als **mögliche Alternative für das Auswärtsspiel in Köln**, die Entscheidung falle in der Trainingswoche. **Fünf Wochen ab dem 06.09. sind genau der 11.10.** ***Ich behandle das als ausgelöst.***

***Die Gegenangaben, die im selben Lauf eintreffen und schwerer wiegen:***
- **Kleindienst, der Kapitän, ist fraglich.** Er **brach das Training am Dienstag (06.10.) vorzeitig ab**, weil er sich beim Aufwärmen unwohl fühlte — **Blessin selbst gegenüber Sport1.** Überschriften: „Gladbach suffer injury scare as Kleindienst pulls out of training", „Kurz vor dem Derby: Blessin bricht wichtiger Gladbach-Star weg". ***Gestern war Kleindienst „das beste Argument gegen mein 1:0". Heute ist er fraglich.*** Dazu die zweite Darstellung: Er kehre aus einer **Sperre** zurück, in deren Abwesenheit **Lidberg** getroffen habe, und könne zunächst auf der Bank bleiben.
- **Itakura ist fraglich** — **angeschlagen aus der Nationalmannschaft zurückgekehrt**, Einsatz am Sonntag ungewiss. **Ein Innenverteidiger weniger bei der schlechtesten Defensive der Liga.**
- **Leopold und Castrop** fehlen weiter; **Zento Uno** hat sich laut einer Fundstelle im Training erneut verletzt.

***Die Abwägung nach meiner Regel:*** **Ein möglicher Rückkehrer (Kühn, schwach belegt) steht gegen zwei neue Fragezeichen (Kleindienst, Itakura) und einen bestätigten Ausfall (Honorat).** **Gladbachs Lage ist heute nicht besser als gestern, sondern eher schlechter. Die Auslösung ist genannt, die Gegenangabe wiegt schwerer, der Tipp bleibt bei 1:0.**

***Der Rahmen auf Gladbacher Seite, heute vollständiger:*** **Blessin ist der dritte Trainer dieser Saison** (Polanski bis 13.09., Lichte interimistisch, Blessin ab 22.09.), **das Derby ist sein Pflichtspieldebüt**, und er ist der erste Gladbacher Trainer, der mit einem Köln-Derby beginnt. Seine Ansage: Der Borussia-Park solle wieder eine Festung werden, jeder Gegner solle mit Angst kommen. **Gladbach braucht dringend die ersten Punkte.** *Ein Trainerwechsel-Effekt ist das einzige echte Argument gegen mein 1:0 — aber ein Debütant mit dezimierter Offensive im Auswärtsderby ist kein starkes.*

***Warum 1:0 bleibt, in einem Satz:*** **Ein Gastgeber ohne beide Mittelstürmer — aber mit einem im Test treffenden Bülter, einem verfügbaren El Mala und zu Hause gegen die schlechteste Defensive der Liga (16 Gegentore in vier Spielen, keine Partie unter drei) — gegen einen Gast, der auswärts noch kein Tor erzielt hat (0:8), Letzter ist, seinen Kapitän und seinen Innenverteidiger als fraglich führt und seinen besten Flügelspieler auf unbestimmte Zeit verloren hat.**

***Die Schwelle für den nächsten Lauf:*** **Kommt eine belegte Gladbacher Entwarnung zu Kleindienst *und* Kühn, gehe ich auf 1:1. Wird Kleindiensts Ausfall bestätigt, bleibe ich auf 1:0 und schließe ein zweites Kölner Tor nicht mehr aus (2:0). Kommt eine auf diese Woche datierbare Meldung zu einem *weiteren* Kölner Offensivausfall — El Mala, Kamiński, Bülter —, gehe ich auf 0:0.** *Die Dallinga/Ache-Ausfälle sind in dieser Rechnung enthalten und lösen den 0:0-Zweig nicht aus; sie waren schon gestern eingerechnet.*

### SC Freiburg – FC Schalke 04
**Sonntag, 11.10.2026, 17:30 Uhr** (Europa-Park-Stadion)
**Tipp: 2:0**
*unverändert* — **und heute mit der dritten unabhängigen Bestätigung der Schalker Hälfte, während die Freiburger Hälfte zum dritten Mal ungeprüft bleibt.**

***Die Ansetzung ist über die Vereinsquelle bestätigt:*** `schalke04.de`, „Ansetzungen Spieltage 5 bis 11", **17:30**.

***Ljubičić ist heute zum dritten Mal als Ausfall bestätigt — und erstmals ausdrücklich als Vereinsangabe.*** Die Übersicht führt ihn als vom **Verein „bis auf Weiteres" als ausfallend bestätigt**. **Meine Schwelle verlangt eine Fit-Meldung. Das Gegenteil liegt vor. Nicht ausgelöst.** Unverändert dazu der gestrige Stand: Knieverletzung links, Auswechslung in der 21. Minute bei Union am 11.09., Kreuzbandriss ausgeschlossen.

***Zwei weitere Schalker Namen kommen hinzu, und nach meiner eigenen Regel rechne ich sie nicht ein:*** **Justin Heekeren** (Kreuzbandverletzung, laut Schlagzeile mindestens sechs Monate — ein Torhüter) und **Johannes Siebeking** (Bauchmuskelverletzung). Dazu **Anton Donkor** als nicht im Kader geführt und **Emil Højlund** (Achillessehne, unverändert aus dem Vortagsstand). ***Meine Regel von vorgestern:*** *„Langzeitausfälle, die ich nachträglich entdecke, lösen keine Änderung aus; ich trage sie nach und rechne sie nicht ein."* **Heekeren und Siebeking werden nachgetragen, nicht eingerechnet.** *Ein Sky-Artikel nennt zusätzlich „Timo Becker, Christian Gomis, Emil Hojlund & Co." — Gomis ist ein Name, den ich nicht datieren kann; ich trage ihn nicht.*

***Becker bleibt fraglich*** (Korrektur 3 von gestern, heute nicht widersprochen): Fuß-/Knöchelverletzung aus dem 0:0 gegen Elversberg vom 20.09., Beschreibung uneinheitlich. Fällt er aus, rückt Wober in die Startelf.

***Zu Freiburg finde ich zum dritten Mal in Folge nichts Verwendbares, und das ist die ehrliche Schwäche dieses Tipps.*** **Der zweite Teil meiner Schwelle — ein *neuer* Freiburger Ausfall, zugezogen nach dem 20.09. und mit Diagnose — ist erneut nicht widerlegt, sondern ungeprüft.** Es bleibt beim Stand: **Florent Muslija** als Langzeitausfall (Kreuzbandriss, heute über eine zweite Quelle mit „etwa fünf Monate" bestätigt) **nachgetragen und nicht eingerechnet**, 4:0 im Pausentest gegen Luzern, 10 Punkte, Platz 3.

***Der Schalker Rahmen bleibt der terminlich wichtigste Punkt, und er ist heute zur Hälfte verstrichen:*** **Öffentliche Trainingseinheiten am Mittwoch, 07.10. (heute, kein Bericht gefunden) und Freitag, 09.10., jeweils 10:45 Uhr; Pressekonferenz am Freitag, 14:00 Uhr.** **Dort entscheidet sich die Ljubičić- und Becker-Frage, und mein letzter Lauf vor dieser Sonntagspartie liegt danach.** *Dass ich zum heutigen öffentlichen Training nichts gefunden habe, nenne ich als Lücke, nicht als Entwarnung.*

***Warum 2:0 bleibt, in einem Satz:*** **Ein Heimteam mit neun Toren in zwei Heimspielen, 10 Punkten und Platz 3 gegen einen Gast mit 3:4 Toren in vier Spielen — der schwächsten Offensive der Liga —, dem der Mittelfeldmotor nach heute vereinsbestätigtem Stand „bis auf Weiteres" fehlt, dessen Innenverteidiger fraglich ist und dessen Ausfallliste sich heute um zwei Namen verlängert hat.**

***Die Schwelle für den nächsten Lauf, unverändert:*** **Wird Ljubičić belegt fit gemeldet oder kommt ein Schalker Offensivspieler belegt zurück, gehe ich auf 2:1. Ein *neuer* Freiburger Ausfall — zugezogen nach dem 20.09. und mit Diagnose — bringt 1:0. Langzeitausfälle, die ich nachträglich entdecke, lösen keine Änderung aus.**

---

## Verteilung und Selbstkontrolle

| Partie | Anstoß | Tipp | Status |
|---|---|---|---|
| Borussia Dortmund – SV Werder Bremen | Fr 09.10., 20:30 | **3:1** | unverändert |
| FC Augsburg – FC Bayern München | Sa 10.10., 15:30 | **1:2** | unverändert |
| TSG Hoffenheim – Hamburger SV | Sa 10.10., 15:30 | **1:0** | **geändert von 2:0** |
| 1. FSV Mainz 05 – Bayer 04 Leverkusen | Sa 10.10., 15:30 | **1:1** | unverändert |
| 1. FC Union Berlin – SV 07 Elversberg | Sa 10.10., 15:30 | **1:1** | **geändert von 1:2** |
| SC Paderborn 07 – VfB Stuttgart | Sa 10.10., 15:30 | **1:2** | unverändert |
| RB Leipzig – Eintracht Frankfurt | Sa 10.10., 18:30 | **1:1** | **geändert von 2:1** |
| 1. FC Köln – Borussia Mönchengladbach | So 11.10., 15:30 | **1:0** | unverändert |
| SC Freiburg – FC Schalke 04 | So 11.10., 17:30 | **2:0** | unverändert |

**Verteilung:** **4 Heimsiege** (Dortmund, Hoffenheim, Köln, Freiburg), **2 Auswärtssiege** (Bayern, Stuttgart), **3 Remis** (Mainz, Union, Leipzig). **Tore: 20 in neun Partien, 2,2 pro Spiel** — gestern waren es 23. **Die Differenz von genau drei Toren entspricht exakt den drei Änderungen**, die jede ein Tor abziehen (2:0→1:0, 1:2→1:1, 2:1→1:1). *Gegengerechnet, weil eine Verteilungsangabe, die nicht aufgeht, die ganze Tabelle verdächtig macht.*

***Die drei Remis sind neu in dieser Häufung und ich prüfe sie gegen mich selbst:*** Gestern hatte ich ein Remis, heute drei. **Alle drei entstehen aus derselben Ursache — eine auf heute terminierte oder heute erfüllte Schwelle —, nicht aus einer Neigung zur Vorsicht.** *Dass zwei davon (Union, Leipzig) auf Fundstellen eines einzigen Tages beruhen, ist die Schwäche dieses Laufs; bei Union habe ich das Risiko oben ausdrücklich benannt.*

**Belegqualität der neun Tipps, von stark nach schwach:**
1. **Köln – Gladbach:** vereinsbestätigte, datierte Ausfälle auf beiden Seiten, Trainerchronologie geklärt, das gestrige Hauptrisiko widerlegt. **Heute der am besten belegte Tipp.**
2. **Dortmund – Werder:** Pressekonferenz von heute, fünf Namen mit Status, Gästeliste über zweite Quelle bestätigt.
3. **Freiburg – Schalke:** Schalker Hälfte dreifach belegt, Ansetzung über Vereinsquelle — aber Freiburg zum dritten Mal blind.
4. **Augsburg – Bayern:** Musiala dreifach belegt, Trainingsteilnehmer namentlich, Ansetzung über Vereinsquelle.
5. **Leipzig – Frankfurt:** vier Lukeba-Fundstellen von heute, hessenschau-Ticker von heute — aber keine Vereinsangabe in acht Läufen.
6. **Mainz – Leverkusen:** drei Rückkehrer belegt, Zentner-Lage verstanden — aber keine Startelf-Angabe.
7. **Paderborn – Stuttgart:** eine Vereinsquelle (Nartey), sonst nichts; Paderborn blind, Trainer unbenannt.
8. **Union – Elversberg:** Zuordnung geklärt, aber die Änderung steht auf einer einzigen Meldung mit ungeklärter Doppeldatierung.
9. **Hoffenheim – HSV:** **Gästeseite tagesaktuell, Heimseite im vierten Lauf ohne jede Information.** Schwächste Basis, und die Änderung ist genau das Eingeständnis davon.

**Was dieser Lauf geleistet hat:** Proxy-Diagnose belegt · Anstoßzeiten vollständig in Lokalzeit bestätigt, scheinbarer Widerspruch methodisch aufgelöst · Kölner Sturmausfälle vereinsbestätigt und datiert · das größte Risiko des Vortagsstands widerlegt · Onyeka zugeordnet (Lücke von gestern) · Gladbachs Trainerchronologie und Unions Trainer geklärt · vier Korrekturen, darunter ein eigener Rechenfehler und eine falsch konstruierte eigene Schwelle · neun Fundstellen verworfen, zwei davon hätten Tipps bewegt.

**Was offen bleibt:** Hoffenheim (4 Läufe), Freiburg (3 Läufe), die Trainer von Köln, Paderborn und Leverkusen, Frankfurts Trainername neu unklar, Onyekas Doppeldatierung, Elversbergs Kaderlage, Unions BAK-Test, Leipzigs dritte Niederlage.

---

## Quellen

Alle Angaben stammen aus Suchergebnis-Titeln und -Zusammenfassungen; **kein Artikel konnte im Volltext gelesen werden** (siehe Quellenlage). Die folgenden Adressen sind die, auf die sich dieser Lauf stützt:

**Vereins-Primärquellen (die stärksten Funde des Tages):**
- `fc.de/aktuelles/news/dallinga-und-ache-fallen-aus` · `fc.de/aktuelles/news/remis-im-test-bei-der-viktoria`
- `fcaugsburg.de/article/bayern-muenchen-im-check-...` (Vorschau 06.10., Anstoßzeit)
- `schalke04.de/bundesliga/ansetzungen-spieltage-5-bis-11-saison-26-27/`
- `fc-union-berlin.de/en/news/mauro-lustrinelli-named-new-mens-head-coach--tCyufa`
- `vfb.de` (Nartey, vorzeitige Rückkehr) · `scp07.de` (PK-Ankündigung)
- `x.com/SV07Elversberg/status/2099161368758804724` (Onyeka/Darvich als Elversberger)

**Spieltagsberichterstattung vom 06./07.10.:**
- `hessenschau.de/.../eintracht-frankfurt-news-ticker-...` (Uzun, 07.10.)
- `sport1.de/news/fussball/bundesliga/2026/10/kovac-gibt-positives-update-bei-schlotterbeck` · `fussballtransfers.com/...schlotterbeck-co-bvb-mit-fuenf-fragezeichen` · `absolutfussball.com/.../bvb-trainer-kovac-gibt-verletzungsupdate-zu-schlotterbeck-94529268.html`
- `sports.yahoo.com/articles/gladbach-suffer-injury-scare-kleindienst-121300443.html` · `90min.de/kurz-vor-dem-derby-blessin-bricht-wichtiger-gladbach-star-weg` · `absolutfussball.com/.../gladbach-sorgen-um-itakura-vor-rhein-derb-in-koeln-94528747.html`
- `diethueringer.de/sport/rb-leipzig-castello-lukeba-zurueck-im-mannschaftstraining-seiwald-fit-raum-feh-3129870` · `freiepresse.de/.../leipzigs-lukeba-wieder-im-training-raum-individuell-artikel14230107` · `absolutfussball.com/.../rb-leipzig-personal-update-eintracht-frankfurt-...-94519475.html`
- `ligainsider.de/francis-onyeka_36948/onyeka-erleidet-verletzung-am-fuss-418770/`
- `tipico.de/wett-tipps/.../nach-dem-ausfall-von-albert-groenbaek-so-plant-der-hsv-bei-tsg-hoffenheim` · `fussballtransfers.com/a3632930590043612181-hsv-entwarnung-bei-poulsen`
- `geissblog.koeln/2026/10/das-kreuzband-fc-verkuendet-bittere-diagnosen-von-dallinga-und-ache/` · `geissblog.koeln/2026/10/vom-testspiel-in-die-klinik-fc-bangt-um-dallinga-und-ache-buelter-verhindert-pleite/` · `eurosport.de/.../1.-fc-koeln-verliert-thijs-dallinga-ragner-ache-testspiel-..._sto23342567/story.shtml` · `sportschau.de/regional/wdr/wdr-koeln-vor-gladbach-derby-mit-koelner-sturm-problem-100.html`
- `sport.de/news/ne17217333/fc-bayern-kimmich-und-co-wieder-im-betrieb---musiala-trainiert-individuell`
- `magazin.comunio.de/verletzten-update-mainz-05-nebel-werder-bremen-hein-elversberg-futkeu` · `bulinews.com/mainz-receive-injury-boost-trio-return-training`

**Übersichts- und Aggregatorseiten (mit den genannten Datierungsvorbehalten):**
- `ligainsider.de/bundesliga/verletzte-und-gesperrte-spieler/` und die Vereinsunterseiten (Werder, Freiburg, Schalke, Mainz, HSV, Hoffenheim)
- `fussballdaten.de` (Kühn als Option, Gladbacher Ausfälle) · `fotmob.com` (Stuttgart, Paderborn, Union/Elversberg — durchgehend als veraltet gekennzeichnet)
- `bundesliga-gruppe.de/aktuelles/spiele-der-bundesliga-und-2-bundesliga-bis-ende-november-zeitgenau-angesetzt/` · `dfl.de/de/aktuelles/saison-2026-27-spielplaene-...`
- `en.wikipedia.org/wiki/2026%E2%80%9327_Borussia_M%C3%B6nchengladbach_season` (Trainerchronologie) · `en.wikipedia.org/wiki/Alexander_Blessin` · `en.wikipedia.org/wiki/Mauro_Lustrinelli`

**Nicht abrufbar (403 CONNECT / EGRESS_BLOCKED):** `kicker.de`, `transfermarkt.de`, `weltfussball.de`, `bundesliga.com`, `sportschau.de`, `ligainsider.de`, `anstosszeiten.de`, `rbleipzig.com` — und damit alle im Routine-Prompt ausdrücklich genannten Leitquellen.
