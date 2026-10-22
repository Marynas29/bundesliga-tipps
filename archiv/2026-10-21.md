# Bundesliga-Tipps – 7. Spieltag 2026/27 (Stand: 21.10.2026)

**Ansetzung:** Freitag, 23.10. bis Sonntag, 25.10.2026.
**Vortagsstand:** 20.10.2026, **ebenfalls 7. Spieltag** — also ist ein echter Vergleich für alle neun Partien möglich.

**Ergebnis dieses Laufs in einem Satz:** ***Kein einziger Tipp geändert, alle neun unverändert*** — **und das ist diesmal keine Folge dünner Quellen, sondern das Gegenteil: der Mittwoch hat sechs Schwellen *entschieden*, und jede einzelne ist gegen eine Änderung ausgegangen.** **Die beiden Mittwochsspiele sind gelaufen (Bayern 2:2 Arsenal, Real Madrid 4:1 Leipzig), drei Donnerstags-Pressekonferenzen haben stattgefunden, und zum ersten Mal seit sechs Läufen habe ich zu *allen neun* Partien eine datierte Personalmeldung.** ***Zwei Lücken, die ich seit drei bzw. sieben Läufen offen führen musste, sind heute geschlossen:*** **Paderborns Personalstand und der Proxy-Zustand.** ***Fünf Korrekturen am Vortagsstand sind nötig, keine davon ändert einen Tipp*** (Neuer, Kompany, Füllkrug, Kleindiensts Ausfalldauer, der Proxy). **Die Hauptnachricht des Tages ist eine, die ich *nicht* verrechne: Joshua Kimmich fehlt wegen eines Trauerfalls, und seine Rückkehr ist offen.**

---

## Hinweis zur Quellenlage (bitte zuerst lesen)

- ***`WebFetch` ist zum elften Tag unbenutzbar.*** **Ich habe es heute erneut getestet (`www.kicker.de`), Ergebnis wie an allen Vortagen: `getaddrinfo ENOTFOUND`.** **Kein Volltextabruf möglich, zu keiner Domain.**
- **`WebSearch` funktioniert und war wieder die einzige tragende Quelle.** **Alles Folgende steht auf Suchergebnis-Zusammenfassungen und -Titeln.**
- ***KORREKTUR UND GESCHLOSSENE LÜCKE: Der Proxy-Zustand ist heute erstmals belegt, und er entlastet den Proxy.*** **Die Abfrage `curl -sS "$HTTPS_PROXY/__agentproxy/status"` ist heute durchgelaufen** (gestern und vorgestern hatte ich sie als „von der Sitzungsberechtigung abgelehnt" bzw. „nicht versucht" geführt). **Das Ergebnis: `enabled: true`, `selective: false`, `toolScoped: false`, `bundleCoversEveryHost: true`, und — entscheidend — `recentRelayFailures: []`, also *keine* kürzlichen Weiterleitungsfehler.** ***Damit ist belegt, dass der Proxy nicht die Ursache ist.*** **Die `noProxy`-Liste enthält keine meiner Leitquellen; was fehlschlägt, ist die Namensauflösung selbst.** ***Die Sperre liegt also in der Netzwerk-Richtlinie der Umgebung, nicht im Proxy und nicht an meiner Bedienung*** — **genau das Bild, das `ENOTFOUND` erwarten lässt, und es ist jetzt kein Schluss mehr, sondern eine Messung.**
- ***Was der Nutzer tun kann, wenn er Volltexte will:*** **Im Menü der Cloud-Umgebung in der Titelzeile der Sitzung → „Edit" → Network access**: entweder eine breitere Zugriffsstufe wählen oder `kicker.de`, `bundesliga.com`, `weltfussball.de` und `transfermarkt.de` unter **Allowed domains** eintragen (Häkchen „Allow package managers" gesetzt lassen). *Unter der Stufe „Limited" erscheint „Allowed domains" direkt; in älteren App-Versionen unter „Custom".* Dokumentiert unter https://code.claude.com/docs/en/cloud-environments#network-access.
- ***Qualitativer Befund des Tages: die beste Quellenlage dieser Woche, und der Grund ist der Kalender.*** **Mittwoch einer Europapokalwoche heißt: zwei abgeschlossene Spiele mit offiziellen Aufstellungen, drei Pressekonferenzen vor den Donnerstagsspielen, dazu die ersten echten Spieltags-Vorberichte für Freitag bis Sonntag.** **Erstmals in dieser Woche habe ich zu allen neun Partien eine datierte Meldung** — *Paderborn war der letzte weiße Fleck und ist heute gefüllt.* **Verworfen habe ich neun Fundstellen, darunter erneut ein Ergebnis für eine ungespielte Partie.**

---

## Die Nachrichtenlage

**Mittwochabend: die Ligaphase der Champions League hat für zwei der neun Partien dieses Spieltags etwas entschieden, und für eine dritte hat eine Pressekonferenz in Freiburg mehr geliefert als beide Spiele zusammen.**

**Erstens Bayern, und die Meldung des Tages ist keine sportliche.** ***Joshua Kimmich fehlte gegen Arsenal wegen eines Trauerfalls im engsten Familienkreis; nach `fussballnationalmannschaft.net` trauert er um seinen Vater, und der Verein hat um Respekt für die Privatsphäre der Familie gebeten.*** **Er hatte bereits am Dienstag im Abschlusstraining gefehlt, die Erklärung des Vereins folgte am Mittwochvormittag.** ***Wann er zur Mannschaft zurückkehrt, ist nach Vereinsangabe offen*** — **und damit ist auch sein Einsatz am Sonntag in Freiburg offen.** **Als Ersatz lief Tom Bischof neben Aleksandar Pavlović auf.** *Ich behandle das weiter unten ausdrücklich als Nicht-Verrechnung, und zwar aus demselben Grund wie Vieira gestern: eine offene Frage trägt keinen Tipp.*

**Das Spiel selbst endete 2:2.** **Eberechi Eze brachte Arsenal in der 25. Minute in Führung, Alphonso Davies glich in der 35. aus, Harry Kane traf in der 61. per Handelfmeter zum 2:1, und Declan Rice sorgte in der 82. Minute für den Endstand.** ***Bayern bleibt damit in der Ligaphase ungeschlagen, hat aber zu Hause zwei Punkte liegen lassen.*** ***Vincent Kompany hat gecoacht*** — **er hatte den Tag vor dem Spiel krank im Bett verbracht und Abschlusstraining wie Pressekonferenz abgesagt, war am Spieltag aber zurück.** **Bei Arsenal fehlten Saliba (Rücken) und Tzolis (Oberschenkel).**

**Zweitens Leipzig, und es ist die zweite hohe Niederlage binnen fünf Tagen.** **RB hat bei Real Madrid 1:4 verloren (0:1 zur Halbzeit).** ***Christoph Baumgartners Comeback ist der eine Lichtpunkt: er kam zurück und legte unmittelbar darauf Leipzigs Treffer für Gomis auf*** (dpa über `rhein-zeitung.de`). **Dieselbe dpa-Einordnung nennt eine lebhafte, mutige erste Halbzeit und Courtois als den Grund, aus dem daraus nichts wurde.** ***Für die Tabelle über Leipzig hinaus wichtig: RB ist damit im fünften Auswärtsspiel aller Wettbewerbe ohne Sieg.*** *Eine Reaktion von Demichelis nach dem Spiel habe ich nicht gefunden; die auffindbaren Zitate stammen von vor der Partie (Mut und Persönlichkeit, Reals Umschaltmoment sei extrem gefährlich).* **Eine Entlassung ist nicht gemeldet.**

**Drittens Freiburg, und das ist der substanzreichste Befund des Tages für meine Tipps.** ***Julian Schuster hat auf der Pressekonferenz vor Monaco eine Rotation angekündigt und dabei den Sonntag ausdrücklich zum Maßstab gemacht.*** **`sports.yahoo.com` und drei baden-württembergische Zeitungen (`zvw.de`, `badische-zeitung.de`, `stimme.de`) berichten übereinstimmend: Philipp Lienhart fehlt in Monaco, und zwar nicht verletzt, sondern wegen Belastungssteuerung; Max Rosenfelder soll ihn ersetzen.** **Schuster sagt, die Voraussetzungen seien da, frische Spieler ins Spiel zu bringen, und die Berichte nennen als Begründung, dass er am Sonntag gegen den Tabellenführer seine stärkste Elf brauche.** ***Damit ist mein Regel-3-Abschlag für Freiburg weitgehend entwertet — der Gegner meiner Partie 9 plant die Donnerstagsreise als Schonung, nicht als Belastung.*** *Eine Vorschau erwartet die „Europa-Elf", also acht gegen Leverkusen ausgesparte Spieler.*

**Viertens Hoffenheim, wo die Pressekonferenz vor Lyon stattgefunden hat, aber keine Personalie geliefert hat.** **Christian Ilzer und Fisnik Asllani haben am Mittwoch gesprochen** (`tsg-hoffenheim.de` kündigt die PK im Livestream an, `sportschau.de`/SWR und `sport1.de` berichten). **Ilzer nennt Lyon wegen der taktischen Flexibilität von Trainer Paulo Fonseca und des Umschaltspiels „extrem gefährlich" und sagt, er habe derzeit genug Baustellen.** ***Eine Rotationsankündigung ist das ausdrücklich nicht, und eine neue Verletztenmeldung enthalten die Berichte nicht.*** *Lyon kommt als Spitzenreiter der Ligue 1 — das ist ein Gegenargument zu meiner gestrigen Einschätzung, Hoffenheims Donnerstag werde „eher leichter", und ich stelle es dazu.* **Hoffenheim hat erst drei von neun Pflichtspielen gewonnen, keines in der Europa League.** *Nebenbefund ohne Tippwert: Ilzer hatte am Mittwoch Geburtstag und musste durch ein Spalier, in dem jeder Spieler einmal zuschlagen durfte.*

**Fünftens Leverkusen, wo ich die Rotationsfrage nicht beantworten konnte.** ***Eine Pressekonferenz-Aussage zur Rotation vor Kreta habe ich nicht gefunden*** — **die auffindbaren Texte sind Vorschauen, keine Trainerzitate.** **Neu und belegbar ist der Europa-League-Kader: Jonas Hofmann wurde nachnominiert, Victor Boniface steht nicht im Kader.** **Zu den Ausfällen: Terrier bis Dezember, dazu Kofane, Doué und Ben Seghir mit Muskelverletzungen, Culbreath fraglich.** ***Patrik Schick wird in der Vorschau als Mittelstürmer gesetzt geführt*** — **also weder Ausfall noch Schonung, und damit bleibt meine 1:1-Schwelle für Partie 8 unausgelöst.** *Bei OFI fehlen Marinakis, Leya Iseka und Sielis.*

**Sechstens Köln und Schalke, und hier ist die Faktenlage heute so dicht wie bei keiner anderen Partie.** ***Auf Kölner Seite ist meine 2:0-Schwelle negativ entschieden:*** **Ragnar Ache ist teilintegriert ins Training zurückgekehrt, wird aber nach `koeln.t-online.de` „gegen Schalke noch keine Option darstellen", und Imad Rondic fällt mit einer Muskelverletzung aus.** ***Dazu liegt Joël Schmieds Diagnose endlich vor: eine Sprunggelenksverletzung*** — **vier Läufe nach dem ersten Bänderverdacht.** **Rav van den Berg laboriert weiter an muskulären Problemen, Dallinga hat einen Kreuzbandriss, und Ellyes Skhiri wird nach Syndesmosebandriss erst im kommenden Jahr zurückerwartet.** **Bei Schalke ist Schallenberg definitiv weg** (*der Verein sprach am Dienstag von einer kleineren Beinverletzung und einer Trainingspause; eine genauere Diagnose hat er nicht veröffentlicht*), **Wöber hat weiter keine Diagnose, und Džeko und Sylla arbeiten individuell.** **Muslić zu Sylla: „Die Beinverletzung ist nicht so schlimm, aber ich weiß nicht, ob wir es bis Köln hinbekommen."** *Die Spieltags-Pressekonferenz der Schalker ist für Donnerstag, 22.10., 14:00 Uhr angesetzt und lag damit heute noch vor mir.*

**Siebtens Paderborn, und das ist die geschlossene Lücke, auf die ich drei Läufe gewartet habe.** ***`nw.de` (Neue Westfälische) liefert erstmals einen datierten Personalstand:*** **Oliver Batista Meier fällt mit einer Innenbandverletzung im Sprunggelenk für das Heimspiel gegen den HSV definitiv aus; Timur Gayret und Marcel Hoffmeier fehlen ebenfalls.** **Laurin Curda soll trotz eines Handbruchs spielen können.** ***Nyamekye Awortwie-Grant ist nach Knieproblemen erst ins Teiltraining zurückgekehrt*** — **und damit ist meine 1:1-Schwelle für Partie 6, die eine *belegte Rückkehr* verlangt, nicht ausgelöst.** ***Zu Tigges und Marino, den beiden Namen meiner 1:3-Schwelle, ist keine Ausfallmeldung auffindbar*** — **beide gelten als verfügbar.**

**Achtens Werder, wo eine Nichtmeldung heute zu einer Meldung geworden ist.** ***Niclas Füllkrug hat die erste Einheit der Mainz-Woche ausgelassen — aber der Verein nennt ausdrücklich Belastungssteuerung und keine Verletzung*** (`deichstube.de`, `weser-kurier.de`). **Deman, Grüll und Arthur wurden von Thioune ebenso geschont, und alle vier haben die Belastungsarbeit mitgemacht.** ***Damit ist meine 2:0-Schwelle für Partie 5 nicht offen, sondern negativ beantwortet.*** **Füllkrug hat nach einer Wett-Vorschau in jedem seiner letzten fünf Bundesligaspiele getroffen und steht bei sieben Pflichtspieltoren; Werder ist seit fünf Spielen unbesiegt.** ***Bei Keke Topp ist aus der undatierten Meldung von gestern eine Diagnose geworden: Kreuzbandriss*** — **genau der Fall, für den meine Schwelle „bleibe bei 1:1 und gehe nicht höher" vorgesehen war.** **Weiter aus: Stage (Oberschenkel), Agu (Wade), Musah (Muskel), Alvero (Wade), N'Diaye (Leiste); Njinmah ist im Teiltraining, Comeback für November angestrebt, Piepers MRT war ohne Befund.**

**Neuntens Gladbach, wo die Lage unverändert schlecht ist und eine Diagnose weiter fehlt.** **Blessin hat Kleindiensts erneuten Muskelfaserriss an anderer Stelle bestätigt und dem 31-Jährigen mehrere Wochen Ausfall in Aussicht gestellt** — ***ohne genauen Zeitrahmen, und das ist eine Korrektur an meinem Vortagsstand.*** **Nicolas Kühn hat nach `bmg-news.de` nahezu die komplette Woche mit der Mannschaft trainiert, und der Verein muss abwägen, ob es für den Spieltag reicht.** ***Isac Lidbergs Diagnose fehlt den dritten Tag:*** **er musste gegen Hoffenheim ausgewechselt werden und griff sich an den Oberschenkel; ob Schlag oder Verletzung, ist offen.** **Leszczyński und Leopold fehlen weiter.** **Der Verein steht nach sechs Spielen bei 0 Punkten und 8:20 Toren.**

**Zehntens Dortmund und Frankfurt, mit einer unangenehmen Selbstkorrektur.** ***Karetsas' Ausfall ist jetzt mit Vereinszitat belegt:*** **Geschäftsführer Lars Ricken sagt, „Kos hat eine Bandverletzung im Fuß. Er wird nicht nach Baku mitfliegen und auch gegen Frankfurt am Samstag nicht spielen können"** (`bundesliga.com`, `sport.sky.de`); **die Verletzung stammt aus dem 0:0 bei Union, und `neunzigplus.de` nennt mehrere Wochen Ausfall.** ***Und hier muss ich meine gestrige Verwerfung revidieren:*** **die Ausfallliste mit Emre Can (Kreuzbandriss), Giannis Konstantelias (Kreuzbandriss am 1. Spieltag) und Justin Lerma (Muskelverletzung), die ich gestern als undatiert nicht verwendet habe, wird heute von einem zweiten, unabhängigen Vorbericht getragen.** *Zu Mussa Kaba widersprechen sich die Quellen (ausgekugelte Schulter bzw. Knieprobleme) — den lasse ich offen.* **Bei Frankfurt ist die Lage entspannter: Ngankam fehlt mit Oberschenkelverletzung, Pimpong und Maluze sind fraglich, gesperrt ist niemand, und Onyedika steht bei vier Gelben Karten.** ***Adi Hütter als Frankfurter Trainer ist heute zum zweiten Mal unabhängig bestätigt*** (erwartetes 4-2-3-1).

---

### Die Europapokalwoche vor dem 7. Spieltag

**Vier Spiele sind gelaufen, drei stehen am Donnerstag aus.**

| Tag | Partie | Wettbewerb | Lage | Ergebnis | Bundesligaspiel danach |
|---|---|---|---|---|---|
| **Di 20.10., 18:45** | Sabah FK – **Borussia Dortmund** | Champions League | **auswärts, Baku, sehr weit** | ***1:2*** (Guirassy 10., 53.) | Sa 18:30 **heim** (4 Tage) |
| **Di 20.10., 21:00** | **VfB Stuttgart** – Atlético Madrid | Champions League | heim, MHP Arena | ***1:1*** (Leweling 36.) | **Fr 20:30 heim (3 Tage)** |
| **Mi 21.10., 21:00** | **FC Bayern** – FC Arsenal | Champions League | heim | ***2:2*** (Davies 35., Kane 61. FE) | So 17:30 **auswärts** (4 Tage) |
| **Mi 21.10., 21:00** | Real Madrid – **RB Leipzig** | Champions League | **auswärts, Madrid, weit** | ***4:1*** (Gomis für RB) | **Sa 15:30 heim (3 Tage)** |
| **Do 22.10., 18:45** | OFI Kreta – **Bayer Leverkusen** | Europa League | **auswärts, Kreta, sehr weit** | offen | **So 15:30 auswärts (3 Tage)** |
| **Do 22.10., 21:00** | **TSG Hoffenheim** – Olympique Lyon | Europa League | **heim, SNP Arena** | offen | **So 15:30 heim (3 Tage)** |
| **Do 22.10., 21:00** | AS Monaco – **SC Freiburg** | Conference League | **auswärts, mittel — Rotation angekündigt** | offen | So 17:30 **heim** (3 Tage) |

***Die wichtigste Zeile ist die letzte:*** **Freiburgs Donnerstag ist seit heute belegt als Schonungstermin geplant, nicht als Belastung.**

---

## Abrechnung des 6. Spieltags

**Unverändert: vier von neun Tendenzen richtig, kein Endstand exakt.** *Die vollständige Tabelle steht im Archiv unter `archiv/2026-10-18.md`.* **Die drei Lehren daraus — Torflaute vor Tabellenplatz, keine Umrechnung fremder Ausfälle in eigene Tore, Tabellenletzter nach Personallage — sind in den vier Regeln unten verarbeitet.**

---

## Korrekturen und geschlossene Lücken

***Heute sind fünf Korrekturen am Vortagsstand nötig. Keine davon ändert einen Tipp — aber zwei davon hätten es gestern beinahe getan, in die falsche Richtung.***

1. ***KORREKTUR: Manuel Neuer ist zurück, nicht länger weg.*** **Mein Vortagsstand führte Eberls Aussage, Neuer fehle „womöglich länger", und Urbig als Vertreter.** **Richtig ist: Neuer ist am Montag ins Mannschaftstraining zurückgekehrt und stand gegen Arsenal wieder im Tor.** ***Die Richtung meines Vortagsstands war damit falsch*** — *ich hatte eine Verschlechterung notiert, wo eine Rückkehr lief.* **Tippwirkung: keine, weil ich den Torwartwechsel nie in Partie 9 verrechnet hatte.**
2. ***KORREKTUR UND GESCHLOSSENE LÜCKE: Kompany steht an der Linie.*** **Gestern führte ich „Kompanys Einsatzfähigkeit ist offen" als echte Lücke und schrieb, ob er am Sonntag in Freiburg coacht, sei unbelegt.** **Heute hat er gegen Arsenal gecoacht, nach einem Tag krank im Bett.** ***Meine Schwelle „wird belegt, dass Kompany auch am Sonntag nicht an der Linie steht, gehe ich auf 1:1" ist damit negativ entschieden und erledigt*** — **nicht ausgelöst.**
3. ***KORREKTUR UND GESCHLOSSENE LÜCKE: Der Proxy ist nicht die Ursache.*** **Gestern stand hier „der Proxy-Zustand bleibt unbelegt (Statusabfrage von der Sitzungsberechtigung abgelehnt)".** **Heute ist die Abfrage durchgelaufen und meldet `recentRelayFailures: []` sowie `selective: false`.** ***Die Sperre liegt in der Netzwerk-Richtlinie der Umgebung.*** *Das ändert für den Nutzer die Abhilfe nicht, aber es nimmt eine falsche Verdachtsrichtung aus dem Bericht.*
4. ***PRÄZISIERT, GEGEN MEINEN VORTAGSSTAND: Kleindiensts Ausfalldauer ist nicht „etwa zwei weitere Spiele".*** **Gestern habe ich diese Blessin-Angabe geführt und die Spannung zu Quellen ohne Dauer gekennzeichnet.** **Heute ist die Lage eindeutiger: Blessin spricht von mehreren Wochen Ausfall und nennt ausdrücklich keinen genauen Zeitrahmen.** ***Ich streiche die „zwei Spiele" und führe „mehrere Wochen, ohne Datum".***
5. ***KORREKTUR EINER VERWERFUNG: Dortmunds Ausfallliste war richtig.*** **Gestern habe ich die `ligainsider`-Liste mit Emre Can (Kreuzbandriss), Konstantelias und Lerma als „undatiert und nicht gegengeprüft" nicht verwendet.** **Heute trägt ein zweiter, unabhängiger Vorbericht dieselben Namen, Konstantelias mit Kreuzbandriss seit dem 1. Spieltag.** ***Die Verwerfung von gestern war zu streng.*** *Ein Vereinszitat fehlt weiter, deshalb führe ich sie als gegenbestätigt, nicht als vereinsbelegt.* **Tippwirkung: keine — Can ist Mittelfeldspieler, und meine Dortmunder Schwelle zielt auf Innenverteidiger.**
6. ***GESCHLOSSEN: Paderborns Personalstand liegt erstmals vor.*** **Drei Läufe ohne Fortschritt sind beendet** (Batista Meier Innenbandverletzung im Sprunggelenk und definitiv aus, Gayret und Hoffmeier aus, Curda spielt trotz Handbruchs, Awortwie-Grant nur im Teiltraining).
7. ***GESCHLOSSEN UND NEGATIV: Füllkrug ist nicht verletzt.*** **Gestern war das eine „entscheidende Nichtmeldung", zum zweiten Tag.** **Heute ist es eine Meldung: Fehlen in der ersten Einheit, Grund Belastungssteuerung, keine Verletzung, Belastungsarbeit mitgemacht.** ***Meine 2:0-Schwelle ist beantwortet, nicht offen.***
8. ***GESCHLOSSEN: Joël Schmieds Diagnose ist eine Sprunggelenksverletzung.*** *Vier Läufe nach dem ersten Bänderverdacht vom 16.10.*
9. ***GESCHLOSSEN UND NEGATIV: Ache ist gegen Schalke keine Option.*** **Gestern führte ich „teilintegriert ins Mannschaftstraining" und eine 2:0-Schwelle über seine Rückkehr.** **Heute steht ausdrücklich, dass er gegen Schalke noch keine Option darstellt.** ***Die Schwelle ist erledigt.***
10. ***GESCHLOSSEN: Keke Topps Diagnose ist ein Kreuzbandriss.*** **Gestern undatiert und mit verwirrter Vereinszuordnung, heute als Werder-Ausfall geführt.** ***Meine Schwelle sah für genau diesen Fall vor, bei 1:1 zu bleiben*** — **Regel 2, und sie greift.**
11. ***GESCHLOSSEN: Claude-Maurices Status ist datiert.*** **Gestern „widersprüchlich", heute: Oberschenkel, teilintegriertes Mannschaftstraining, Einsatz gegen Union nach `Augsburger Allgemeine` unwahrscheinlich.**
12. ***GESCHLOSSEN: Vuskovics Sperre hat ein Enddatum*** (bis 15. November). *Gestern nur „Dopingsperre".*
13. ***GESCHLOSSEN: Die Tabelle ist heute wieder unabhängig gegenbestätigt*** (`de.wikipedia.org` und `bundesliga.com`: Bayern 6/22:5/+17/14, Dortmund 6/11:4/+7/14, Gladbach 6/0 Punkte/8:20, Platz 18). *Gestern musste ich sie als bloße Fortschreibung kennzeichnen.*

---

## Tabelle nach dem 6. Spieltag

***Heute wieder unabhängig gegenbestätigt*** *(`de.wikipedia.org`, `bundesliga.com`; die `kicker`-Tabellenseite und die `sportschau`-Blitztabelle zeigten ältere Stände mit 4 bzw. 5 Spielen und wurden nicht verwendet).* **Es ist seit dem 18.10. kein Bundesligaspiel gelaufen, es gibt also nichts zu verschieben.**

| # | Verein | Sp | Tore | Diff | Pkt | Form (1.–6. ST) | Europapokal diese Woche |
|---|---|---|---|---|---|---|---|
| 1 | FC Bayern München | 6 | 22:5 | +17 | 14 | S U S S U S | **Mi, CL, heim — 2:2** |
| 2 | Borussia Dortmund | 6 | 11:4 | +7 | 14 | S S S S U U | **Di, CL, auswärts — 2:1 gewonnen** |
| 3 | SC Freiburg | 6 | 15:6 | +9 | 13 | S S S U S N | **Do, ECL, auswärts (Monaco) — Rotation** |
| 4 | Bayer 04 Leverkusen | 6 | 16:9 | +7 | 13 | N S U S S S | **Do, EL, auswärts (Kreta)** |
| 5 | 1. FSV Mainz 05 | 6 | 14:10 | +4 | 10 | U S N S N S | — |
| 6 | SV 07 Elversberg | 6 | 12:11 | +1 | 10 | S S N U N S | — |
| 7 | RB Leipzig | 6 | 16:11 | +5 | 9 | S N S N S N | **Mi, CL, auswärts — 1:4** |
| 8 | SV Werder Bremen | 6 | 12:12 | 0 | 9 | N S U S U U | — |
| 9 | Hamburger SV | 6 | 6:15 | −9 | 9 | N N N S S S | — |
| 10 | FC Augsburg | 6 | 16:12 | +4 | 8 | S S U N U N | — |
| 11 | Eintracht Frankfurt | 6 | 10:16 | −6 | 8 | U N S U N S | — |
| 12 | 1. FC Köln | 6 | 8:11 | −3 | 7 | S N U N S N | — |
| 13 | VfB Stuttgart | 6 | 8:10 | −2 | 6 | N S N N S N | **Di, CL, heim — 1:1** |
| 14 | TSG Hoffenheim | 6 | 11:14 | −3 | 6 | N N S N N S | **Do, EL, heim (Lyon)** |
| 15 | FC Schalke 04 | 6 | 5:7 | −2 | 5 | N U S U N N | — |
| 16 | SC Paderborn 07 | 6 | 5:9 | −4 | 5 | U N N S N U | — |
| 17 | 1. FC Union Berlin | 6 | 5:17 | −12 | 5 | U N N N S U | — |
| 18 | Bor. Mönchengladbach | 6 | 8:20 | −12 | 0 | N N N N N N | — |

---

## Heute geprüft und verworfen

***Neun Fundstellen verworfen. Die erste ist zum zweiten Tag in Folge ein Ergebnis für eine ungespielte Partie — diesmal mit vertauschtem Heimrecht.***

1. ***Eine `ligainsider`-Seite, die „Hamburger SV 0:0 SC Paderborn 07" als Ergebnis führt.*** **Verworfen aus zwei unabhängigen Gründen:** *die Partie findet erst am Samstag statt, und sie findet in Paderborn statt, nicht in Hamburg — das Heimrecht ist vertauscht.* ***Dass mir das zwei Tage hintereinander passiert, ist der Grund, aus dem ich jede Ergebnisangabe gegen den Spielplan prüfe, bevor ich sie anfasse.***
2. **Die `sport1`-Anstoßzeiten für diesen Spieltag: 18:30 für Stuttgart – Gladbach, 14:30 für Hoffenheim – Leverkusen, 16:30 für Freiburg – Bayern.** **Verworfen:** *`datencenter.dfb.de`, `ruhrnachrichten.de` und `anstosszeiten.de` nennen übereinstimmend 20:30, 15:30 und 17:30.* **Drei übereinstimmende Quellen gegen eine abweichende.**
3. ***Eine Suchzusammenfassung, nach der Leipzigs Spiel bei Real Madrid „noch bevorsteht".*** **Verworfen:** *das Spiel ist gelaufen und 1:4 ausgegangen, belegt durch `realtotal.de`, `fussballnationalmannschaft.net` und die dpa-Einordnung über `rhein-zeitung.de`.* **Die Zusammenfassung stützte sich erkennbar auf Vorberichte vom 19./20.10.**
4. **Zwei Liveticker-Zwischenstände: eine DAZN-Seite mit 2:1 für Bayern – Arsenal und eine Seite mit 3:0 für Real – Leipzig.** **Verworfen:** *beides sind Zwischenstände; die Endstände 2:2 und 4:1 sind jeweils von mehreren Quellen gedeckt.*
5. ***Die Startelf-Angaben zum Spiel in Madrid.*** **Nicht verwendet:** *die auffindbaren Listen nennen für Real unter anderem Bernardo Silva und Cucurella, für Leipzig unter anderem Nkunku — die Zusammenfassung weist selbst auf Widersprüche hin.* ***Ich übernehme aus diesem Spiel nur, was mehrfach gedeckt ist: das Ergebnis, Baumgartners Einwechslung und seine Vorlage zum Treffer von Gomis.***
6. **Die Unioner Ausfallliste, zum dritten Tag in Folge.** **Eine `comunio`-Vorschau nennt Nsoki (Wade), Markgraf (Kreuzbandriss) und Ilić („Aufbautraining nach Blinddarm-OP"), dazu Juranović, Burcu und Burke als fraglich.** **Verworfen:** *die Liste enthält erkennbar Spieler der Vorsaison, und die Ilić-Angabe widerspricht direkt der von gestern („Lebensmittelvergiftung").* ***Dass derselbe Spieler in zwei Tagen zwei verschiedene undatierte Diagnosen bekommt, ist für mich der Beweis, dass dieser Bestand nicht tragfähig ist.***
7. ***Der Elversberger Trainername.*** **Eine `comunio`-Seite nennt „Wagner".** **Nicht verwendet:** *Einzelquelle aus einer Aufstellungsdatenbank, und ich habe gestern bei Augsburg gelernt, was solche Stammdatenfelder wert sind (Manuel Baum, sechs Jahre veraltet).* ***Zusätzlich misstrauisch macht mich, dass „Wagner" auch der Name ist, den ich für Köln führe*** — **eine Verwechslung ist nicht auszuschließen.** **Ich schreibe deshalb zu Partie 4 keinen Elversberger Trainernamen hin.**
8. **Hoeneß-Rotationszitate.** **Die auffindbaren Treffer betreffen eine Pressekonferenz vor einem Bratislava-Spiel („neun Pflichtspiele in vier Wochen") und sind rund zwölf Tage alt; ein weiterer Text beschreibt eine Rückreise aus Rom vor einem Gladbach-Spiel und stammt erkennbar aus einer früheren Saison.** **Verworfen als Grundlage für diese Woche:** ***eine Rotationsankündigung vor diesem Freitag habe ich nicht gefunden, und ich löse die Schwelle nicht auf einem alten Zitat aus.***
9. **Zwei `vfb.de`-Pressekonferenzseiten zu „Hoeneß vor Gladbach".** **Verworfen:** *die URLs tragen die Saisonkürzel 2425 und 2526, betreffen also frühere Spielzeiten.*

---

## Offen benannte Restlücken

**Der 7. Spieltag beginnt in zwei Tagen. Ich trenne weiter, was fehlt, von dem, was fehlen *muss*.**

***Strukturell noch nicht verfügbar (kein Mangel meiner Recherche):***
- **Keine Spieltags-Pressekonferenz zu einer der neun Partien.** *Die erste ist Schalkes am Donnerstag, 22.10., 14:00 Uhr, die Stuttgarter vor dem Freitagsspiel folgt voraussichtlich ebenfalls Donnerstag.* ***Die drei Pressekonferenzen von heute (Hoffenheim, Freiburg, und die ausgefallene Leverkusener) galten den Donnerstagsspielen*** — **bei Freiburg hat eine davon trotzdem für den Sonntag geliefert.**
- **Kein Kaderaufgebot und keine Aufstellung zum 7. Spieltag.** ***Das bleibt der Grund, aus dem neun von neun Tipps stehen.***

***Echte Lücken:***
- ***Kimmichs Verfügbarkeit für Sonntag ist offen*** *(Trauerfall im engsten Familienkreis, Rückkehr nach Vereinsangabe ohne Datum).* **Das ist meine wichtigste neue Lücke und die einzige, die einen Tipp bewegen könnte.**
- ***Lidbergs Diagnose fehlt den dritten Tag*** *(Auswechslung gegen Hoffenheim, Griff an den Oberschenkel, Schlag oder Verletzung offen).* **Kühns Einsatz hängt am Kaderaufgebot vom Freitag; „nahezu die komplette Woche mittrainiert" ist noch keines.**
- ***Wöbers Diagnose fehlt den zweiten Tag*** *(Trainingsabbruch am Dienstag, keine Vereinsdiagnose, keine Einsatzentscheidung).* **Džekos und Syllas Status bleiben offen.**
- ***Vieiras Status beim HSV ist den zweiten Tag offen*** — *heute präzisiert in der Richtung: die Berichte deuten auf die hintere Oberschenkelmuskulatur, eine abschließende Einschätzung fehlt.* **Das bleibt das Gegenargument zu meiner Änderung von gestern.**
- **Eine datierte Unioner Ausfallliste fehlt weiterhin** — ***siebter Lauf in Folge und meine am längsten offene echte Lücke.***
- **Zu Mainz habe ich auch heute keinen aktuellen Personalstand gefunden** *(Zentner, Kohr, Silas stehen nur in undatierten Listen; Kohrs Ausfall bis Anfang Januar ist der belegte Stand der Vortage).*
- ***Luis Díaz' Status ist widersprüchlich.*** **Ein `ran`-Artikel titelt „Darum fehlt Luis Diaz" und nennt eine Verletzung aus dem Leipzig-Spiel; eine Vorschau desselben Abends führt ihn auf Linksaußen in der Startelf.** *Ich verrechne ihn nicht und nenne es, weil es Partie 9 betreffen kann.*
- **Der Elversberger Trainername bleibt eine Lücke** *(siehe Verworfenes 7).* **Kölns Trainername ruht weiter auf der Prüfung vom 19.10. (René Wagner); heute kein neuer Beleg und kein gegenteiliger.**
- **Eine Leverkusener Rotationsankündigung fehlt** *(Pressekonferenz vor Kreta nicht in Textform auffindbar).* **Eine Demichelis-Reaktion nach dem 1:4 fehlt ebenfalls.**
- **Keine belastbare Gelbsperren-Übersicht nach dem 6. Spieltag.** *Einziger Teilbefund: Onyedika (Frankfurt) steht bei vier Gelben Karten.*
- **Keine Transfermeldung mit Spielrelevanz für den 7. Spieltag.**
- ***Direkte Vergleiche: heute der erste Teilbefund in acht Läufen*** — **eine Vorschau nennt, dass Hütter als Frankfurter Trainer nur zwei von sechs Spielen gegen den BVB verloren hat.** *Das steht in einem Vorberichtstext, nicht in einer Statistikquelle, und ich verrechne es nicht; ich halte es fest, weil es die erste Historienangabe ist, die ich überhaupt gefunden habe.* **Zu den übrigen acht Partien bleibt die Lücke bestehen.**
- **Zu Mussa Kaba (Dortmund) widersprechen sich die Angaben** *(ausgekugelte Schulter bzw. Knieprobleme).*

---

## Die Tipps zum 7. Spieltag

**Der Vortagsstand betraf denselben Spieltag, also ist jede Partie vergleichbar.** ***Kein Tipp ändert sich, alle neun bleiben*** — **aber sechs Schwellen sind heute entschieden worden, und das ist der Unterschied zu einem Lauf, in dem nichts passiert.**

**Die vier Regeln, nach denen ich diesen Spieltag angelegt habe** — *unverändert:*

1. **Eine Torflaute wiegt schwerer als ein guter Tabellenplatz.**
2. **Ausfälle beim Gegner senken dessen Tore, sie erhöhen nicht automatisch meine.**
3. **Drei Tage nach einem weiten Auswärtsspiel in Europa gebe ich einen halben Tor-Abschlag**, bei einem Heimspiel in Europa keinen. ***Heute erstmals mit einer Ausnahme: wer die Europapartie belegt als Schonungstermin plant, bekommt keinen Abschlag.***
4. **Aufsteiger *und* den punktlosen Tabellenletzten tippe ich nach Spielweise und Personallage, nicht nach Tabellenplatz oder Heimrecht.**

**Für jede Partie nenne ich außerdem die Schwelle: die konkrete Information, die den Tipp bis zum Anpfiff ändern würde.**

---

### 1. VfB Stuttgart – Borussia Mönchengladbach
**Freitag, 23.10.2026, 20:30 Uhr, MHP Arena**
**Tipp: 2:0**
***unverändert***

**Beide Schwellen dieser Partie sind heute geprüft und keine ausgelöst.**

***Erstens Kühn, und er ist näher dran als gestern, aber nicht da.*** **`bmg-news.de` berichtet, er habe nahezu die komplette Woche mit der Mannschaft trainiert, und der Verein müsse abwägen, ob es für den Spieltag reicht.** **Meine Schwelle verlangt wörtlich ein Kaderaufgebot oder eine Startelf, *nicht* eine Prognose.** ***Eine Abwägung des Vereins ist keine Nominierung*** — *und diese Regel hat mich in diesem Spieltag schon zweimal vor einem Fehler bewahrt (Al-Dakhil am 20.10., Baumgartner am 19.10.).* **Das Kaderaufgebot kommt am Freitag.**

***Zweitens Hoeneß' Rotation: keine Fundstelle für diese Woche.*** **Die auffindbaren Rotationszitate sind rund zwölf Tage alt und betreffen ein anderes Spiel (siehe Verworfenes 8).** **Ich löse die Schwelle nicht auf einem alten Zitat aus.** *Die Stuttgarter Spieltags-Pressekonferenz liegt voraussichtlich am Donnerstag und ist damit der nächste prüfbare Punkt.*

***Drittens die Stuttgarter Innenverteidigung: kein neuer Ausfall aus dem Atlético-Spiel gemeldet.*** **Der Stand vom 20.10. gilt — Chabot und Hendriks haben gespielt, Jeltsch saß als vierte Option auf der Bank, Mittelstädt war zurück in der Startelf, Al-Dakhil fehlte im Kader (Knie) und Zagadou weiter.**

***Was für den Tipp spricht, ist unverändert und heute präziser:*** **Gladbach steht bei 0 Punkten und 8:20 Toren, Leszczyński und Leopold fehlen sicher, Kleindienst fällt mit erneutem Muskelfaserriss mehrere Wochen aus, und Lidbergs Einsatz ist nach seiner Auswechslung gegen Hoffenheim offen.** ***Dass Blessin für Kleindienst heute keinen Zeitrahmen nennt, verschärft die Lage gegenüber meinem Vortagsstand*** — *ich hatte dort noch „etwa zwei weitere Spiele" geführt.*

***Was gegen Stuttgart spricht, bleibt die kürzeste Pause des Spieltags:*** **90 intensive Minuten am Dienstagabend, davon 30 in Überzahl, und am Freitag um 20:30 wieder Anpfiff.** **Kein Abschlag nach Regel 3, weil es ein Heimspiel ohne Reise war.** *Dass Stuttgart in Überzahl gegen Atlético keinen Sieg geholt hat, passt zu 8 Toren in sechs Bundesligaspielen — der Grund, aus dem ich nicht höher tippe.*

***Schwelle:*** *Wird Kühns **oder** Kleindiensts Einsatz belegt (Kaderaufgebot oder Startelf, **nicht** Prognose), gehe ich auf **2:1**. Kündigt Hoeneß auf der Spieltags-Pressekonferenz belegt eine Rotation an **oder** wird ein Stuttgarter Innenverteidiger-Ausfall gemeldet, gehe ich auf **1:1**. **Wird Lidbergs Ausfall bestätigt, bleibe ich bei 2:0 und gehe nicht höher — Regel 2.***

---

### 2. FC Augsburg – 1. FC Union Berlin
**Samstag, 24.10.2026, 15:30 Uhr, WWK Arena**
**Tipp: 2:1**
***unverändert — und zum siebten Lauf die Partie mit der schlechtesten Quellenlage***

***Auf Augsburger Seite ist heute eine Lücke geschlossen, auf Unioner Seite ist sie zum siebten Mal offen.***

**Geschlossen: Alexis Claude-Maurice.** **Nach `Augsburger Allgemeine` (über `rotowire.com`) ist er mit einer Oberschenkelverletzung ins teilintegrierte Mannschaftstraining zurückgekehrt, ein Einsatz gegen Union gilt aber als unwahrscheinlich.** ***Das ist eine datierte Angabe und beendet den Widerspruch von gestern.*** ***Meine 1:1-Schwelle löst sie trotzdem nicht aus***, **weil die Schwelle eine *genannte Ersatzlösung* verlangt — und die steht in keiner Quelle.** *Weiter aus: Banks (Außenbandverletzung im rechten Knie, Vereinsmeldung vom 4.10.), Mounié und Breithaupt.* ***Einen Augsburger Trainernamen schreibe ich weiter nicht hin*** — *der einzige auffindbare Treffer nannte Manuel Baum und war sechs Jahre veraltet.*

***Offen, und heute mit einem neuen Argument für meine Zurückhaltung:*** **die auffindbare Unioner Liste nennt Ilić im „Aufbautraining nach Blinddarm-OP".** **Gestern nannte eine andere undatierte Liste bei demselben Spieler eine Lebensmittelvergiftung.** ***Zwei undatierte Quellen, zwei unvereinbare Diagnosen, derselbe Spieler, zwei Tage Abstand*** — **das ist kein Informationsmangel mehr, das ist ein Beleg dafür, dass dieser Datenbestand nicht tragfähig ist.** **Meine 2:0-Schwelle zielt genau auf einen Unioner Offensivausfall, und ich löse sie weiter nicht aus.** *Dieselbe Liste enthält erkennbar Spieler der Vorsaison.* **Markgraf (Kreuzbandriss) ist der einzige Name, der über mehrere Läufe stabil bleibt; Nsoki soll wieder im Training mitmischen.**

**Was den Tipp trägt, ist unverändert die Tordifferenz:** **Union hat mit 5 Toren in 6 Spielen die zweitschwächste Offensive und mit 17 Gegentoren die schwächste Abwehr der Liga.** **Augsburg ist zu Hause und hat mit 16 Toren die vierbeste Offensive, kassiert aber zuverlässig** — *das 3:4 in Elversberg nach 0:3-Führung bleibt die klarste Aussage über diese Mannschaft.* **Keine der beiden Mannschaften spielt international** — *der einzige Spieltagspunkt, bei dem das für beide Seiten gilt, und damit die einzige Partie ohne jeden Belastungsfaktor.* **Der Punkt für Union bleibt das 0:0 gegen Dortmund.**

***Schwelle:*** *Wird ein Augsburger Offensivausfall **mit genannter Ersatzlösung** gemeldet, gehe ich auf **1:1**. Wird Unions Null-zu-null-Formation gegen Dortmund in einem Vorbericht als Linie für Augsburg bestätigt (Tiefbau, fünf Verteidiger), gehe ich auf **1:0**. **Taucht eine datierte Unioner Ausfallliste mit Ilić oder Latte Lath auf, gehe ich auf **2:0**.***

---

### 3. 1. FC Köln – FC Schalke 04
**Samstag, 24.10.2026, 15:30 Uhr, RheinEnergieSTADION**
**Tipp: 1:0**
***unverändert — und heute ist beide Schwellen zur Ruhe gekommen***

***Das ist die Partie mit der dichtesten Faktenlage des Tages, und sie bestätigt genau den Tipp, den ich seit vier Läufen führe: ein Spiel zweier Mannschaften ohne gesunden Mittelstürmer.***

***Meine 2:0-Schwelle ist negativ entschieden, und zwar auf beiden Namen.*** **Ragnar Ache ist teilintegriert ins Training zurück, wird aber nach `koeln.t-online.de` „gegen Schalke noch keine Option darstellen".** **Imad Rondic fällt mit einer Muskelverletzung aus.** ***Meine Schwelle verlangte eine belegte Rückkehr für diesen Spieltag — stattdessen ist das Gegenteil belegt.*** **Dazu Dallinga (Kreuzbandriss) und Skhiri, der nach Syndesmosebandriss erst im kommenden Jahr zurückerwartet wird.** **Vorn sollen weiter Waldschmidt und Bülter spielen; Köln hat in Frankfurt nicht getroffen.**

***Meine 1:1-Schwelle ist ebenfalls nicht ausgelöst, und hier liegt die Entscheidung dichter.*** **Sie lautete: Syllas Einsatz belegt **oder** ein weiterer Kölner Innenverteidiger-Ausfall über Schmied hinaus.** **Syllas Einsatz ist nicht belegt, sondern offen — Muslić: „Die Beinverletzung ist nicht so schlimm, aber ich weiß nicht, ob wir es bis Köln hinbekommen."** ***Und bei den Kölner Innenverteidigern ist heute eine Diagnose dazugekommen, aber kein Spieler:*** **Schmieds Verletzung ist als Sprunggelenksverletzung präzisiert, van den Bergs muskuläre Probleme standen schon gestern im Bericht.** **Ein *weiterer* Ausfall ist das nicht.**

**Bei Schalke bleibt die Lage schlecht und unverändert offen:** **Schallenberg definitiv aus** (*Vereinsmitteilung vom Dienstag: kleinere Beinverletzung, Trainingspause, keine genauere Diagnose veröffentlicht*), **Wöber ohne Diagnose und ohne Einsatzentscheidung, Džeko und Sylla im Individualtraining, Ljubičić dämpft die eigene Hoffnung auf ein Comeback beim Ex-Klub.**

***Und damit wende ich Regel 2 zum dritten Lauf in Folge gegen meine eigene Versuchung an:*** **mein Tipp lautet 1:0, Schalke steht darin schon bei null Toren.** **Weitere Schalker Ausfälle können diesen Wert nicht senken, und Kölner Tore erzeugen sie nicht.** *Genau dieser Fehler hat mich am 15.10. bei Frankfurt – Köln zwei Tore gekostet.* **Dass Schalke zu Hause noch ohne eigenes Tor ist, bleibt ein Heimbefund, und hier wird auswärts gespielt** — *das schwächt mein Argument, und ich schreibe es weiter hin.* **Die Schalker Spieltags-Pressekonferenz am Donnerstag, 14:00 Uhr, ist der nächste prüfbare Punkt.**

***Schwelle:*** *Wird Syllas **oder** Wöbers Einsatz belegt (Kaderaufgebot), gehe ich auf **1:1**. Fällt über Schmied und van den Berg hinaus ein weiterer Kölner Innenverteidiger aus, ebenfalls **1:1**. **Wird Aches Nominierung doch noch belegt, gehe ich auf **2:0**. Džekos und Schallenbergs Ausfälle ändern nach Regel 2 nichts.***

---

### 4. RB Leipzig – SV 07 Elversberg
**Samstag, 24.10.2026, 15:30 Uhr, Red Bull Arena**
**Tipp: 2:1**
***unverändert — und der Tipp, bei dem ich mir weiter am wenigsten sicher bin***

***Leipzig hat am Mittwoch 1:4 in Madrid verloren, und ich ändere den Tipp trotzdem nicht. Der Grund steht in meiner eigenen Schwellenformulierung, und ich lege ihn offen.***

**Meine Schwelle lautete: Entlassung oder Freistellung von Demichelis → 1:1; belegte Rotationsankündigung nach Madrid oder ein vom Verein gemeldeter Leipziger Offensivausfall mit genannter Ersatzlösung → ebenfalls 1:1.** ***Keiner dieser drei Fälle ist eingetreten.*** **Demichelis ist im Amt, eine Entscheidung ist nicht gemeldet, und eine Reaktion von ihm nach dem Spiel habe ich nicht gefunden.** *Die auffindbaren Zitate stammen von vor der Partie. Der Druck ist unverändert hoch: nach dem 1:6 gegen Bayern gab es scharfe Kritik aus der Klubführung, und ein Bericht nennt die Elversberg-Partie ausdrücklich als eine der Aufgaben, bei denen Siege nötig seien.* ***Zu den Namen in der Leipziger Führung widersprechen sich die Quellen*** (ein Text nennt einen Sportgeschäftsführer, ein anderer einen Sportchef, mit verschiedenen Namen) — **ich schreibe deshalb keinen hin.**

***Ein hohes Auswärtsergebnis im Bernabéu ist für mich kein Änderungsgrund, und das ist eine Entscheidung, die ich begründen muss.*** **Real Madrid ist nicht der Maßstab, an dem sich ein Heimspiel gegen einen Aufsteiger messen lässt.** **Was ich dagegen verrechne, ist die Belastung, und sie ist die zweitschwerste des Spieltags: Mittwoch 21:00 in Madrid, Samstag 15:30 in Leipzig — drei Tage nach einer weiten Auswärtsreise, also voller Abschlag nach Regel 3.** ***Der Abschlag war gestern schon drin und bleibt drin.*** *Der Befund „im fünften Auswärtsspiel aller Wettbewerbe ohne Sieg" betrifft Auswärtsspiele; dieses ist ein Heimspiel.*

***Positiv und belegt: Baumgartner ist zurück und war sofort wirksam*** — **Einwechslung in Madrid, unmittelbar darauf die Vorlage zum Treffer von Gomis.** **`rb-fans.de` führt im Vorbericht keine Sperren und keine neuen Verletzten.** *Eine `comunio`-Vorschau nennt Guiu (Muskelverletzung) und Ouédraogo (Schulter) als Ausfälle; Ouédraogo deckt sich mit meinem Stand, Guiu ist undatiert und löst die Schwelle nicht aus, weil es keine Vereinsmeldung mit Ersatzlösung ist.*

***Zu Elversberg bleibt der Stand von gestern im Kern bestehen und wird heute breiter:*** **Seifert (Syndesmose seit Juni) und Zimmerschied (Bänderverletzung im Sprunggelenk) fehlen, Onyeka ist angeschlagen und verpasst nach dem Stand von gestern Leipzig und Mainz, dazu werden Campbell, Gyamerah, Keidel und Darvich als angeschlagen geführt.** ***Meine 3:1-Schwelle verlangt einen **neuen** Innenverteidiger-Ausfall, und Seifert ist seit dem 15.10. in meinem Stand*** — **ich deute sie weiter nicht um.** *Zimmerschied stand gestern im Aufbautraining und wird heute als Ausfall geführt; er ist für mich kein Innenverteidiger, und ich löse darauf nichts aus.* ***Den Elversberger Trainernamen lasse ich offen*** (siehe Verworfenes 7).

**Elversberg hat Augsburg 4:3 geschlagen, nach 28 Minuten 3:0 geführt (Petkov, Günther, Rohr) und steht mit 10 Punkten vor Augsburg und über Leipzig.** **Der Aufsteiger spielt nicht international und hat die ganze Woche trainiert.** ***Nach Regel 4 tippe ich ihn nach Spielweise und Personallage, nicht nach Tabellenplatz*** — **und beides sagt: eine Mannschaft, die in Augsburg vier Tore erzielt, bekommt von mir keinen 2:0-Tipp entgegengesetzt.** **Ich bleibe bei einem knappen Heimsieg, weil Leipzig mit 16 Toren in 6 Spielen die zweitbeste Offensive der Liga hat.**

***Schwelle:*** *Wird Demichelis entlassen oder freigestellt, gehe ich auf **1:1**. Kündigt er auf der Spieltags-Pressekonferenz belegt eine Rotation an **oder** wird ein Leipziger Offensivausfall **vom Verein** mit genannter Ersatzlösung gemeldet, ebenfalls **1:1**. **Wird ein *neuer* Elversberger Innenverteidiger-Ausfall gemeldet (nicht Seifert), gehe ich auf **3:1**.***

---

### 5. 1. FSV Mainz 05 – SV Werder Bremen
**Samstag, 24.10.2026, 15:30 Uhr, Mewa Arena**
**Tipp: 1:1**
***unverändert — und beide Schwellen sind heute beantwortet, beide gegen eine Änderung***

***Diese Partie hatte gestern die dünnste Faktenlage des Spieltags und hat heute die klarste Schwellenentscheidung.***

***Erstens Füllkrug, und aus der Nichtmeldung von gestern ist eine Meldung geworden.*** **Er hat die erste Einheit der Mainz-Woche ausgelassen, aber `deichstube.de` und `weser-kurier.de` nennen ausdrücklich Belastungssteuerung und keine Verletzung; Deman, Grüll und Arthur wurden ebenso geschont, und alle vier haben die Belastungsarbeit mitgemacht.** ***Meine 2:0-Schwelle („wird Füllkrugs Ausfall belegt gemeldet") ist damit nicht offen, sondern negativ beantwortet*** — **und das ist ein echter Fortschritt gegenüber gestern, wo ich mich auf das Fehlen einer Meldung stützen musste.** *Nach einer Wett-Vorschau hat er in jedem seiner letzten fünf Bundesligaspiele getroffen und steht bei sieben Pflichtspieltoren; das deckt sich mit dem Doppelpack gegen Paderborn in meinem Archiv, bleibt aber eine Vorschauangabe.*

***Zweitens Topp, und meine Schwelle hat diesen Fall wörtlich vorhergesehen.*** **Aus der undatierten Meldung mit verwirrter Vereinszuordnung ist heute eine Diagnose geworden: Kreuzbandriss, Werder.** **Meine Schwelle lautete: „Wird Topps Ausfall datiert belegt, bleibe ich bei 1:1 und gehe nicht höher — Regel 2."** ***Genau das tue ich.*** **Werders Ausfallliste ist lang — Stage (Oberschenkel), Agu (Wade), Topp (Kreuzband), Musah (Muskel), Alvero (Wade), N'Diaye (Leiste), Njinmah im Teiltraining mit November-Ziel** — **aber sie senkt Werders Tore, sie erhöht nicht Mainz' Tore.**

***Was ich offen hinschreibe: das stärkste Argument gegen meinen eigenen Tipp ist heute größer geworden.*** **Werder ist seit fünf Spielen unbesiegt, Füllkrug trifft in Serie, und Mainz hat aus drei Heimspielen genau einen Punkt geholt** (*nach dem 1:0 in Gelsenkirchen der dritte Auswärtssieg aus drei Auswärtsspielen; die Heimrechnung ist meine eigene Subtraktion aus 10 Punkten in 6 Spielen und bleibt als Rechnung gekennzeichnet*). ***Das ist ein Argument für 1:2, und ich tippe es trotzdem nicht*** — **weil Werder in dieser Serie dreimal in Folge einen Zwei-Tore-Rückstand aufgeholt hat, also Punkte *nach* Rückstand geholt hat (Ligabestwert: sechs), und weil ich zu Mainz nach wie vor keinen Personalstand habe, der einen Auswärtssieg stützen würde.** ***Ein Remis ist hier nicht der Mittelweg, sondern die Summe beider Befunde: eine Heimmannschaft, die zu Hause nicht gewinnt, gegen eine Auswärtsmannschaft, die nicht verliert.***

**Zu Mainz bleibt die Lücke:** *Zentner, Kohr und Silas stehen nur in undatierten Listen; belegt ist allein Kohrs Ausfall bis Anfang Januar 2027 (Syndesmoseverletzung), und damit bleibt meine 2:1-Schwelle über seine Rückkehr erledigt.* **`bundesliga.com` führt die Partie als Duell Tietz gegen Füllkrug** — *das bestätigt Tietz als Mainzer Spitze, ohne eine Personalie zu liefern.*

***Schwelle:*** *Wird Füllkrugs Ausfall **doch** belegt gemeldet (nicht Schonung), gehe ich auf **2:0**. Wird ein Mainzer Innenverteidiger-Ausfall mit genannter Ersatzlösung gemeldet, gehe ich auf **1:2**. **Wird eine Werder-Rotation für Mainz angekündigt, bleibe ich bei 1:1 — Regel 2.***

---

### 6. SC Paderborn 07 – Hamburger SV
**Samstag, 24.10.2026, 15:30 Uhr, Home Deluxe Arena**
**Tipp: 1:2**
***unverändert — und die Änderung von gestern hält, erstmals mit Paderborns Personalstand dagegen geprüft***

***Dies war gestern die einzige Änderung des Laufs, und sie stand auf einem Befund, der heute bestätigt ist, gegen ein Gegenargument, das heute noch offen ist.***

***Bestätigt: Grönbaek ist zurück.*** **Ein Vorbericht führt ihn als zurückgekehrt und nennt ihn als Kandidaten für die Startelf.** **Meine Änderung von gestern (1:1 → 1:2) stand auf seinem absolvierten Einsatz gegen Stuttgart in der 78. Minute — belegt, gegen mein Archiv gegengeprüft und heute nicht bestritten.**

***Noch offen: Vieira.*** **Meine Schwelle für eine Rücknahme lautet: Vieiras Ausfall belegt **und** Grönbaek fehlt im Kaderaufgebot.** **Heute ist die Richtung präzisiert — die Berichte deuten auf die hintere Oberschenkelmuskulatur —, aber eine abschließende Einschätzung fehlt, und Grönbaek fehlt nirgends.** ***Beide Bedingungen sind nicht erfüllt, und ich nehme die Änderung nicht zurück.***

***Und hier ist die Lücke, die drei Läufe offenstand, endlich gefüllt: Paderborns Personalstand.*** **`nw.de` nennt Oliver Batista Meier mit einer Innenbandverletzung im Sprunggelenk als definitiven Ausfall für dieses Heimspiel, dazu Timur Gayret und Marcel Hoffmeier; Laurin Curda soll trotz Handbruchs spielen können, und Nyamekye Awortwie-Grant ist erst ins Teiltraining zurückgekehrt.** ***Drei Schwellenfragen klären sich damit auf einmal:***
- ***Awortwie-Grant:*** **meine 1:1-Schwelle verlangte eine belegte Rückkehr. Teiltraining ist keine.** **Nicht ausgelöst.**
- ***Tigges und Marino:*** **meine 1:3-Schwelle verlangte deren Ausfall. Beide stehen in keiner Ausfallliste.** **Nicht ausgelöst** — *und das ist die wichtigere Hälfte des Befunds, weil es die beiden Torschützen des 2:0 bei Werder sind.*
- ***Batista Meier:*** **ein Offensivausfall bei Paderborn.** **Nach Regel 2 senkt das Paderborns Tore, es erhöht nicht die des HSV.**

***Und damit die Frage, die heute ehrlich zu stellen ist: warum nicht 0:2?*** **Ein weiterer Offensivausfall beim Tabellensechzehnten mit 5 Toren in 6 Spielen wäre ein Argument dafür.** ***Ich tippe es nicht, und der Grund sind Tigges und Marino.*** **Paderborn hat in jedem der letzten beiden Heimspiele getroffen und bei Werder mit genau diesen beiden 2:0 geführt; in der Nachspielzeit stand Philippe am Pfosten, Torwart Noll hielt mehrfach stark.** **Solange die beiden Werder-Torschützen verfügbar sind, schreibe ich Paderborn zu Hause keine Null.** *Kettemann beschreibt seine Mannschaft als „Gruppe junger, unerfahrener Bundesliga-Menschen", der es an Torgefahr fehlt — Regel 4 angewandt, und sie hält den Tipp knapp.*

**Beim HSV weiter aus: Remberg (Kreuzbandriss, wohl Restsaison), Vuskovic (Sperre bis 15. November — heute erstmals mit Enddatum), Daka und Jatta im Aufbautraining, Moffi mit Knieproblemen.** **Sambi Lokonga hofft auf sein Comeback genau in Paderborn, sein Einsatz ist offen** — *eine Prognose, die den Tipp nicht trägt.* ***Warum nicht 1:3: 6 Tore in 6 Spielen und ein Torverhältnis von −9 decken keinen höheren Auswärtstipp, auch mit Grönbaek nicht.*** **Die Dreier-Serie des HSV steht auf dünnen Zahlen, und das bleibt so.**

***Schwelle:*** *Wird Vieiras Ausfall belegt **und** fehlt Grönbaek im Kaderaufgebot, gehe ich zurück auf **1:1**. Fällt bei Paderborn Tigges **oder** Marino aus, gehe ich auf **1:3**. **Wird Awortwie-Grants Rückkehr ins Kaderaufgebot belegt, gehe ich auf **1:1**.***

---

### 7. Borussia Dortmund – Eintracht Frankfurt
**Samstag, 24.10.2026, 18:30 Uhr, Signal Iduna Park**
**Tipp: 2:0**
***unverändert — und die Partie mit dem größten Puffer des Spieltags***

***Die Schwelle, die diesen Tipp gestern hätte ändern können, ist am Dienstag entschieden worden, und heute ist nichts dazugekommen, was sie wieder öffnet.***

**Dortmund hat in Baku 2:1 gewonnen, Guirassy hat beide Tore erzielt (10., 53.), und damit sind die Mannschaftsflaute von drei Pflichtspielen und Guirassys eigene Torflaute beendet.** **Meine 1:0-Schwelle („bleibt Dortmund in Aserbaidschan ohne Tor") ist erledigt.** *Einschränkend bleibt: der Sieg war weniger souverän als das Ergebnis — 22 Torschüsse gegen 13, McCarthys Ausgleich in der 39. Minute, und Kovač mahnte die Chancenverwertung an.*

***Die Dortmunder Ausfallliste ist heute länger und besser belegt als gestern, und sie trifft meinen Tipp trotzdem nicht.*** **Karetsas' Ausfall ist mit Vereinszitat belegt — Ricken: „Kos hat eine Bandverletzung im Fuß. Er wird nicht nach Baku mitfliegen und auch gegen Frankfurt am Samstag nicht spielen können"; `neunzigplus.de` nennt mehrere Wochen.** ***Dazu revidiere ich meine gestrige Verwerfung:*** **Emre Can (Kreuzbandriss), Konstantelias (Kreuzbandriss seit dem 1. Spieltag) und Lerma (Muskelverletzung) werden heute von einem zweiten, unabhängigen Vorbericht genannt und sind damit gegenbestätigt.** *Zu Kaba widersprechen sich die Angaben (Schulter bzw. Knie) — offen.* ***Entscheidend für meine Schwelle ist, dass keiner dieser Namen ein Innenverteidiger ist:*** **Schlotterbeck, Anton und Bensebaini standen im 24-Mann-Kader von Baku, es gibt keinen Dortmunder Innenverteidiger-Ausfall, Guirassy ist Doppeltorschütze, und eine Rotationsankündigung von Kovač gibt es nicht.**

**Belastung: Dienstag 18:45 in Baku, die weiteste Reise des Spieltags — aber mit vier Tagen Abstand, dem größten Puffer aller sieben Europapokalstarter.** ***Dortmund ist die einzige Mannschaft dieses Spieltags, die weit gereist ist und trotzdem keinen Abschlag nach Regel 3 bekommt.***

***Zu Frankfurt ist die Lage heute zum zweiten Mal unabhängig geklärt und für die Eintracht entspannt.*** **Adi Hütter ist als Trainer bestätigt (erwartetes 4-2-3-1), Ngankam fehlt mit Oberschenkelverletzung, Pimpong und Maluze sind fraglich, gesperrt ist niemand, und Onyedika steht bei vier Gelben Karten.** ***Meine 3:0-Schwelle zielt auf einen Frankfurter Innenverteidiger-Ausfall, und ein solcher ist nicht gemeldet*** — **Robin Koch ist verfügbar, von Hütter nach dem Köln-Spiel ausdrücklich gelobt.** **Was den Tipp trägt, bleibt die Abwehr: 16 Gegentore in 6 Spielen, die zweitschwächste der Liga, und zwei Spiele vor diesem Spieltag eine 0:6-Niederlage, die Hütter selbst als „Klatsche" bezeichnet hat.** **Der Köln-Sieg war Frankfurts erster Heimsieg seit dem 14. März; auswärts steht die Mannschaft weiter ohne Ausweis.** *Erstmals habe ich zu dieser Partie eine Historienangabe: eine Vorschau nennt, dass Hütter als Frankfurter Trainer nur zwei von sechs Spielen gegen den BVB verloren hat. Ich verrechne sie nicht — es ist eine Vorbereitungsangabe, keine Statistikquelle — aber ich nenne sie, weil sie gegen meinen Tipp spricht und ich sie nicht unterschlage.*

***Schwelle:*** *Wird ein Dortmunder Innenverteidiger-Ausfall mit genannter Ersatzlösung gemeldet **oder** fällt Guirassy aus, gehe ich auf **1:1**. Kündigt Kovač auf der Spieltags-Pressekonferenz belegt eine Rotation an, gehe ich auf **1:0**. **Wird bei Frankfurt ein Innenverteidiger-Ausfall **belegt** gemeldet (Koch eingeschlossen), gehe ich auf **3:0**.***

---

### 8. TSG Hoffenheim – Bayer 04 Leverkusen
**Sonntag, 25.10.2026, 15:30 Uhr (MEZ), SNP Arena**
**Tipp: 2:2**
***unverändert — und die Partie, die am Donnerstagabend noch am meisten bewegen kann***

***Drei der fünf Schwellen dieser Partie sind heute geprüft, keine ausgelöst, und zwei hängen an Spielen, die erst am Donnerstag stattfinden.***

***Erstens Schick: nicht ausgefallen, nicht geschont.*** **Die Vorschau zum Kreta-Spiel führt ihn als Mittelstürmer in der erwarteten Startelf.** ***Meine 1:1-Schwelle ist damit nicht ausgelöst.*** **Er ist fit und hat in allen sechs Bundesligaspielen getroffen.**

***Zweitens die Leverkusener Rotation: keine Fundstelle.*** **Eine Pressekonferenz-Aussage zur Rotation vor Kreta habe ich nicht gefunden, nur Vorschautexte.** ***Ich löse meine 2:1-Schwelle nicht auf einer Nichtfundstelle aus*** — **dieselbe Regel, die ich heute bei Hoeneß angewandt habe.** **Neu und belegbar ist stattdessen der Europa-League-Kader: Hofmann nachnominiert, Boniface nicht im Kader.** **Ausfälle: Terrier bis Dezember, Kofane, Doué und Ben Seghir mit Muskelverletzungen, Culbreath fraglich.**

***Drittens Hoffenheims Startelf: kein weiterer Ausfall aus der Gladbach-Elf.*** **Meine Schwelle lautet „fällt über De Cat, Kabak und Wimmer hinaus ein Spieler der Gladbach-Startelf aus", und die Pressekonferenz vom Mittwoch hat keine neue Personalie geliefert.** **Der Stand bleibt: De Cat mit Meniskusschaden und Operation vom Montag lange aus, Hajdari mehrere Wochen, Wimmer verletzt genannt, Kabak als Kandidat für die Startelf gegen Lyon.** ***Keiner der belegten Ausfälle stand in der Elf, die in Gladbach 2:1 gewonnen hat*** (Baumann; Coufal, Hranáč, Machida, Rots; Avdullahu, Conté, Prass; Lemperle, Asllani, Hložek) — **es sind Kaderverluste, keine Stammelfverluste.**

***Was den Tipp trägt, ist unverändert der Belastungsunterschied, und er ist der schärfste des Spieltags.*** **Leverkusen muss Donnerstag 18:45 nach Kreta — die weiteste Donnerstagsreise — und dann Sonntag 15:30 schon wieder auswärts antreten; Hoffenheim empfängt Lyon zu Hause.** ***Der Abschlag nach Regel 3 bleibt voll bestehen.*** **Dazu Hoffenheims 2:1 in Gladbach (Conté 11., Prass 54.).**

***Was ich heute gegen mich selbst eintrage:*** **gestern habe ich geschrieben, Hoffenheims Donnerstag werde „eher leichter", weil bei Lyon Tagliafico, Ouédraogo und Openda fehlen.** **Heute kommt Lyon als Spitzenreiter der Ligue 1, und Ilzer nennt die Mannschaft wegen Fonsecas taktischer Flexibilität und des Umschaltspiels „extrem gefährlich".** ***Meine Einschätzung von gestern war zu optimistisch, und ich korrigiere die Begründung, nicht den Tipp*** — **Hoffenheim hat erst drei von neun Pflichtspielen gewonnen, keines in der Europa League.** *Dass Bernardo in der Gladbach-Startelf fehlte, bleibt mein Indizienschluss für eine abgesessene Einspielsperre — kein Beleg der Sperrdauer.*

***Schwelle:*** *Wird Schicks Ausfall oder Schonung belegt, gehe ich auf **1:1**. Kündigt Leverkusen nach Kreta belegt eine Rotation an, gehe ich auf **2:1** (für Hoffenheim). Verliert Hoffenheim am Donnerstag gegen Lyon hoch (drei Tore oder mehr), gehe ich zurück auf **1:2**. Wird Bernardos Sperre als länger als ein Spiel belegt, gehe ich auf **1:2**. **Fällt über De Cat, Kabak und Wimmer hinaus ein Spieler der Gladbach-Startelf aus, gehe ich auf **1:2**.***

---

### 9. SC Freiburg – FC Bayern München
**Sonntag, 25.10.2026, 17:30 Uhr (MEZ), Europa-Park Stadion**
**Tipp: 1:2**
***unverändert — und die Partie mit den meisten neuen Fakten und der schwersten Entscheidung des Tages***

***Hier ist heute mehr passiert als bei jeder anderen Partie, in beide Richtungen, und am Ende hebt sich beides auf. Ich lege die Rechnung offen, weil der Tipp sonst wie Trägheit aussieht.***

***Erstens die Schwelle, die negativ entschieden ist: Kompany steht an der Linie.*** **Er hat gegen Arsenal gecoacht, nach einem Tag krank im Bett.** **Meine Schwelle lautete „wird belegt, dass Kompany auch am Sonntag nicht an der Linie steht, gehe ich auf 1:1".** ***Das Gegenteil ist belegt, die Schwelle ist erledigt.*** **Eine Rotationsankündigung für Freiburg gibt es ebenfalls nicht** — **meine zweite 1:1-Schwelle bleibt damit unausgelöst.**

***Zweitens, und das ist die Hauptnachricht des Tages: Kimmich fehlt, und seine Rückkehr ist offen.*** **Trauerfall im engsten Familienkreis; nach `fussballnationalmannschaft.net` ist sein Vater gestorben, der Verein bittet um Respekt für die Privatsphäre, und wann er zur Mannschaft zurückkehrt, ist nach Vereinsangabe offen.** **Gegen Arsenal spielte Bischof neben Pavlović.** ***Ich verrechne das nicht, und ich nenne den Grund, weil es derselbe ist, mit dem ich gestern Vieira behandelt habe:*** **ein Tipp steht nicht auf einer offenen Frage.** **Zwischen Mittwoch und Sonntag liegen vier Tage, ein Trauerfall ist keine Verletzung mit Ausfalldauer, und der Verein hat ausdrücklich kein Datum genannt — weder für die Rückkehr noch für ein weiteres Fehlen.** ***Hätte ich auf diese Nachricht hin geändert, hätte ich eine Abwesenheit für Sonntag behauptet, die keine Quelle behauptet.*** **Stattdessen steht sie als Schwelle unten.**

***Drittens, und belegt: Freiburg plant den Donnerstag als Schonung.*** **Lienhart fehlt in Monaco wegen Belastungssteuerung, nicht verletzt; Rosenfelder ersetzt ihn; Schuster kündigt eine Rotation an und begründet sie damit, dass er am Sonntag gegen den Tabellenführer die stärkste Elf braucht.** ***Das entwertet meinen Regel-3-Abschlag für Freiburg, und ich schreibe die Regel deshalb oben ausdrücklich um:*** **wer die Europapartie belegt als Schonungstermin plant, bekommt keinen Abschlag.** **Gestern hatte ich für die 550 Kilometer nach Monaco „keinen vollen Abschlag" gegeben; heute gebe ich keinen.** ***Das ist eine Verschiebung zugunsten Freiburgs, und sie ist die einzige heute, die auf einem Trainerzitat statt auf einer Vermutung steht.***

***Viertens die Gegenrechnung für Bayern, und sie ist nicht klein.*** **Neuer ist nach Fußverletzung zurück im Tor** — *eine Korrektur meines Vortagsstands, der „womöglich länger" führte, und ein Zugewinn gegenüber Urbig.* **Olise kehrt nach der Gelb-Rot-Sperre aus der Champions League ausgeruht zurück** — *er hat gegen Arsenal nicht gespielt.* **Bayern steht bei 22:5 Toren, ist in sechs Bundesligaspielen unbesiegt und bleibt auch in der Ligaphase ungeschlagen.**

***Und damit die Abwägung, die ich nicht verstecke.*** **Auf der einen Seite: Kimmich fehlt (für Sonntag offen), Bayern hat zu Hause zwei Punkte liegen lassen, 90 Minuten in den Beinen, Musiala fehlt belegt auch am Sonntag, Luis Díaz' Status ist widersprüchlich, und Freiburg kommt frisch und mit Absicht frisch.** **Auf der anderen Seite: Kompany coacht, Neuer hält, Olise ist ausgeruht, vier Tage Pause statt drei, und der Offensivunterschied ist in Zahlen eindeutig (22:5 gegen 15:6).** ***Mein Tipp war schon gestern der knappste mögliche Bayern-Sieg, und genau das ist der Punkt:*** **die neuen Fakten machen die Partie enger, und enger als ein Tor Unterschied geht nicht, ohne auf ein Remis zu gehen.** ***Für ein Remis bräuchte ich Kimmichs Ausfall für Sonntag belegt, und den habe ich nicht.*** **Freiburg ist Dritter mit 13 Punkten, hat in Leverkusen geführt und bis zur 76. Minute gestanden; Beste und Scherhant sind fit, Suzuki ist nach abgesessener Sperre wieder dabei, Muslija fehlt mit Kreuzbandriss.**

*Zur Belastung auf der Gegenseite: Monacos Kader bleibt geschwächt (Balogun nicht nominiert, Dier Oberschenkel, Idumbo-Muzambo Hüftbeuger und Leiste, Camara fraglich, Brunner nach Sperre zurück) — das macht Freiburgs Rotation leichter durchzuhalten und stützt die Schonungsabsicht.*

***Schwelle:*** *Wird Kimmichs Fehlen für Sonntag belegt (Kaderaufgebot ohne ihn oder Vereinsangabe), gehe ich auf **1:1**. Wird eine Bayern-Rotation für Freiburg belegt angekündigt, ebenfalls **1:1**. **Verliert Freiburg am Donnerstag in Monaco hoch **und** wird trotz der Schonungsankündigung eine Freiburger Rotation für Sonntag gemeldet, gehe ich auf **0:2**. Kompanys, Musialas und Neuers Status ändern nichts mehr.***

---

## Verteilung und Selbstkontrolle

| | Anzahl | Partien |
|---|---|---|
| **Heimsiege** | **5** | 1 (2:0), 2 (2:1), 3 (1:0), 4 (2:1), 7 (2:0) |
| **Remis** | **2** | 5 (1:1), 8 (2:2) |
| **Auswärtssiege** | **2** | 6 (1:2), 9 (1:2) |

**Gesamttore: 23 in 9 Partien, 2,56 je Spiel** — *identisch mit gestern, weil kein Tipp gewechselt hat.*

***Selbstkontrolle zu diesem Lauf, in drei Punkten:***

1. ***Null Änderungen sind ein Ergebnis, kein Ausfall.*** **Sechs Schwellen waren heute an echten Dokumenten prüfbar — Kompany, Ache, Füllkrug, Topp, Awortwie-Grant, Schick — und alle sechs sind gegen eine Änderung ausgegangen.** *Am 20.10. war eine prüfbare Schwelle übererfüllt und hat sofort einen Tipp bewegt; dass heute keine es tut, liegt an den Befunden, nicht an fehlender Prüfung.*
2. ***Die eine Nachricht, die einen Tipp bewegen könnte, habe ich bewusst nicht verrechnet.*** **Kimmichs Fehlen ist für Mittwoch belegt und für Sonntag offen.** **Ich halte mich an die Regel, die ich gestern bei Vieira angewandt habe, und schreibe die Schwelle hin, statt die Lücke zu füllen.** *Wenn das Kaderaufgebot am Sonntag ohne ihn kommt, ist Partie 9 die erste Änderung des nächsten Laufs.*
3. ***Eine eigene Verwerfung von gestern war zu streng.*** **Die Dortmunder Ausfallliste (Can, Konstantelias, Lerma) habe ich gestern wegen fehlender Datierung nicht verwendet; heute trägt sie eine zweite Quelle.** *Tippwirkung hatte sie keine, aber die Lehre ist, dass „undatiert" ein Grund zum Nachprüfen ist und nicht zum Verwerfen.*

---

## Quellen

**Alle Angaben dieses Laufs stammen aus `WebSearch`-Ergebnissen (Titel und Zusammenfassungen).** ***Kein Volltextabruf war möglich*** — `WebFetch` scheitert zum elften Tag an der Namensauflösung.

**Europapokal Mittwoch:** `spox.com`, `vavel.com`, `bnn.de`, `fussballnationalmannschaft.net` (Bayern – Arsenal 2:2); `realtotal.de`, `fussballnationalmannschaft.net`, `rhein-zeitung.de` (dpa) (Real Madrid – Leipzig 4:1).
**Pressekonferenzen:** `tsg-hoffenheim.de`, `sportschau.de` (SWR), `sport1.de`, `sports.yahoo.com` (Ilzer vor Lyon); `sports.yahoo.com`, `zvw.de`, `badische-zeitung.de`, `stimme.de` (Schuster vor Monaco).
**Personalmeldungen:** `fussballnationalmannschaft.net`, `lessentiel.lu`, `neunzigplus.de`, `ad-hoc-news.de`, `ran.joyn.de` (Bayern); `koeln.t-online.de`, `baykusen.de` (Köln/Schalke); `recklinghaeuser-zeitung.de`, `ruhrnachrichten.de`, `reviersport.de`, `ligaportal.at` (Schalke); `nw.de`, `magazin.comunio.de` (Paderborn/HSV); `deichstube.de`, `weser-kurier.de`, `90min.de` (Werder); `gladbachlive.de`, `bmg-news.de`, `fussballdaten.de` (Gladbach); `bundesliga.com`, `sport.sky.de`, `sport.de`, `sportsmole.co.uk` (Dortmund/Frankfurt); `rb-fans.de`, `kicker.de` (Vereinsinfo), `magazin.comunio.de` (Leipzig/Elversberg); `rotowire.com` nach `Augsburger Allgemeine`, `ligainsider.de` (Augsburg); `fussballnationalmannschaft.net`, `sportsmole.co.uk` (Leverkusen).
**Leipziger Trainerlage:** `fussballtransfers.com`, `sport.de`, `ms-aktuell.de`, `rblive.de`.
**Tabelle:** `de.wikipedia.org`, `bundesliga.com` — **an drei Werten gegenbestätigt** (Bayern 6/22:5/+17/14, Dortmund 6/11:4/+7/14, Gladbach 6/0/8:20/Platz 18).
**Ansetzungen und Anstoßzeiten:** `datencenter.dfb.de`, `anstosszeiten.de`, `ruhrnachrichten.de` — **alle neun Partien und alle Anstoßzeiten gegenbestätigt und unverändert gegenüber gestern** (abweichende `sport1`-Zeiten verworfen).
**Umgebung:** `curl "$HTTPS_PROXY/__agentproxy/status"` — **heute erstmals erfolgreich**, `recentRelayFailures: []`.
