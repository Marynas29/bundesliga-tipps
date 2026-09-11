# Projektanweisungen: Bundesliga-Tipps

Dieses Repo wird von einer täglichen geplanten Aufgabe („Bundesliga-Tipps", 23:00 MEZ/MESZ)
bearbeitet. Die Arbeitsschritte stehen im Prompt der Routine. Hier stehen nur Vorgaben, die
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

## Dateistruktur

- `tipps-aktuell.md` — aktueller Tippstand, wird bei jedem Lauf komplett neu geschrieben.
- `archiv/JJJJ-MM-TT.md` — der jeweils vorherige Stand, vor dem Überschreiben dorthin kopiert.
  Das Datum ist das des bisherigen Standes, ersatzweise das gestrige.

## Git

Der Klon der geplanten Sitzung steht auf einem abgekoppelten HEAD (`detached HEAD`).
`git push -u origin HEAD:refs/heads/main` funktioniert, `git push -u origin HEAD` nicht.
