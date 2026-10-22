# Projektanweisungen: Bundesliga-Tipps

Dieses Repo wird von zwei geplanten Aufgaben bearbeitet:

- **„Bundesliga-Tipps"** — täglich abends. Schreibt `tipps-aktuell.md` neu.
- **„Bundesliga-Lernabgleich"** — montags mittags. Rechnet den gespielten Spieltag ab und
  schreibt `lernen.md` fort. Fasst `tipps-aktuell.md` nicht an.

Die Arbeitsschritte stehen jeweils im Prompt der Routine. Hier stehen nur Vorgaben, die
der Nutzer nachträglich ergänzt hat — sie gelten **zusätzlich** zum Routine-Prompt und haben
bei Widersprüchen Vorrang.

## Umfang der Benachrichtigung

Die PushNotification am Ende des Laufs ist die einzige Ausgabe, die den Nutzer erreicht; die
Antwort im Terminal liest niemand. Für ihren Inhalt gilt:

- **Donnerstags** (Wochentag zu Beginn per `date` prüfen): **alle neun Partien vollständig**
  auflisten, nicht nur die geänderten. Eine Zeile je Partie in der Reihenfolge des Spielplans,
  jeweils mit Heim – Gast, Anstoßzeit und Tipp, dahinter der Vermerk `geändert von <alter Tipp>`
  bzw. `unverändert`. Bei geänderten Partien zusätzlich in einem Halbsatz den Auslöser nennen.
- **An allen übrigen Tagen**: kompakte Form — geänderte Tipps mit Begründung, die unveränderten
  als eine Sammelzeile.
- **Immer**: Quellenprobleme, gescheiterte Abrufe, offene Recherchelücken und Korrekturen am
  Vortagsstand ausdrücklich nennen.

*Vom Nutzer angeordnet am 11.09.2026, gültig ab der Woche vom 14.09.2026.*

## Lernen aus gespielten Spieltagen

**`lernen.md` ist das Gedächtnis der Routine, und der Abendlauf muss es benutzen.**

- ***Pflicht für jeden Abendlauf:*** **Lies `lernen.md`, bevor du tippst**, und wende den
  Abschnitt *Aktive Lehren* auf alle neun Partien an. **Nenne im Bericht ausdrücklich, welche
  Lehre bei welcher Partie gewirkt hat** — und auch, wo du bewusst gegen eine Lehre
  entschieden hast, mit Begründung.
- **Widerspricht eine Lehre dem Routine-Prompt, hat die Lehre Vorrang** (sie stammt aus einer
  echten Abrechnung).
- **Der Abendlauf ändert `lernen.md` nicht.** Fällt dir eine Lehre auf, die dort fehlt, notiere
  sie im Tippbericht unter *Selbstkontrolle*; der Montagslauf übernimmt sie.
- **Die vier bzw. mittlerweile mehr „Regeln", nach denen `tipps-aktuell.md` den Spieltag anlegt,
  sind die Kurzfassung der aktiven Lehren.** Sie dürfen nicht auseinanderlaufen: ändert der
  Montagslauf eine Lehre, zieht der nächste Abendlauf die Regelliste nach.

*Vom Nutzer angeordnet am 22.10.2026.*

## Dateistruktur

- `tipps-aktuell.md` — aktueller Tippstand, wird bei jedem Abendlauf komplett neu geschrieben.
- `archiv/JJJJ-MM-TT.md` — der jeweils vorherige Stand, vor dem Überschreiben dorthin kopiert.
  Das Datum ist das des bisherigen Standes, ersatzweise das gestrige.
- `lernen.md` — Abrechnungen gespielter Spieltage und die daraus abgeleiteten aktiven Lehren.
  Wird **nur** vom Montagslauf geschrieben, von jedem Abendlauf **gelesen**.

## Git

Der Klon der geplanten Sitzung steht auf einem abgekoppelten HEAD (`detached HEAD`).
`git push -u origin HEAD:refs/heads/main` funktioniert, `git push -u origin HEAD` nicht.
