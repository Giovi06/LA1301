# LA1301
Unity 2D Street Fighter

Giovanni Innamorato, Giuliano Martullo, Steven Salie

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|20.09.23| 0.0.1   | Funktionierendes Playermovement|
|18.10.23| 0.0.2   | Main Menu erstellt, Healthbar erstellt, Player animationen implementiert|
|25.10.23| 0.1     |Funktionierende Healthbar und Main Menu scene|
|01.11.23| 1.0.0   |Player combat funktioniert, Game Over Scene erstellt, Sounds hinzugefügt|

## 1 Informieren

### 1.1 Ihr Projekt

Wir haben in Unity ein 2D Street Fighter im Pixel Design erstellt.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
|1|Muss|F| Als ein Spieler möchte ich, dass das Player-Movement funktioniert, damit ich meinen Charakter im Spiel steuern kann.|
|2|Muss|F|Als ein Spieler möchte ich, dass das Main Menu erstellt wird, damit ich das Spiel starten und navigieren kann.|
|3|Muss|F|Als ein Spieler möchte ich, dass die Healthbar erstellt wird, damit ich den Gesundheitszustand meines Charakters im Auge behalten kann.|
|4|Muss|F|Als ein Spieler möchte ich, dass die Player-Animationen implementiert werden, um eine flüssige und ansprechende Spielgrafik zu haben.|
|5|Muss|F|Als ein Spieler möchte ich, dass das Player-Combat funktioniert, damit ich gegen Gegner kämpen und das Spiel genießen kann.|
|6|Muss|F|Als ein Spieler möchte ich, dass die Game Over Scene erstellt wird, um den Spielabschluss anzuzeigen.|
|7|Muss|Q| Als ein Spieler möchte ich, dass Sounds hinzugefügt werden, um das Spielerlebnis zu verbessern.|
|8|Muss|F|Als ein Spieler möchte ich mich ducken können, und dabei möchte ich langsamer fortbewegen können, um besser ausweichen zu können.|
|9|Muss|F||
|10|Muss|F||


✍️ Jede User Story hat eine ganzzahlige Nummer (1, 2, 3 etc.), eine Verbindlichkeit (Muss oder Kann?), und einen Typ (Funktional, Qualität, Rand). Die User Story selber hat folgende Form: *Als ein 🤷‍♂️ möchte ich 🤷‍♂️, damit 🤷‍♂️*.

### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |Das Spiel läuft.|Der Spieler versucht, den Charakter zu bewegen.|Der Charakter bewegt sich entsprechend der Eingabe des Spielers.|
| 2.1  |Das Spiel befindet sich im Hauptmenü.|Der Spieler klickt auf die Starttaste im Hauptmenü.|Das Spiel startet und die Spielumgebung wird geladen.|
|3.1|Das Spiel läuft und der Spielercharakter hat einen Gesundheitsbalken.|Der Spielercharakter erleidet Schaden.|Der Gesundheitsbalken des Charakters wird aktualisiert, um den verlorenen Gesundheitszustand anzuzeigen.|
|4.1|Das Spiel läuft.|Der Spieler beobachtet die Bewegungen des Charakters.|Der Charakter zeigt flüssige und ansprechende Animationen entsprechend seinen Aktionen.|
|5.1| Das Spiel läuft und der Spielercharakter kann gegen Gegner kämpfen.|Der Spielercharakter greift einen Gegner an.|Der Gegner erleidet Schaden, die Healthbar sinkt.|
|6.1 |Das Spiel läuft und der Spieler hat das Spiel beendet.|Der Spieler beendet das Spiel oder erreicht ein Game Over.|Die Game Over Scene wird angezeigt, um den Spieler über das Spielende zu informieren.|
|8.1|Der Spielercharakter kann sich bewegen.|Der Spieler versucht, den Charakter ducken zu lassen und sich langsamer zu bewegen.|Der Charakter duckt sich und bewegt sich langsamer, um es dem Spieler zu ermöglichen, Angriffen auszuweichen.|
|||||
|||||
✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, die der Testfall abdeckt, und `m` von `1` an nach oben gezählt. Beispiel: Der dritte Testfall, der die zweite User Story abdeckt, hat also die Nummer `2.3`.


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |20.9|Giovanni|Implementierung des grundlegenden Player-Movements, einschließlich Bewegung nach links und rechts.|180'|
|1.B|-|Giovanni| Implementierung von zusätzlichen Bewegungsaktionen wie Springen und Ducken.|180'|
|2.A|-|Steven|Erstellung des Hauptmenüs mit Optionen wie "Play", "Options" und "Quit".|180'|
|3.A|-|Giuliano| Implementierung der Healthbar, die den Gesundheitszustand des Spielers anzeigt.|180'|
|4.A||Giovanni| Implementierung von grundlegenden Animationen für den Spielercharakter, einschließlich Laufen, Springen und Ducken.|120'|
|5.A||Giovanni|Implementierung von Grundmechaniken für den Spielerkampf, einschließlich Angriff und Verteidigung.|240'|
|6.A||Steven|Erstellung der Game Over Scene, die dem Spieler das Spielende anzeigt.|120'|
|7.A||Giuliano|Hinzufügen von Soundeffekten und Hintergrundmusik, um das Spielerlebnis zu bereichern.|180'|
|8.A||Giovanni|Implementierung der Fähigkeit des Spielers, sich zu ducken und dabei langsamer zu bewegen, um Angriffen auszuweichen.|180'|
||||||

## 3 Realisieren

| AP-№ | Datum     | Zuständig | Geplante Zeit | Tatsächliche Zeit |
| ---- | --------- | --------- | ------------- | ----------------- |
| 1.A  | 20.09.23  | Giovanni  | 180 Minuten   |       180 Minuten|
| 1.B  | 20.09.23  | Giovanni  | 180 Minuten   | 180 Minuten|
| 2.A  | 18.10.23  | Steven    | 180 Minuten   | 180 Minuten      |
| 3.A  | 18.10.23  | Giuliano  | 180 Minuten   | 180 Minuten       |
| 4.A  | 18.10.23  | Giovanni  | 120 Minuten   | 120 Minuten    |
| 5.A  | 01.11.23  | Giovanni  | 240 Minuten   | 240 Minuten      |
| 6.A  | 01.11.23  | Steven    | 120 Minuten   | 120 Minuten       |
| 7.A  | 01.11.23  | Giuliano  | 180 Minuten   | 180 Minuten    |
| 8.A  | 01.11.23| Giovanni  | 180 Minuten   | 180 Minuten|


## 4 Kontrollieren

###  Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |


