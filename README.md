# Bomberman

# Projekt-Dokumentation

Özden, Heiniger

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 20.9      | 0.0.1   | Anfang |
| 18.10      | 0.0.2    |  Erste Prototypen                                                            |
| 25.10      | 0.0.3    |   Erste richtige Version des Spieles                            |
| 1.11      | 1.0.0   |   Fertiges Spiel                                                           |

## 1 Informieren

### 1.1 Ihr Projekt

In unserem Projekt programmieren wir in Unity ein 2D Spiel, welches verschiedene Levels hat.


Wir möchten lernen, wie man verschiedene Levels erstellt und wie man auf diese zugreiffen kann, beziehungsweise spielen kann. Ausserdem möchten wir uns mit Unity vertraut machen, und ein kleines Spiel erstellten und wir möchten unsere Programmierfähigkeiten weiter ausbauen.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
|1|muss|funktional|Als Spieler möchte ich mich bewegen, damit ich die Chance habe zu gewinnen.|
|2|muss|funktional|Als Spieler möchte ich Bomben werfen, damit ich Hindernisse zersötren kann wie auch meinen Gegner|
|3|muss|funktional|Als Spieler möchte ich Bomben aufsameln können, damit ich mehr Munition habe|
|4|muss|funktional|Als Spieler möchte ich eine KI die gegen mich spielt, damit ich das Spiel spielen kann.|
|5|muss|funktional|Als Spieler möchte ich, dass die Bomben schaden machen, damit ich gewinnen oder verlieren kann.|
|6|kann|funktional|Als Spieler möchte ich die Schwierigkeit einstellen können, damit ich mich verbessern kann.|
|7|kann|qualität|Als Spieler möchte ich ein Scoreboard haben, damit ich sehen kann wie meine KD aussieht.|
|8|kann|funktional|Als Spieler möchte ich Multiplayer, damit ich gegen andere Menschen spielen kann.|




### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Das Spiel lässt den Spieler sich bewegen             |  W,A,S,D       | Spieler bewegt sich dementsprechend |
| 2.1  | Spiel wurde gestartet       |  Leertaste      |Bombe wird platziert            |
| 2.2  | Bombe wurde platziert|  /      |Bombe zerstört Objekte so wie auch den Spiel            |
|3.1|Spieler braucht neue Bomben|Spieler läuft über das Bombenicon|+1 Bomben|
|4.1|Das Level hat Gegner|-|KI Gegner existiert|
|5.1|Bombe wurde gelegz|/|Spieler oder KI verliert leben|
|6.1|Spiel gestarten|Schwierigkeit auswählen|KI verhaltet sich anhand der schwierigkeit|
|7.1|Runden sind vergangen|Tabulatortaste|Game zeigt Scoreboard|
|8.1|Spiel wird gestartet|Multiplayer auswählen|Spieler kann joinen|





## 2 Planen
| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 29.05 | Mirhan | Skript für den Player, damit man ihn bewegen kann. | 60 min |
| 1.B  | 29.05 | Mirhan | Skript, damit die Kamera nicht statisch ist sondern sich mit dem Spieler mit bewegt. | 20 min |
| 2.A  |  05.06 | Lukas | Skript für das Werfen der Bomben. | 60 min |
| 2.B  |  05.06 | Lukas | Skript für die Bombenexplosion und Schaden. | 45 min |
| 3.A  |  05.06 | Lukas | Ammobox programmieren, damit Bomben eingesammelt werden können. | 45 min |
| 4.A  | 05.06| Mirhan | Gegner (KI) für das Spiel erstellen. | 120 min |
| 5.A  | 05.06| Lukas | Funktion, damit die Bomben Schaden verursachen. | 45 min |
| 6.A  | 12.06 | Lukas | Schwierigkeitseinstellungen hinzufügen. | 45 min |
| 7.A  |12.06  | Mirhan | Scoreboard hinzufügen. | 45 min |
| 8.A  | 12.06  | Lukas | Multiplayer-Funktionalität hinzufügen. | 120 min |

Total: 18

## 3 Entscheiden

Wir haben uns entschieden einen Platformer zu programmieren mithilfe von Unity. Man soll im Spiel das Ende erreichen, was sich ganz rechts befindet. Falls man dabei eliminiert wird, haben wir uns entschieden einen Knopf einzufügen, der das Spiel neustartet. Im Spiel selber gibt es Gegner, die dich beim Berühren eliminiert, Spikes die das selbe machen und Münzen die sammelbar sind. Zur Verteidigung steht eine Waffe mit 10 Schüssen zur Verfügung, die durch Munitionsboxen wieder aufgefüllt werden kann.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  | 18.10      | Mirhan          |   60            |   60                |
| 2.A  | 18.10      |  Mirhan          |   20             |   30                |
| 3.A  | 18.10      |  Mirhan          |    45           |      45             |
| 4.A  |  18.10     |  Mirhan          |    60           |        60           |
| 5.A  |  25.10     |   Lukas        |     45          |        50           |
| 6.A  |  25.10     |  Mirhan          |    45           |      55             |
| 7.A  |  25.10     |  Mirhan          |    45           |      45             |
| 8.A  |  25.10     |   Mirhan         |    50           |      50             |
| 9.A  |  25.10     |   Mirhan         |   50            |     45              |
| 10.A  | 25.10      |  Lukas         |    45           |      55             |
|10.B    |25.10    |   Lukas         |     45             |    60   Angefangen     |
| 11.A  | 1.11      |  Lukas         |     45          |       45            |
| 12.A  | 1.11      |   Mirhan        |    45           |        45           |
| 13.A  | 1.11      |  Lukas         |     45          |         40          |
|14.A|1.11          | Lukas         |        45        |       55    Angefangen       |
| 14.B  | 1.11      |  Lukas         |    60           |       70    Angefangen        |
| 15.A | 1.11      |    Lukas       |    45           |       55            |
| 16.A  | 1.11      |   Lukas        |    45           |       55            |
| 17A  | 1.11      |  Lukas/Mirhan         |    120           |       180      |



## 5 Kontrollieren

| TC-№ | Datum | Resultat | Tester | Testumgebung|
| ---- | ----- | -------- | ------ | -------|
| 1.1  | 1.11.23 | funktioniert         |  Lukas      | Klassenzimmer|
| 2.1  | 1.11.23 | funktioniert         |  Lukas      | Klassenzimmer|
| 3.1  | 1.11.23 | funktioniert nicht       |  Lukas      | Klassenzimmer|
| 4.1  | 1.11.23 | korrekt         |  Lukas      | Klassenzimmer|
| 5.1  | 1.11.23 | funktioniert         |  Lukas      | Klassenzimmer|
| 6.1  | 1.11.23 | korrekt         |  Lukas      | Klassenzimmer|
| 7.1  | 1.11.23 | funktioniert         |  Lukas      | Klassenzimmer|
| 8.1  | 1.11.23 | nicht vorhanden      |  Lukas      | Klassenzimmer|
| 9.1  | 1.11.23 | funktioniert nicht         |  Lukas      | Klassenzimmer|
| 10.1  | 1.11.23 | funktioniert         |  Lukas      | Klassenzimmer|


## Fazit
Wir sind sehr zufrieden mit unserem Projekt, jedoch konnten wir nicht alles umsetzen, da wir uns zuerst mit Unity vertraut machen mussten. Jedoch würden wir sagen, dass unser Spiel spielbar ist auch wenn es nicht 100% fertig ist.





