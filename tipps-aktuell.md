# Bundesliga-Tipps – 5. Spieltag 2026/27 (Stand: 06.10.2026)

**Ansetzung:** Freitag, 09.10. bis Sonntag, 11.10.2026. Der Vortagsstand (05.10.) betraf denselben Spieltag – **alle neun Tipps sind vergleichbar.**

**Dienstag der Spielwoche, drei Tage vor dem Anpfiff in Dortmund.** Das Länderspielfenster ist seit gestern geschlossen, die Nationalspieler kehren in dieser Woche zurück, **und der FC Bayern nimmt heute das Mannschaftstraining auf** – gestern stand hier noch, dass das „morgen" geschieht.

**Heute ändert sich kein Tipp.** **Keine der acht offenen Schwellen ist ausgelöst.** *Das ist heute aber ein anderes Ergebnis als gestern, und der Unterschied ist der eigentliche Inhalt dieses Laufs:* **Zwei Fundstellen hätten heute Tipps bewegt, und beide sind an der Datierung gescheitert** – ein doppelter Kölner Verletzungsschock vor dem Derby und eine Frankfurter Spieltags-Pressekonferenz. **Hätte ich sie übernommen, stünden unten zwei andere Ergebnisse.**

**Dafür ist heute der Belegstand auf der Gästeseite in Hoffenheim so gut wie nie** (Grønbæks Rückkehrtermin ist jetzt genannt und liegt *nach* dem 10.10.), **und zwei Lücken, die ich mehrere Läufe lang offen geführt habe, sind geschlossen: Zimmerschied und Zentner.**

**Vier Korrekturen am Vortagsstand sind nötig** – bei Musiala, bei Coufal, bei Becker und in der Einordnung der Agu-Fundstellen. **Die Coufal-Korrektur ist die unangenehmste, weil sie eine Angabe entwertet, die ich drei Läufe lang geführt habe.**

## Hinweis zur Quellenlage (bitte zuerst lesen)

**Die Primärseiten sind aus dieser Umgebung weiterhin nicht abrufbar.** Heute einzeln geprüft:

- **Direkte Verbindungsprüfung** auf acht Sportdomains (`kicker.de`, `www.kicker.de`, `transfermarkt.de`, `weltfussball.de`, `bundesliga.com`, `sportschau.de`, `ligainsider.de`, `rbleipzig.com`) → **alle acht mit HTTP-Status `000`**, also kein Verbindungsaufbau.
- **WebFetch auf drei voneinander unabhängigen Domains** – `www.ligainsider.de` (die neueste Lukeba-Meldung), `www.90min.de` (die Gladbacher Ausfallmeldung) und `en.wikipedia.org` (zur Datierung eines Kölner Spielers) → **alle drei mit `EGRESS_BLOCKED` und namentlicher Nennung der Domain.**

***Das ist heute der bessere Befund als gestern, und ich sage auch, warum:*** **Gestern lag genau ein Fetch-Versuch vor, auf einer Sportdomain. Heute sind es drei auf drei inhaltlich völlig verschiedenen Domains – darunter mit Wikipedia eine, die keine Sportseite ist – und alle drei scheitern identisch und mit derselben Fehlerkennung.** **Damit ist belegt, dass die Sperre nicht site-spezifisch ist, sondern flächig greift.**

**Was weiterhin fehlt, nenne ich trotzdem:** **Die formale Gegenprobe auf den Agent-Proxy konnte ich auch heute nicht durchführen – der Statusaufruf wurde erneut vom Berechtigungs-Klassifikator dieser Umgebung abgelehnt**, heute mit der Begründung „Credential Exploration" (gestern „Exfil Scouting"). **Ich habe den Aufruf nicht auf anderem Weg wiederholt.** **Folge: TLS- und Proxyfehler sind formal weiterhin nicht ausgeschlossen; die Breite des heutigen Befunds macht die Netzwerk-Policy aber zur mit Abstand wahrscheinlichsten Ursache.** **Das ist eine Verbesserung der Beweislage, keine Schließung der Lücke.**

**Alles unten steht deshalb auf Suchergebnis-Zusammenfassungen und -Titeln, nicht auf gelesenen Artikeln.** Wo eine Adresse ein Datum oder eine Spielzeit trägt, nenne ich es mit, weil die Datierung in diesem Repo die Hauptarbeit ist. **Vereinsmeldungen kann ich weiterhin nicht im Volltext prüfen.**

*Zum Hilfsmittel der aufsteigenden `ligainsider.de`-Meldungsnummern, das ich gestern eingeführt habe:* **Es hat heute erneut getragen** – die neueste Lukeba-Meldung (418597) liegt über den gestrigen (418481, 418564), die Daka-Meldung (418573) liegt im selben Bereich, und die verworfenen Agu- und Coufal-Meldungen (409299, 411427, 412344) liegen deutlich darunter. **Die Annahme bleibt plausibel und unbelegt, und sie ist heute nirgends mein einziges Datierungsargument.**

## Korrekturen am Vortagsstand

### 1. Coufal (Hoffenheim): die „angeschlagen"-Angabe hat keinen tragfähigen Beleg mehr

**Seit drei Läufen steht in meinen Hoffenheimer Notizen, Kramarić und Coufal seien „angeschlagen".** **Heute habe ich erstmals die mutmaßliche Quelle dieser Angabe in der Hand – und sie passt nicht in diese Saison.**

**Die Fundstelle (`ligainsider.de`, Meldungsnummer 411427, Überschrift „Coufal musste angeschlagen vom Feld") beschreibt eine Auswechslung in der 61. Minute mit Adduktorenproblemen, „seine früheste Auswechslung der Saison" – in einem Spiel gegen Mainz.**

***Hoffenheim hat in dieser Saison nicht gegen Mainz gespielt.*** **Die vier Hoffenheimer Partien des 1. bis 4. Spieltags sind: 2:3 in Köln, 2:3 gegen Dortmund, 2:1 gegen Stuttgart, 1:3 in Paderborn.** **Kein Mainz.** **Dazu passt die niedrige Meldungsnummer.**

**Ich kann nicht rekonstruieren, worauf frühere Läufe sich gestützt haben, und behaupte deshalb nicht, es sei genau diese Fundstelle gewesen.** **Was ich sagen kann:** **Heute finde ich zu Coufal keine Angabe, die sich auf diese Saison datieren lässt – und die einzige, die ich finde, gehört in eine andere.** **Ich führe Coufal ab heute als *unbekannt*, nicht als angeschlagen.** **Für Kramarić gilt dasselbe aus einem schwächeren Grund: zu ihm finde ich seit drei Läufen gar nichts Partiebezogenes.**

**Für den Tipp ändert das nichts** – beide standen nie als Ausfall in meiner Rechnung –, **aber es nimmt dem Hoffenheim-Tipp ein Argument, von dem ich dachte, ich hätte es.**

### 2. Musiala (Bayern): meine gestrige Diagnose ist heute bestritten, nicht bestätigt

**Gestern habe ich geschrieben, Musiala habe sich „den Muskelfaserriss im rechten Oberschenkel am 25.09. beim Aufwärmen vor dem Nations-League-Spiel gegen die Niederlande zugezogen", und das ausdrücklich als „jetzt partiebezogen belegt" bezeichnet.**

**Heute liegt eine zweite Darstellung vor, die mit der ersten nicht vereinbar ist:** **Musiala habe eine Hüftprellung bzw. eine Schwellung im Hüftgelenk; Bundestrainer Julian Nagelsmann habe ihn *vorsorglich* gar nicht erst für die Nations-League-Spiele gegen Bosnien-Herzegowina und die Niederlande nominiert; die medizinische Abteilung arbeite nach der Länderspielpause daran, die Schwellung vollständig abzubauen, mit dem Ziel einer baldigen Rückkehr ins Gruppentraining.**

***Die beiden Versionen widersprechen sich im Mechanismus:*** **Wer vorsorglich nicht nominiert wird, verletzt sich nicht beim Aufwärmen vor demselben Spiel.** **Beide beziehen sich aber auf dasselbe Länderspielfenster, und beide beschreiben ihn als derzeit nicht einsatzfähig.**

**Ich korrigiere deshalb nicht den Befund, sondern meine Sicherheit:** **Dass Musiala am 10.10. fehlt, halte ich weiter für gut belegt – er arbeitet in der günstigeren der beiden Versionen gerade erst auf das Gruppentraining hin.** **Die Diagnose dagegen führe ich ab heute als strittig.** **Mein gestriges „partiebezogen belegt" war zu stark.**

### 3. Becker (Schalke): die Verletzungsbeschreibung weicht ab

**Gestern stand hier „Fleischwunde am Knöchel, zugezogen gegen Elversberg".** **Heute beschreibt eine zweite Fundstelle denselben Vorgang anders:** **Becker sei im 0:0 gegen Elversberg am 20.09. nach gut einer Stunde ausgewechselt worden, nachdem er einen Schlag auf den rechten Fuß bekommen hatte, der ihn sichtlich behinderte.**

**Spiel, Datum und Spielminute stimmen überein, die Verletzungsart nicht.** **Ich führe ihn ab heute als „Fuß-/Knöchelverletzung aus dem Elversberg-Spiel vom 20.09., Beschreibung uneinheitlich".** **Am Befund – fraglich für Freiburg – ändert das nichts.**

### 4. Agu (Werder): die heutigen Fundstellen sind älter als der gestrige Stand

**Gestern habe ich Agu korrekt als Ausfall mit Wadenverletzung geführt.** **Heute liefert die Suche zu ihm drei Fundstellen, die alle *älter* sind und ein *anderes* Beschwerdebild tragen:** **eine Adduktorenverletzung, die ihn ein fünftägiges Trainingslager verpassen ließ („Es steht außer Frage, dass Felix mittrainiert. Deshalb fährt er nicht mit", Thioune), sowie zwei `ligainsider`-Meldungen mit den Nummern 409299 („Neuer Rückschlag: Agu fällt bis auf Weiteres aus") und 412344 („Agu steht noch auf 0: Kein Einsatz gegen Stuttgart").**

***Beide Nummern liegen weit unter dem heutigen Bereich, und entscheidend ist der Gegner:*** **Werder hat in dieser Saison nicht gegen Stuttgart gespielt** (Werder-Partien 1. bis 4. Spieltag: 1:4 in Freiburg, 3:1 gegen Leipzig, 1:1 in Köln, 3:2 gegen Augsburg). **Ein Trainingslager fällt zudem in die Sommervorbereitung, nicht in die Oktober-Länderspielpause.**

**Ich schreibe das nicht als Korrektur meines Tipps, sondern als Korrektur einer Verwechslungsgefahr:** **Agu hat eine längere Verletzungsgeschichte, und die Suchmaschine mischt die Episoden.** **Gültig bleibt der gestrige Stand – Wadenverletzung, heute wie gestern unter den Fehlenden.**

## Geschlossene Lücken

### Zimmerschied: er ist Elversberger, und die Rückenverletzung ist zwei Jahre alt

**Seit sechs Läufen steht in meinen Notizen zu Union – Elversberg der Satz „Tom Zimmerschied bleibt auf keiner Seite belegt".** **Das ist ab heute erledigt.**

**Belegt ist: Zimmerschied ist Linksaußen des SV Elversberg, gewechselt am 21. August 2024 mit Dreijahresvertrag.** **Er ist also Elversberger, nicht Unioner.**

**Und damit zu der Fundstelle, die mich heute beinahe zu einer Tippänderung gebracht hätte.** **Eine Aufstellungsseite zur Partie am 10.10. führt unter *Union Berlin* die Ausfälle „Zimmerschied (Rückenverletzung, out), Seifert (Knöchelverletzung, out)" sowie „Onyeka fraglich".** **Beide genannten Spieler sind in Wahrheit Elversberger** – **Luis Seifert ist mein seit Läufen geführter Elversberger Langzeitausfall.** **Das ist exakt dieselbe Seitenvertauschung, die ich gestern bei dieser Partie schon einmal verworfen habe**, als dieselbe Art Quelle Nsoki, Burke, Friedrich und Markgraf der Elversberger Seite zuschlug.

***Hätte ich die Seitenangabe für bare Münze genommen und nur korrigiert, stünde hier jetzt ein zweiter Elversberger Ausfall mit Diagnose – und meine Schwelle wäre ausgelöst.*** **Sie ist es nicht, und zwar aus einem zweiten, unabhängigen Grund:** **Zimmerschieds Rückenverletzung ist in seiner Verletzungshistorie auf den 2. bis 18. Oktober 2024 datiert.** **Das ist zwei Jahre her.** **Die Aufstellungsseite zieht einen abgelaufenen Historieneintrag als aktuellen Ausfall ein.** **Nicht ausgelöst, und ich bin froh, dass ich nachgesehen habe.**

### Zentner: die Vereinsangabe existiert, und sie erklärt den Widerspruch der letzten vier Läufe

**Seit vier Läufen führe ich Zentner als Lücke: Verein nennt „mehrere Wochen", Aggregatoren hoffen auf Rückkehr, nichts davon ist partiebezogen.** **Heute liegt erstmals eine Darstellung vor, die beides zusammenbringt – und sie zeigt, dass es *zwei* Vorgänge waren.**

- **Vorgang 1:** **Zentner verpasste das 5:0 beim HSV wegen muskulärer Probleme im Oberschenkel**, Schwolow spielte und hielt zu null. **Das 0:5 des HSV gegen Mainz ist der 2. Spieltag (04.–06.09.) – damit ist dieser Vorgang auf diese Saison datiert.**
- **Vorgang 2:** **Mainz bestätigte anschließend, dass Zentner sich im 1:3 gegen Eintracht Frankfurt eine Handverletzung zugezogen hat**; der 31-Jährige falle „für die kommenden Wochen" aus, die Rückkehr hänge vom individuellen Heilungsverlauf ab; Schwolow vertrete bis auf Weiteres. **Mainz 1:3 Frankfurt ist der 3. Spieltag (11.–13.09.) – ebenfalls diese Saison.**

***Damit löst sich auf, woran ich mich vier Läufe lang gerieben habe:*** **Die „mehreren Wochen" des Vereins gehörten zur Handverletzung aus dem Frankfurt-Spiel, nicht zu den Oberschenkelproblemen vor dem HSV-Spiel.** **Zwei Verletzungen in zwei Wochen, dieselbe Vertretung – deshalb liefen die Meldungen so durcheinander.**

***Für meine Schwelle ändert das nichts, und das sage ich ausdrücklich:*** **Diese Vereinsbestätigung ist die Erstmeldung der Verletzung aus Mitte September. Sie sagt nichts über den 10.10.** **„Für die kommenden Wochen" aus dem Zeitraum um den 13.09. lässt den 10.10. offen.** **Meine Schwelle verlangt eine Mainzer Angabe dazu, *ob er spielt*. Die liegt nicht vor.** **Nicht ausgelöst.**

*Eine Warnung zum selben Fundstellenbündel:* **Eine der Zusammenfassungen schreibt die Zentner-Einschätzung „Trainer Urs Fischer" zu.** **Mainz' Trainer ist Bo Henriksen.** **Ich habe aus dieser Fundstelle deshalb nur übernommen, was eine zweite trägt.**

### Eine Lücke, die ich heute neu an mir selbst entdecke: Saïd El Mala

**Bei der Datierungsprüfung unten ist mir aufgefallen, dass ein Kölner Spieler in sechs Läufen nie in meinen Notizen vorkam, obwohl er dort hingehört.**

**Belegt ist: Saïd El Mala hat im August 2026 seinen Vertrag beim 1. FC Köln langfristig bis 2031 verlängert, trägt die Nummer 10, und Borussia Dortmund ist im Sommer 2026 mit drei Anläufen an einer Verpflichtung gescheitert.** **Er ist also ein aktueller Kölner Spieler, und zwar ein zentraler.**

**In meinen Kölner Notizen – fünf Läufe lang über Dallinga, Ache, Bülter, Thielmann, Waldschmidt und Maina – taucht er nicht auf.** **Das ist keine neue Information über das Spiel, sondern eine Lücke meiner eigenen Liste, und ich schreibe sie als solche hin, so wie gestern bei Castrop und Leopold.** **Eine Tippänderung ziehe ich daraus ausdrücklich nicht** – ich weiß über seinen aktuellen Zustand nichts, und das Nichtwissen ist nicht zu meinen Gunsten auszulegen.

## Heute ausdrücklich verworfene Fundstellen

**1. Der doppelte Kölner Verletzungsschock vor dem Derby – die folgenreichste Verwerfung des Tages.**
**Eine Fundstelle meldet unter der Überschrift „1. FC Köln: Doppelter Verletzungsschock vor Derby gegen Gladbach":** **Saïd El Mala brach die erste Trainingseinheit der Derbywoche ab, griff sich nach einer Übungsform mit schmerzverzerrtem Gesicht an den linken Knöchel und verließ den Platz humpelnd, begleitet von Athletiktrainer Tillmann Bockhorst; Jakub Kamiński trainierte am Mittwoch nach einem Schlag auf den Fuß am Dienstag nur individuell, sein Einsatz gegen Gladbach sei „völlig offen".**

***Wäre das aktuell, wäre es der Auslöser des Tages:*** **Köln fehlen in meinem Tipp ohnehin beide Mittelstürmer, und wenn zusätzlich die beiden gefährlichsten Offensivspieler ausfielen, wäre mein 1:0 zu hoch.**

***Es ist nicht aktuell, und das ergibt sich aus der Fundstelle selbst:*** **Sie nennt beide „die gefährlichsten Torschützen des Aufsteigers, mit neun Toren (El Mala) und sechs Toren (Kaminski)".**
- **„Aufsteiger" trifft auf Köln in der Saison 2025/26 zu, nicht in dieser – Köln spielt sein zweites Bundesligajahr.**
- **Neun Saisontore sind nach vier Spieltagen unmöglich: Köln hat in dieser Saison insgesamt sechs Tore erzielt.** **Es sind Zahlen einer vollen Spielzeit.**
- **Dazu passt eine mitgefundene Adresse `bundesliga.com/de/bundesliga/spieltag/2025-2026/27/1-fc-koeln-vs-borussia-moenchengladbach` – das Kölner Heimderby am 27. Spieltag der Vorsaison.**

**Verworfen.** ***Und die ehrliche Einschränkung dazu, weil sie meinen Tipp betrifft:*** **Mein Altersargument (El Mala als „19-Jähriger") trägt hier nicht – er wird auch in Meldungen vom August 2026 so bezeichnet.** **Die Verwerfung ruht auf „Aufsteiger" und auf den neun Toren, nicht auf dem Alter.** **Sollte sich diese Fundstelle wider Erwarten doch auf diese Woche beziehen, ist mein 1:0 zu hoch – das ist das größte Einzelrisiko in den neun Tipps unten.**

**2. Die Frankfurter Spieltags-Pressekonferenz, die zeitlich nicht stattgefunden haben kann.**
**Eine Fundstelle gibt wieder:** **„Hugo Larsson und Can Uzun könnten für das Auswärtsspiel in Leipzig (Samstag, 18:30) in den Kader zurückkehren. Beide hätten am Donnerstag nach längerer Pause wieder mit der Mannschaft trainiert, sagte Trainer Dino Toppmöller auf der Spieltags-Pressekonferenz; das Abschlusstraining am Freitag müsse aber abgewartet werden. Stürmer Jonathan Burkardt stehe definitiv nicht zur Verfügung."**

***„Auswärtsspiel in Leipzig, Samstag, 18:30" ist wörtlich meine Partie.*** **Und genau deshalb habe ich nachgerechnet.**

**Heute ist Dienstag, der 06.10.2026.** **Der Donnerstag dieser Woche ist der 08.10., der Freitag der 09.10. – beide liegen in der Zukunft.** **Eine Pressekonferenz, die ein Donnerstagstraining im Rückblick schildert und ein Freitags-Abschlusstraining ankündigt, kann nicht vor heute über den 10.10.2026 gehalten worden sein.** **Es muss ein früheres Frankfurter Auswärtsspiel in Leipzig sein.** **Verworfen – samt der Larsson- und Uzun-Rückkehr und samt der Burkardt-Angabe.**

*Dass Frankfurt auch in Leipzig antritt, wenn die Ansetzung stimmt, macht diese Verwechslung besonders leicht – wie gestern bei Mainz – Leverkusen. Deshalb nenne ich sie ausführlich.*

**3. Musiala, Muskelbündelriss, acht Wochen – aus einem Spiel, das noch nicht stattgefunden hat.**
**Eine Fundstelle schildert: Musiala wurde in der 54. Minute verletzt ausgewechselt und erlitt „einen Muskelbündelriss im hinteren linken Oberschenkel" beim 3:1-Sieg des FC Bayern in Augsburg an einem Freitagabend; laut Sky rund acht Wochen Ausfall.**
***Augsburg – Bayern ist meine Partie am 10.10.2026 und noch nicht angepfiffen.*** **Es kann kein 3:1 geben, und es kann keinen Freitagabend geben – die Partie ist für Samstag, 15:30 Uhr angesetzt.** **Vorsaison, verworfen.** **Weder das Ergebnis noch die Achtwochenangabe übernehme ich.**

**4. Die HSV-Ausfallliste aus dem April 2026 – zweite Bestätigung einer gestrigen Verwerfung.**
**Eine Fundstelle meldet: „Luka Vuskovic fehlt dem HSV im Heimspiel gegen die TSG Hoffenheim am Samstag, wie Trainer Merlin Polzin auf der Pressekonferenz mitteilte; dazu fehlen die verletzten Miro Muheim und Yussuf Poulsen sowie der gesperrte Philip Otele."**
**Ihre Adresse lautet `sport1.de/news/fussball/bundesliga/2026/04/vuskovic-fehlt-hsv-auch-gegen-hoffenheim` – April 2026 – und sie beschreibt ein *Heimspiel des HSV*; meine Partie ist das Heimspiel der TSG.** **Das ist derselbe Vorgang, den ich gestern über die Adresse `.../matchday/2025-2026/31/` verworfen habe, heute über eine zweite Quelle bestätigt.** **Verworfen.** ***Wichtig für meinen Tipp:*** **Die dort genannte Poulsen-Verletzung gehört in den April und widerspricht seiner Entwarnung von vorgestern nicht.**

**5. Hugo Bolin als Gladbacher Derby-Ausfall.**
**Eine Fundstelle schreibt, Gladbach müsse sich ohne Stürmer Hugo Bolin auf das Derby vorbereiten, er sei für Schweden nominiert worden.** **Eine Nominierung für ein Länderspielfenster, das gestern geendet hat, ist kein Ausfall für den 11.10.** **Entweder beschreibt der Satz die Trainingswoche während der Pause, oder er gehört in ein anderes Fenster.** **So oder so nicht verwendbar – ich führe Bolin nicht als Ausfall.**

**6. Die Agu-Fundstellen aus der Sommervorbereitung** (siehe Korrektur 4). **Verworfen als älterer Stand.**

**7. Die Coufal-Fundstelle aus einem Mainz-Spiel** (siehe Korrektur 1). **Verworfen – und sie hat mir eine Angabe genommen, statt eine zu geben.**

## Offen benannte Restlücken und Unsicherheiten

- **Die formale Proxy-Gegenprobe fehlt zum zweiten Mal** (siehe Quellenlage). **Dafür ist die Sperre heute über drei Domains breit belegt statt über eine.**
- **Hoffenheims Personallage ist jetzt zum dritten Mal in Folge nicht aktualisiert – und heute zusätzlich entwertet.** **Nach Korrektur 1 führe ich Kramarić und Coufal als *unbekannt*.** **Die Heimseite dieser Partie ist damit die am schlechtesten belegte des gesamten Spieltags, und das ist kein Einzelfall mehr, sondern ein Dauerzustand von drei Läufen.**
- **Ryersons Diagnose ist weiter nicht veröffentlicht; heute kam dazu nichts Neues.** Es bleibt bei: kein Langzeitausfall erwartet, Einsatz am 09.10. unsicher.
- **Schlotterbecks Ausfalldauer ist weiterhin keine Vereinsangabe.** **„Zwei bis drei Wochen" bleibt Ersteinschätzung, eine Rückkehrankündigung zum 09.10. liegt nicht vor.** **Heute habe ich zu ihm nur Material gefunden, das in frühere Verletzungsepisoden gehört** (ein „Comeback vor der Länderspielpause denkbar" sowie eine Rückkehr ins Training vom 02.09.2026).
- **Zu Dortmund gibt es heute insgesamt keine verwendbare neue Fundstelle.** Das ist der zweite Tag in Folge ohne Bewegung auf der Heimseite dieser Partie.
- **Die Trainerfrage ist heute an zwei Stellen schlechter statt besser belegt.** **Zu Leverkusen bleibt der Name ungeklärt** (zwei verschiedene Angaben in zwei Läufen, heute nichts Neues). **Neu hinzu: Ich führe Köln unter René Wagner und Paderborn ohne Namen, finde heute aber Fundstellen, die Lukas Kwasniok dem 1. FC Köln zuordnen, und eine weitere, die Kwasniok im März 2026 bei Paderborn entlassen sieht.** **Diese Angaben sind untereinander widersprüchlich und für mich nicht auflösbar.** **Ich nenne die Trainer deshalb unten nur dort, wo ich sie in mehreren Läufen gleichlautend hatte.**
- **Unions Testspiel beim BAK 07: Zu diesem Punkt habe ich heute nicht gesucht.** Ich trage die Lücke unverändert fort, statt sie als geprüft auszugeben.
- **Die dritte Leipziger Niederlage bleibt unzuordenbar – sechster Lauf mit derselben Lücke, heute ebenfalls nicht erneut geprüft.**
- **Zu Freiburg habe ich heute keine einzige verwendbare neue Fundstelle.** **Damit ist der zweite Teil meiner Freiburg-Schalke-Schwelle – ein *neuer* Freiburger Ausfall – nicht etwa widerlegt, sondern ungeprüft geblieben.** Das ist ein Unterschied, und er geht zulasten der Belegqualität.
- **Zu Paderborn und zu Augsburg habe ich heute ebenfalls nichts Partiebezogenes gefunden.** Beide Partien stehen damit auf dem gestrigen Stand.
- **Die Tabelle ist aus den einzeln belegten Ergebnissen gerechnet**, weil keine Tabellenseite abrufbar ist. Seit dem 20.09. wurde nicht gespielt. **Heute keine neue externe Gegenprobe; es bleibt bei der gestrigen Bestätigung von Platz 3** (Freiburg, 10 Punkte, vier Spieltage).

### Tabelle nach dem 4. Spieltag

Aus den einzeln belegten Ergebnissen gerechnet. **Form = 1. bis 4. Spieltag von links nach rechts.** Werte unverändert – seit dem 20.09. wurde nicht gespielt.

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
- **Gladbach auswärts:** 0:3 in Leipzig, 0:5 in Freiburg – **null Tore, 0:8.**
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
*unverändert* — **und heute der Tipp mit dem geringsten Zuwachs an Material: zu beiden Mannschaften habe ich nichts Neues, das sich auf den 09.10. datieren lässt.**

***Auf Dortmunder Seite ist heute nichts hinzugekommen.*** **Meine Schwelle verlangt eine Ryerson-Freigabe oder eine BVB-Rückkehrankündigung zu Schlotterbeck mit Bezug auf den 09.10. oder auf Werder.** **Weder noch.** **Was ich zu Schlotterbeck finde, gehört in frühere Episoden** – eine Rückkehr ins Training am 02.09.2026 und ein „Comeback vor der Länderspielpause denkbar", beides vor der Außenbandverletzung vom 30.09. **Es bleibt deshalb bei: Schlotterbeck Außenbandverletzung im rechten Sprunggelenk (30.09., DFB-Training, Ersteinschätzung zwei bis drei Wochen, keine Vereinsangabe, Einsatz am 09.10. gefährdet); Ryerson Rippenverletzung, kein Langzeitausfall erwartet, Einsatz unsicher; dazu Emre Can (Kreuzbandriss), Justin Lerma, Filippo Mane, Giannis Konstantelias.** **Innenverteidigung: Anton und Gadou.**

***Auf Werder Seite bleibt der gestrige Stand, und ich musste ihn heute gegen ältere Fundstellen verteidigen*** (Korrektur 4). **Unverändert: Felix Agu (Wadenverletzung, unter den Fehlenden), Karl Hein (muskuläre Probleme, Torhüter), Moussa Ndiaye (Leistenprobleme), Itten fraglich; dazu die Langzeitfälle Jens Stage, Justin Njinmah, Salim Musah, Keke Topp und Senne Lynen.** **Thiounes Ansage nach dem 0:7 in Enschede – „Ich erwarte eine Reaktion. Schon im Training am Montag und besonders im Spiel gegen Dortmund" – bleibt das beste Argument gegen einen hohen Dortmunder Sieg.**

***Warum 3:1 bleibt:*** **Das Gegentor in meinem Tipp stammt nicht aus Werders Stärke, sondern aus Dortmunds Improvisation rechts und zentral hinten – und genau diese Improvisation ist heute zum zweiten Mal in Folge unverändert belegt.** **Ein Tipp, dessen Gegentor auf der Heimelf begründet ist, wird nicht sauberer, wenn beim Gast weitere Namen fehlen.** **3:1 bleibt.**

***Die Schwelle für den nächsten Lauf, unverändert:*** **Wird Ryerson belegt fit gemeldet oder Schlotterbecks Rückkehr vom BVB angekündigt – mit Bezug auf den 09.10. oder auf Werder, nicht auf einen anderen Gegner –, gehe ich auf 3:0. Fällt ein Dortmunder Innenverteidiger zusätzlich aus, gehe ich auf 2:1.** **Da dies der Freitagabend-Anstoß ist, bleibt mir dafür genau ein weiterer Lauf.**

### FC Augsburg – FC Bayern München
**Samstag, 10.10.2026, 15:30 Uhr** (WWK Arena)
**Tipp: 1:2**
*unverändert* — **und heute mit einer Abschwächung auf der Bayern-Seite, die den Tipp nicht bewegt, aber meine gestrige Formulierung zurücknimmt.**

***Musialas Diagnose ist heute strittig, sein Fehlen nicht*** (Korrektur 2). **Zwei miteinander unvereinbare Darstellungen liegen vor: Muskelfaserriss im rechten Oberschenkel beim Aufwärmen vor dem Niederlande-Spiel am 25.09. gegen Hüftprellung mit vorsorglicher Nicht-Nominierung durch Nagelsmann.** **Beide beschreiben ihn als derzeit nicht einsatzfähig; in der für Bayern günstigeren Version arbeitet die medizinische Abteilung nach der Pause erst darauf hin, ihn wieder ins Gruppentraining zu bringen.** **Ich halte am Ausfall fest und nehme das gestrige „partiebezogen belegt" zurück.**

***Ein zweiter Bayern-Ausfall mit Diagnose – das wäre die Schwelle – liegt nicht vor.*** **Ich habe heute nichts gefunden, was einen weiteren Münchner Namen für den 10.10. ausschließt.** **Konrad Laimer führe ich weiter nicht als Ausfall.** **Verworfen habe ich dazu eine Fundstelle, die Musiala einen Muskelbündelriss „beim 3:1-Sieg in Augsburg" zuschreibt – diese Partie ist meine, sie ist nicht gespielt** (Verworfene Fundstellen, Punkt 3).

***Auf Augsburger Seite nichts Neues.*** **Der Stand bleibt: Steve Mounié im Aufbautraining, Juma Bah offen, Gregoritsch verfügbar – und die Kade-Entwarnung, die ich gestern nach eigener Schwelle ausdrücklich nicht angewendet habe.** **Das Thema bleibt erledigt und wird nicht wieder aufgenommen.**

***Neu und rein terminlich:*** **Bayern hat heute, am 06.10., das Mannschaftstraining aufgenommen – vier Tage vor dem Anpfiff.** *Kein Argument; diese Lage hat Bayern in jeder Länderspielpause.*

***Warum 1:2 bleibt, in einem Satz:*** **Augsburg hat zu Hause in zwei Spielen fünf Tore erzielt und steht auf Platz 4 – ein Tor ist die Mindestzahl, die dazu passt; Bayern hat in vier Spielen zwei Gegentore kassiert – mehr als ein Tor ist gegen diese Abwehr nicht zu begründen.**

***Die Schwelle für den nächsten Lauf, unverändert:*** **Nur ein zweiter belegter Bayern-Ausfall mit Diagnose bewegt diesen Tipp auf 2:2.**

### TSG Hoffenheim – Hamburger SV
**Samstag, 10.10.2026, 15:30 Uhr** (SNP Arena)
**Tipp: 2:0**
*unverändert* — **und heute kippt das Ungleichgewicht dieser Partie noch weiter: die Gästeseite ist so gut belegt wie keine zweite im Spieltag, die Heimseite ist heute sogar schlechter belegt als gestern.**

***Die HSV-Sturmnot ist heute zum sechsten Mal bestätigt – und erstmals mit einem Rückkehrtermin, der nach meinem Spieltag liegt.***
- **Patson Daka: Muskelfaserriss im linken Oberschenkel, zugezogen in den Länderspielen mit Sambia; die nächste Bundesligapartie des HSV ist der 10.10. bei der TSG.** *Heute präziser als bisher – mit Muskel, Seite und Entstehungszusammenhang.*
- **Albert Grønbæk: Muskelfaserriss im Oberschenkel, drei bis vier Wochen, Hoffnung auf eine Rückkehr zum Heimspiel gegen den VfB Stuttgart am 17.10.** ***Das ist der wichtigste neue Satz des Tages für diesen Tipp:*** **Ein genannter Rückkehrtermin am 17.10. schließt den 10.10. aus.** **Bisher stand hier nur „verletzt aus der Länderspielpause zurückgekehrt".**
- **Terem Moffi: Knieprobleme, arbeitet individuell, kann nicht regulär mit der Mannschaft trainieren; das Spiel am 10.10. in Hoffenheim „könnte zu früh kommen".**
- **Als fitte Mittelstürmer bleiben Merlin Polzin Yussuf Poulsen und der junge Otto Stange.** **Poulsens Entwarnung steht unwidersprochen; die eine Fundstelle, die ihn als verletzt führt, gehört in den April 2026 und ist heute über eine zweite Quelle als solche bestätigt** (Verworfene Fundstellen, Punkt 4).
- **Mario Vuskovic: gesperrt bis 15.11.2026**, unverändert.

***Hoffenheims Lage ist heute nicht nur wieder nicht aktualisiert, sie ist schlechter als gestern*** (Korrektur 1). **Kramarić und Coufal führe ich ab heute als *unbekannt* statt als angeschlagen, weil die einzige Coufal-Fundstelle, die ich finde, ein Spiel gegen Mainz beschreibt – das Hoffenheim in dieser Saison nicht bestritten hat.** **Belegt bleibt auf Heimseite praktisch nur der Trainername Christian Ilzer und das 2:3 gegen Elversberg vom 02.10., entschärft durch die gemischte Elf und 18 abgestellte Profis.** **Prass und Asllani führe ich weiter als unbekannt.**

***Warum 2:0 trotzdem bleibt:*** **Der Tipp ruht auf der Gästeseite, und die ist heute besser belegt als je zuvor – drei Angreifer namentlich und diagnostisch weg, einer davon nachweislich erst zum 17.10. zurück erwartet, dazu null Auswärtstore in zwei Spielen.** **Dagegen ein Gastgeber mit vier Heimtoren in zwei Spielen.** ***Und die ehrliche Einschränkung, die heute größer ist als gestern:*** **Ich tippe hier ein Heimergebnis, über dessen Heimmannschaft ich seit drei Läufen nichts Belastbares weiß.** **Das ist die schwächste Belegbasis der neun Tipps – schwächer sogar als Union – Elversberg, wo ich wenigstens einen stabilen Ausfallstand habe.**

***Die Schwelle für den nächsten Lauf, angepasst:*** **Wird Kramarić oder Coufal belegt als Ausfall gemeldet – mit Bezug auf den 10.10. –, gehe ich auf 1:0. Kommt ein HSV-Angreifer belegt zurück oder fällt Poulsen doch aus, gehe ich auf 2:1 bzw. 3:0.** **Neu ab heute: Bleibt die Hoffenheimer Seite auch im nächsten Lauf ohne jede partiebezogene Fundstelle, gehe ich auf 1:0 – nicht weil ein Ausfall belegt wäre, sondern weil ein Zwei-Tore-Heimtipp vier Läufe ohne Heiminformation nicht verdient.**

### 1. FSV Mainz 05 – Bayer 04 Leverkusen
**Samstag, 10.10.2026, 15:30 Uhr** (MEWA Arena)
**Tipp: 1:1**
*unverändert* — **und heute mit dem größten Erkenntnisgewinn aller neun Partien, der den Tipp trotzdem nicht bewegt.**

***Teil (a), Zentner: die Vereinsangabe ist gefunden – und sie ist die falsche*** (siehe „Geschlossene Lücken"). **Belegt ist jetzt: Zentner verpasste das 5:0 beim HSV (2. Spieltag) mit muskulären Oberschenkelproblemen, und Mainz bestätigte anschließend eine Handverletzung aus dem 1:3 gegen Frankfurt (3. Spieltag), Ausfall „für die kommenden Wochen", Rückkehr abhängig vom Heilungsverlauf, Schwolow vertritt.** **Zwei Vorgänge, nicht einer – das erklärt die widersprüchlichen Meldungen der letzten vier Läufe.**

**Meine Schwelle verlangt eine Mainzer Angabe dazu, *ob er am 10.10. spielt*.** **Eine Erstmeldung von Mitte September ist das nicht.** **Nicht ausgelöst – 1:1 bleibt.** *Die Richtung bleibt die von gestern:* **Die Aggregatorlage bewegt sich auf einen Einsatz zu („Mainz hofft auf Zentner-Rückkehr gegen Leverkusen"), und wenn Mainz das bestätigt, steht hier 2:1.**

***Teil (b), Nebel und Leverkusener Rückkehrer: heute nichts Neues.*** **Weder eine datierbare Nebel-Absage für den 10.10. noch ein belegter Leverkusener Rückkehrer von meiner Ausfallliste.** **Die gestrige Verwerfung bleibt gültig: Die „Mainz 05 bestätigt wochenlange Pause für Paul Nebel"-Meldung ist die Erstmeldung aus dem August 2026 (Adduktorenverletzung aus der letzten Einheit im Trainingslager Hopfgarten).** **Nicht ausgelöst.**

***Die Ausfallbilanz, unverändert bei sechs gegen drei.***
- **Mainz: Dominik Kohr** (nach Operation), **Silas** (Schien- und Wadenbeinbruch, sechs Monate), **Silvan Widmer** (Patellasehne, mehrere Wochen, kein Termin – Kapitän), **Paul Nebel** (Adduktoren, seit dem Trainingslager, Rückkehr laut Aggregator 10.10.), **Katompa Mvumpa** und **Caci** (beide nur Listeneintrag). **Dazu Zentner als siebtes Fragezeichen – heute besser verstanden, aber nicht aufgelöst.**
- **Leverkusen: Doué** (Wadenmuskel), **Eichhorn** (Stoffwechselerkrankung), **Culbreath** (nur Listeneintrag).
- **Pausenform, unverändert:** Mainz 3:0 beim Drittligisten SV Waldhof (03.10.), Leverkusen 6:0 gegen den Drittligisten Fortuna Köln (02.10., mit sechs U19-Spielern). **Zwei Siege gegen Drittligisten – das trennt nichts.**

***Warum 1:1 bleibt, unverändert:*** **Beide Mannschaften haben 7 Punkte, und die entscheidende Symmetrie ist eine Schwäche-Symmetrie: Mainz hat zu Hause einen Punkt aus zwei Spielen bei 1:3 Toren, Leverkusen auswärts einen Punkt aus zwei Spielen bei 4:5 Toren und keinen Auswärtssieg.**

***Die Schwelle für den nächsten Lauf, unverändert und um die heutige Erfahrung ergänzt:*** **(a)** **Nur eine Mainzer Vereinsangabe dazu, *ob Zentner spielt*, bewegt diesen Tipp** – spielt er, 2:1; spielt er nicht, 1:2. **Ab heute ausdrücklich: Eine Vereinsbestätigung *der Verletzung* ist keine Aussage über den Einsatz; ich prüfe jede Zentner-Vereinsmeldung zuerst darauf, ob sie den 10.10. nennt.** **(b)** **Ein belegter Leverkusener Rückkehrer von meiner Ausfallliste oder eine auf den 10.10. datierbare Nebel-Absage bringt 1:2.**

### 1. FC Union Berlin – SV 07 Elversberg
**Samstag, 10.10.2026, 15:30 Uhr** (Alte Försterei)
**Tipp: 1:2**
*unverändert* — **und heute mit der Lücke geschlossen, die ich sechs Läufe lang mitgeschleppt habe, und mit einer Beinahe-Änderung, die an zwei unabhängigen Prüfungen gescheitert ist.**

***Tom Zimmerschied ist Elversberger*** (siehe „Geschlossene Lücken"). **Linksaußen, gewechselt am 21.08.2024 mit Dreijahresvertrag.** **Der Satz „bleibt auf keiner Seite belegt" entfällt ab heute.**

***Und beinahe wäre daraus eine Tippänderung geworden.*** **Eine Aufstellungsseite zur Partie führt „Zimmerschied (Rückenverletzung, out)" und „Seifert (Knöchelverletzung, out)" – unter *Union Berlin*.** **Beide sind Elversberger.** **Das ist dieselbe Seitenvertauschung, die ich gestern bei dieser Partie schon verworfen habe.** **Nach der Korrektur der Seite wäre Zimmerschied ein zweiter Elversberger Ausfall mit Diagnose gewesen – und damit meine Schwelle.**

***Er ist es nicht, und das entscheidet die Datierung:*** **Zimmerschieds Rückenverletzung ist in der Verletzungshistorie auf den 02. bis 18. Oktober 2024 datiert.** **Die Seite zieht einen zwei Jahre alten, längst abgelaufenen Historieneintrag als aktuellen Ausfall ein.** **Nicht ausgelöst.** *Der dritte dort genannte Name – „Onyeka fraglich" – ist mir keiner Seite zuzuordnen; ich führe ihn nicht.*

***Der Stand bleibt deshalb der von gestern.*** **Union: Robert Skov, Marvin Friedrich, Andrej Ilić, Oliver Burke, Stanley Nsoki, Andrik Markgraf (Kreuzbandverletzung), Frederik Rønnow (Oberschenkel, weiter als fraglich geführt).** **Sechs sichere Ausfälle plus ein fraglicher, sieben Läufe lang namentlich identisch.** **Elversberg: ein belegter Ausfall, Luis Seifert (Knöchel, Langzeitfall – heute über eine zweite Quelle bestätigt).** **Zu Rønnow heute nichts Neues; die Baumgart-Probe von gestern hat keine neue Fundstelle zu prüfen gehabt.**

***Historisch belegt und heute neu:*** **Union und Elversberg sind sich noch nie in einem Pflichtspiel begegnet, auch nicht im DFB-Pokal; für Elversberg ist die Alte Försterei das erste Auswärtsspiel in einem Stadion dieser Größe.** *Das ist kein Tipp-Argument, aber es erklärt, warum zu dieser Partie so wenig direkte Vergleiche existieren – ich habe sie in sieben Läufen nie gefunden, und jetzt weiß ich, dass es keine gibt.*

***Die Abwägung, unverändert:*** **Elversberg hat als Aufsteiger in Gladbach 4:3 und gegen Leverkusen 3:2 gewonnen – der Club trifft, und er trifft auswärts.** **7 Punkte gegen 1, 8:7 gegen 4:17, ein Ausfall gegen sechs.** **Union hat in vier Spielen 17 Gegentore kassiert, keinen Sieg und einen Punkt.** **Das Elversberger 3:2 bei Hoffenheim vom 02.10. ziehe ich weiter ab (gemischte TSG-Elf).** **1:2 bleibt.**

***Die Schwelle für den nächsten Lauf, unverändert und geschärft:*** **Nur eine belegte Rønnow-Entwarnung oder ein zweiter Elversberger Ausfall mit Diagnose bewegt diesen Tipp.** **Ab heute ausdrücklich: Ausfälle von Aufstellungs- und Trackingseiten prüfe ich erstens auf die Seitenzuordnung und zweitens auf das Datum des Historieneintrags. Heute hätte jede der beiden Prüfungen allein gereicht, um einen Fehler zu verhindern.**

### SC Paderborn 07 – VfB Stuttgart
**Samstag, 10.10.2026, 15:30 Uhr** (Home Deluxe Arena)
**Tipp: 1:2**
*unverändert* — **und heute ohne jede neue Fundstelle zu beiden Mannschaften. Ich schreibe das hin, statt die gestrigen Argumente umzuformulieren.**

***Zu Stuttgart habe ich heute nichts Partiebezogenes gefunden.*** **Der Stand bleibt der gestrige, und er ist gut: „Gegen SC Paderborn 07 fehlen dem VfB: Justin Diehl (Langzeitverletzter), Jarzinho Malanga (Bauchmuskelverletzung), Dan-Axel Zagadou (Individualprogramm)." Kein vierter Name.** **Die zweite Hälfte meiner Schwelle – ein Stuttgarter Ausfall mit Diagnose – ist damit zum dritten Mal in Folge nicht erfüllt.** *Heute allerdings nur „nicht gefunden", nicht wie gestern „belegt nicht erfüllt".*

***Das gestern gestrichene Torwart-Argument bleibt gestrichen.*** **Hoeneß hat Seimens Pflichtspiel-Comeback offengelassen („Wir lassen uns in keiner Weise drängen") und Jobsharing angekündigt.** **Ich nehme es nicht wieder auf.**

***Zu Paderborn habe ich heute ebenfalls nichts gefunden – und dabei ist mir eine Unsicherheit über den Trainer aufgefallen, die ich offen nenne.*** **Eine Fundstelle datiert Lukas Kwasnioks Entlassung in Paderborn auf den 22. März 2026 nach einem 3:3 gegen Gladbach, eine andere macht ihn zum Kölner Cheftrainer.** **Beide zusammen ergeben keinen stimmigen Verlauf, und ich kann sie nicht auflösen.** **Ich nenne den Paderborner Trainer deshalb nicht.** **Der Personalstand bleibt: Curda, Obermair, Hansen und Baack nach der Erkältungswelle gesund, die USA-Reise mit dem 1:0 bei D.C. United am 01.10. als Belastungsfaktor.**

***Stuttgarts Pausenform, unverändert:*** **zwei Testspiele, zwei Siege, 8:0 – 3:0 gegen Heidenheim und 5:0 gegen Greuther Fürth.**

***Warum 1:2 bleibt:*** **Paderborn hat in drei Heimspielen vier Punkte und drei Saisontore insgesamt bei 3:5 – die schwächste Heimoffensive des Spieltags.** **Dagegen ein Auswärtsteam mit 2:7, das in der Pause 8:0 testet und dessen drei Ausfälle sich im Aufbau befinden.** **Der Tipp stand nie auf dem Torwart, sondern auf drei Paderborner Toren in vier Spielen.**

***Die Schwelle für den nächsten Lauf, unverändert:*** **Nur ein Stuttgarter Ausfall mit Diagnose oder ein belegter Paderborner Rückkehrer in der Offensive bewegt diesen Tipp.**

### RB Leipzig – Eintracht Frankfurt
**Samstag, 10.10.2026, 18:30 Uhr** (Red Bull Arena)
**Tipp: 2:1**
*unverändert* — **und heute wird die gestrige Abschwächung wieder zurückgenommen: Lukebas Trainingsstand ist eine Stufe höher belegt als gestern.**

***Die neueste Lukeba-Meldung (Nummer 418597, über den gestrigen 418481 und 418564) trägt die Überschrift „Lukeba vor Rückkehr ins volle Teamtraining".*** **Ihr Inhalt:** **Lukeba macht Fortschritte bei seinen Leistenproblemen und soll in der kommenden Woche vollständig ins Mannschaftstraining integriert sein; er absolviert bereits Teile des Mannschaftstrainings, die Belastung wird in den nächsten Tagen schrittweise gesteigert; ein Startelfeinsatz gegen Eintracht Frankfurt am 10.10. rückt in den Blick.**

***Das ist die Gegenbewegung zu gestern, und ich sage, wie weit sie reicht:*** **Gestern musste ich „bereits im Mannschaftstraining, voll verfügbar erwartet" auf „teilintegriert" zurücknehmen. Heute steht die Richtung wieder nach oben – „vor der Rückkehr ins volle Teamtraining", Startelf im Blick.** **Was weiterhin fehlt, ist dasselbe wie gestern: eine Vereinsangabe.** **Die Meldung ist ein Aggregator, die Vereinsmeldung (`rbleipzig.com/de/news/training-lukeba-reitz-baumgartner-comeback`) bleibt unabrufbar.**

***Meine beiden Schwellen, beide nicht ausgelöst:*** **(1) Eine Leipziger Vereinsangabe, dass Lukeba nicht spielt, liegt nicht vor.** **(2) Meine gestern neu gesetzte Frist – „Bringt der 07.10. oder 08.10. keine Bestätigung, dass Lukeba im vollen Mannschaftstraining ist, gehe ich auf 1:1" – ist heute, am 06.10., noch nicht fällig.** *Sie bleibt scharf gestellt, und die heutige Meldung macht ihre Erfüllung wahrscheinlicher, ersetzt sie aber nicht:* **„Vor der Rückkehr" ist nicht „zurück".**

***Der Rest der Leipziger Lage, unverändert:*** **Demichelis' Mannschaft ist nach der freien Woche am Cottaweg ins Training zurückgekehrt; Raum, Orbán und Nusa kehren im Lauf dieser Woche von den Nationalmannschaften zurück; Reitz und Baumgartner machen Fortschritte, fehlen aber gegen Frankfurt.** **Nach dem Spieltag folgt das Champions-League-Heimspiel gegen PSV Eindhoven – ein Rotationsargument, aber keines gegen den Heimvorteil am Samstag.**

***Auf Frankfurter Seite habe ich heute eine Fundstelle gehabt, die genau meine Partie zu betreffen schien, und sie ist an der Uhr gescheitert*** (Verworfene Fundstellen, Punkt 2). **Eine Spieltags-Pressekonferenz meldet Hugo Larsson und Can Uzun als mögliche Rückkehrer „für das Auswärtsspiel in Leipzig (Samstag, 18:30)" nach einem Donnerstagstraining, mit Verweis auf das Abschlusstraining am Freitag, und Jonathan Burkardt als definitiven Ausfall.** **Heute ist Dienstag, der 06.10.; der Donnerstag dieser Woche ist der 08.10.** **Eine PK, die ein Donnerstagstraining im Rückblick schildert, kann nicht vor heute über den 10.10. gehalten worden sein.** **Verworfen – vollständig, samt Burkardt.**

**Es bleibt deshalb beim gestrigen Frankfurter Stand:** **Maluze im Reha-Training und nicht einsatzfähig; Dreierkette nach aktuellem Stand Robin Koch, Nnamdi Collins, Lilian Brassier; Robin Koch nach Infekt zurück, Dōan fit; 4:0 gegen Braunschweig am 02.10.**

***Die Zahl, die Lukebas Gewicht trägt, heute zum zweiten Mal extern bestätigt:*** **In beiden Bundesligaspielen mit Lukeba in der Startelf gewann Leipzig zu null – 3:0 gegen Gladbach, 5:0 gegen den HSV. Ohne ihn kamen die Niederlagen: 1:3 in Bremen, 0:2 in Leverkusen.**

***Warum 2:1 bleibt:*** **Leipzigs Heimbilanz ist 8:0 mit zwei Zu-null und sie ist Lukebas Bilanz; er rückt in die Startelf-Diskussion statt aus ihr heraus.** **Das Gegentor steht für Frankfurts Auswärtsstärke – vier Punkte bei 6:4, auswärts besser als zu Hause.**

***Die Schwellen für den nächsten Lauf, unverändert:*** **Kommt eine Leipziger Vereinsangabe, dass Lukeba nicht spielt, gehe ich auf 1:1 und bleibe dort bis zum Anpfiff.** **Und: Bringt der 07.10. oder 08.10. keine Bestätigung, dass Lukeba im vollen Mannschaftstraining ist, gehe ich auf 1:1.** **Die zweite Frist wird im nächsten Lauf fällig.**

### 1. FC Köln – Borussia Mönchengladbach
**Sonntag, 11.10.2026, 15:30 Uhr** (RheinEnergieStadion)
**Tipp: 1:0**
*unverändert* — **und das ist heute der Tipp, bei dem ich am meisten gegen mich selbst geprüft habe. Er ist auch der riskanteste der neun.**

***Die Fundstelle, die diesen Tipp gekippt hätte, ist verworfen*** (Verworfene Fundstellen, Punkt 1). **Ein „doppelter Verletzungsschock" vor dem Derby – El Mala mit Knöchelverletzung beim Trainingsabbruch, Kamiński nach einem Schlag auf den Fuß nur individuell – wäre für mein 1:0 das Ende gewesen: Köln fehlen in meiner Rechnung ohnehin beide Mittelstürmer.** **Die Fundstelle nennt beide aber „die gefährlichsten Torschützen des *Aufsteigers*" mit **neun** und **sechs** Saisontoren.** **Köln ist in dieser Saison kein Aufsteiger, und Köln hat in vier Spieltagen insgesamt sechs Tore erzielt – neun Saisontore eines einzelnen Spielers sind arithmetisch unmöglich.** **Vorsaison, 27. Spieltag, verworfen.**

***Und ich nenne die Gegenprobe, die *nicht* funktioniert hat, weil das zur Ehrlichkeit gehört:*** **Ich wollte die Verwerfung über El Malas Alter absichern („19-Jähriger" passt nicht zu Oktober 2026).** **Das trägt nicht – auch Meldungen vom August 2026 bezeichnen ihn als 19-Jährigen.** **Die Verwerfung ruht allein auf „Aufsteiger" und auf den neun Toren.** **Sollte sie falsch sein, ist mein 1:0 zu hoch.** **Das ist das größte Einzelrisiko dieses Spieltags, und es steht hier, statt in einer Fußnote.**

***Dafür habe ich heute eine Lücke meiner eigenen Kölner Liste entdeckt*** (siehe „Geschlossene Lücken"). **Saïd El Mala ist aktueller Kölner Spieler – Vertrag im August 2026 bis 2031 verlängert, Rückennummer 10, drei abgelehnte Dortmunder Angebote.** **In fünf Läufen Kölner Personaldiskussion kam er bei mir nie vor.** **Das ist kein neuer Vorgang, sondern eine alte Lücke, und ich ziehe daraus ausdrücklich keine Tippänderung – über seinen aktuellen Zustand weiß ich nichts.**

***Gladbachs Derby-Ausfälle sind heute an einer Stelle besser belegt.*** **Nicolas Kühn: Muskelbündelriss, zugezogen im Training nach dem 3:4 gegen Elversberg (2. Spieltag), Ausfall fünf bis sechs Wochen.** ***Das ist neu und es ist eine Zahl:*** **Fünf bis sechs Wochen ab Anfang September reichen über den 11.10. hinaus.** **Kühn fehlt im Derby, und das ist jetzt gerechnet, nicht vermutet.** **Unverändert dazu: Franck Honorat (Muskelverletzung, „auf unbestimmte Zeit", verpasst voraussichtlich auch das Folgespiel gegen Hoffenheim), Enzo Leopold (Kreuzbandriss), Jens Castrop (nach Schulteroperation im Lauftraining, Derbyteilnahme gilt als nicht realistisch – heute über eine zweite Quelle bestätigt, die ihn als Doppeltorschützen eines früheren Derbys führt).**

***Kölns Sturmzentrum bleibt eine Prognose.*** **Bülter Favorit (44 seiner 182 Bundesligaspiele als Mittelstürmer), Alternativen Thielmann, Waldschmidt, Maina.** **Dallinga (Kreuzbandverletzung, Monate) und Ache (Oberschenkelmuskelverletzung, „vorerst") fehlen beide.** **Eine Vereinsangabe gibt es weiterhin nicht.**

***Zur Trainerlage, heute unsicherer statt sicherer.*** **Gladbach: Alexander Blessin (53), Vertrag bis 2028, das Derby ist sein Bundesliga-Debüt für die Borussia, nach zwei ungeschlagenen Tests (3:0 in Siegen, 1:1 bei St. Pauli) – heute erneut bestätigt, samt dem Zitat von seiner Vorstellung: „Ich will aus dieser Scheißzeit eine gute Zeit machen."** **Köln: Ich habe René Wagner geführt, finde heute aber Fundstellen, die Lukas Kwasniok dem 1. FC Köln zuordnen, sowie eine Überschrift, die eine Derbyniederlage mit dem Ende einer „Wagner-Ära" in Köln verknüpft.** **Ich kann das nicht auflösen und nenne den Kölner Trainer deshalb heute nicht.** *Für den Tipp ist das ohne Gewicht – er steht auf Toren und Ausfällen, nicht auf der Bank.*

***Kleindienst bleibt das beste Argument gegen mein 1:0*** – gestrige Auflösung unverändert: Erkältung vor dem Siegen-Test, danach Rückkehr und Kopfballtor bei St. Pauli, heute nicht widersprochen.

***Warum 1:0 bleibt, in einem Satz:*** **Ein Gastgeber ohne beide Mittelstürmer, aber zu Hause gegen die schlechteste Defensive der Liga (16 Gegentore in vier Spielen, keine Partie unter drei), gegen einen Gast, der auswärts noch kein Tor erzielt hat (0:8), Letzter ist und im Derby vier Offensiv- und Mittelfeldspieler nicht einsetzen kann – bei einem davon ist die Ausfalldauer seit heute durchgerechnet.**

***Die Schwelle für den nächsten Lauf, unverändert und um einen Zweig ergänzt:*** **Kommt eine Kölner Vereinsangabe, dass ein Nachwuchsspieler im Sturmzentrum beginnt, gehe ich auf 0:0. Kommt eine belegte Gladbacher Entwarnung zu Honorat oder Kühn, gehe ich auf 1:1 zurück.** **Neu ab heute: Findet sich eine auf diese Woche datierbare Meldung zu einem Kölner Offensivausfall – El Mala, Kamiński oder ein anderer –, gehe ich auf 0:0. Ich habe heute eine solche Meldung verworfen und möchte nicht, dass die Verwerfung mich beim nächsten Mal blind macht.**

### SC Freiburg – FC Schalke 04
**Sonntag, 11.10.2026, 17:30 Uhr** (Europa-Park-Stadion)
**Tipp: 2:0**
*unverändert* — **und heute ist die Schalker Hälfte unabhängig bestätigt, während die Freiburger Hälfte ungeprüft geblieben ist.**

***Ljubičić ist heute über eine zweite, unabhängige Quelle als Ausfall bestätigt und präziser datiert.*** **Knieverletzung im linken Knie, Auswechslung in der 21. Minute im Auswärtsspiel bei Union Berlin am Freitag, dem 11. September (3. Spieltag); ein Kreuzbandriss wurde ausgeschlossen; er steht Schalke „bis auf Weiteres" nicht zur Verfügung, und ein Einsatz im Spiel beim SC Freiburg nach der Länderspielpause am 11.10. erscheint unwahrscheinlich.** **Nicht fit gemeldet – meine Schwelle ist nicht ausgelöst.** *Gestern stand hier „Auswechslung in der ersten Halbzeit", heute ist es die 21. Minute und das linke Knie.*

***Becker ist bestätigt, die Verletzungsart aber uneinheitlich*** (Korrektur 3). **Auswechslung nach gut einer Stunde im 0:0 gegen Elversberg am 20.09., nach einem Schlag auf den rechten Fuß.** **Gestern stand hier „Fleischwunde am Knöchel".** **Spiel, Datum und Minute stimmen, die Beschreibung nicht.** **Am Ergebnis ändert das nichts: fraglich für Freiburg; fällt er aus, rückt Maximilian Wober in die Startelf.**

***Ein dritter Schalker Name kommt heute hinzu:*** **Emil Højlund fehlt nach derselben Quelle längerfristig; außer Ljubičić habe Trainer Miron Muslic keine größeren Personalsorgen.** *Ein Langzeitausfall, den ich bisher nicht geführt habe – nach meiner gestern gesetzten Regel trage ich ihn nach und rechne ihn nicht ein.*

***Zu Freiburg habe ich heute keine einzige verwendbare Fundstelle, und das ist die ehrliche Schwäche dieses Laufs.*** **Der zweite Teil meiner Schwelle – ein *neuer* Freiburger Ausfall, zugezogen nach dem 20.09. und mit Diagnose – ist damit nicht widerlegt, sondern ungeprüft.** **Es bleibt beim gestrigen Stand: Florent Muslija als Langzeitausfall (Kreuzbandriss, rund fünf Monate und drei Wochen) nachgetragen und nicht eingerechnet, 4:0 im Pausentest gegen den FC Luzern, 10 Punkte aus vier Spieltagen auf Platz 3.**

***Der Schalker Rahmen bleibt der terminlich wichtigste Punkt:*** **öffentliche Trainingseinheiten am Mittwoch, 07.10., und Freitag, 09.10., jeweils 10:45 Uhr; Pressekonferenz am Freitag, 14:00 Uhr im Medienzentrum der Veltins-Arena.** **Dort entscheidet sich die Ljubičić- und Becker-Frage, und mein letzter Lauf vor dieser Sonntagspartie liegt danach.**

***Warum 2:0 bleibt, in einem Satz:*** **Ein Heimteam mit neun Toren in zwei Heimspielen, 10 Punkten, Platz 3 und einem 4:0 im Pausentest gegen einen Gast mit 3:4 Toren in vier Spielen – der schwächsten Offensive der Liga –, dem der Mittelfeldmotor nach heute erneut bestätigtem Stand „bis auf Weiteres" fehlt und dessen Innenverteidiger kaum rechtzeitig fit wird.**

***Die Schwelle für den nächsten Lauf, unverändert:*** **Wird Ljubičić belegt fit gemeldet oder kommt ein Schalker Offensivspieler belegt zurück, gehe ich auf 2:1.** **Ein *neuer* Freiburger Ausfall – zugezogen nach dem 20.09. und mit Diagnose – bringt 1:0.** **Langzeitausfälle, die ich nachträglich entdecke, lösen keine Änderung aus; ich trage sie nach und rechne sie nicht ein.**

## Verteilung und Selbstkontrolle

**Die neun Tipps im Überblick:**

| Partie | Anstoß | Tipp | Status |
|---|---|---|---|
| Borussia Dortmund – SV Werder Bremen | Fr 09.10., 20:30 | **3:1** | unverändert |
| FC Augsburg – FC Bayern München | Sa 10.10., 15:30 | **1:2** | unverändert |
| TSG Hoffenheim – Hamburger SV | Sa 10.10., 15:30 | **2:0** | unverändert |
| 1. FSV Mainz 05 – Bayer 04 Leverkusen | Sa 10.10., 15:30 | **1:1** | unverändert |
| 1. FC Union Berlin – SV 07 Elversberg | Sa 10.10., 15:30 | **1:2** | unverändert |
| SC Paderborn 07 – VfB Stuttgart | Sa 10.10., 15:30 | **1:2** | unverändert |
| RB Leipzig – Eintracht Frankfurt | Sa 10.10., 18:30 | **2:1** | unverändert |
| 1. FC Köln – Borussia Mönchengladbach | So 11.10., 15:30 | **1:0** | unverändert |
| SC Freiburg – FC Schalke 04 | So 11.10., 17:30 | **2:0** | unverändert |

**Verteilung:** vier Heimsiege, vier Auswärtssiege, ein Unentschieden. **Torsumme 12:10.** **Kein Tipp über drei Toren, kein Zu-null-Tipp gegen eine Mannschaft mit Auswärtstoren.**

**Belegqualität der neun Tipps, von gut nach schwach** – *heute mit zwei Verschiebungen gegenüber gestern:*
1. **Hoffenheim – HSV (Gästeseite):** bestbelegte Einzelseite des Spieltags, heute mit Rückkehrtermin nach dem Spieltag.
2. **Union – Elversberg:** stabiler Ausfallstand, heute eine Sechs-Läufe-Lücke geschlossen.
3. **Freiburg – Schalke (Gästeseite):** heute über eine zweite Quelle bestätigt.
4. **Köln – Gladbach:** Gladbachs Ausfälle gerechnet, Kölns Offensive prognostiziert – **und mit dem größten Verwerfungsrisiko des Spieltags.**
5. **Leipzig – Frankfurt:** Lukeba wieder aufwärts belegt, Frankfurt heute unverändert.
6. **Mainz – Leverkusen:** heute am meisten verstanden, in der Sache unverändert.
7. **Paderborn – Stuttgart:** heute ohne jede neue Fundstelle.
8. **Dortmund – Werder:** zweiter Tag ohne Bewegung auf der Heimseite.
9. **Hoffenheim – HSV (Heimseite):** **die schwächste Belegbasis des Spieltags, heute schwächer als gestern** – deshalb steht dort jetzt eine Frist-Schwelle.

**Was mich an diesem Lauf am meisten beschäftigt:** **Von den beiden Fundstellen, die heute Tipps bewegt hätten, war keine erfunden und keine offensichtlich alt.** **Beide trugen den richtigen Gegner, die richtige Partie und – im Frankfurter Fall – sogar die richtige Anstoßzeit.** **Gescheitert sind sie an einer Arithmetik (neun Saisontore bei sechs Mannschaftstoren) und an einem Kalenderblick (ein Donnerstag, der noch kommt).** **Das sind die beiden Prüfungen, die diesen Lauf getragen haben, und ich schreibe sie als Methode auf, nicht als Anekdote.**

## Quellen

**Abrufversuche auf Primärquellen sind aus dieser Umgebung sämtlich gescheitert** (acht Domains mit HTTP `000`, drei WebFetch-Versuche mit `EGRESS_BLOCKED`). **Die folgenden Adressen sind über Suchergebnisse und deren Zusammenfassungen eingegangen und nicht im Volltext gelesen.**

- Spielplan und Ansetzungen: `hessenschau.de/sport/ergebnisse-tabellen/fussball-1bl100~_matchday-5.html`, `anstosszeiten.de/bundesliga/spieltag-5/`, `bundesliga.com/de/bundesliga/spieltag/2026-2027/5/tsg-hoffenheim-vs-hamburger-sv/`, `thescore.com/bund/event/99505`, `99507`, `99509`, `starting11.com/fixtures/union-berlin-vs-sv-elversberg`
- Leipzig/Lukeba: `ligainsider.de/castello-lukeba_27079/lukeba-vor-rueckkehr-ins-volle-teamtraining-418597/` (Fetch blockiert), `rbleipzig.com/de/news/training-lukeba-reitz-baumgartner-comeback` (nicht abrufbar)
- HSV: `ligainsider.de/patson-daka_16774/daka-fehlt-sambia-mit-muskelproblemen-418573/`, `ms-aktuell.de/?p=164250` (Daka), `ms-aktuell.de/?p=161736` (Grønbæk), `bundesliga.com/de/bundesliga/news/hamburger-sv-albert-groenbaek-verletzt-ausfall-39358`, `90min.de/gronbaek-comeback-schneller-als-gedacht-polzin-gibt-personalupdate`
- Schalke: `ms-aktuell.de/welt/ljubicic-schalke-ausfall-17-09-2026/`, `bulinews.com/schalke-rule-out-ljubi-indefinitely-knee-injury`, `90min.de/so-lange-fehlt-ljubicic-dem-fc-schalke`
- Mainz/Zentner: `bulinews.com/mainz-confirm-injury-setback-for-zentner`
- Gladbach/Köln: `ms-aktuell.de/?p=156781` (Kühn), `flashscore.de/news/gladbach-gewinnt-blessin-debut-bei-sportfreunde-siegen/`, `ms-aktuell.de/welt/blessin-gladbach-trainer-22-09-2026/`, `90min.de/posts/gladbach-aufstellung-und-ausfalle-so-konnte-die-borussia-im-derby-gegen-koln-antreten`
- Union/Elversberg: `de.soccerway.com/spieler/zimmerschied-tom/Qm2kw3bd/verletzungshistorie`, `starting11.com/fixtures/union-berlin-vs-sv-elversberg-20261010`
- Dortmund: `ms-aktuell.de/welt/schlotterbeck-verletzt-30-09-2026/`

**Verworfene Adressen, damit sie im nächsten Lauf nicht erneut Arbeit machen:**
`90min.de/1-fc-koln-doppelter-verletzungsschock-vor-derby-gegen-gladbach` · `watson.de/sport/fussball/619631456-...` · `t-online.de/.../id_100986872/...` · `bulinews.com/mala-sits-out-training-ahead-koln-derby-against-gladbach` (alle: Kölner Derby der Vorsaison) · `hessenschau.de/.../bundesliga-ticker-104~_p-46/47/48/116.html` (Frankfurter Archivticker) · `sport1.de/news/fussball/bundesliga/2026/04/vuskovic-fehlt-hsv-auch-gegen-hoffenheim` (April 2026) · `leinetal24.de/.../wie-lange-faellt-musiala-zr-93341713.html` (Musiala, Vorsaison) · `ligainsider.de/felix-agu_21590/...-409299/` und `...-412344/` (Agu, Sommer) · `ligainsider.de/vladimir-coufal_11929/coufal-musste-angeschlagen-vom-feld-411427/` (Coufal, andere Saison)
