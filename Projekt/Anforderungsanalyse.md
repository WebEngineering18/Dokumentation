### Anforderungsanalyse

#### Funktionale Anforderungen

##### Allgemein

- Der Fragebogen dient zum Ausfüllen für Sachverständiger, Baugewerbe und Bauindustrien im Bezug auf Schadensdaten für das Institut für Bauforschung.
- Die Daten werden anschließend in einer Datenbank gespeichert und hinterher sollen diese auch in eine Excel-Datei überführt werden.



##### Eingabe-/Bedienelemente

- Checkbox (hauptsächliches Eingabeelement)
- Textfelder
- Schieberegler
- Buttons zum Wechseln der Seiten und zum Starten/Absenden des Fragebogens.



##### Navigation

- Dem User sollte es möglich sein, die letzte Seite nochmal aufzurufen, um Verbesserungen vorzunehmen.
- Natürlich gibt es auch einen Button, um die nächste Seite aufzurufen.



##### Hilfe

- Bei manchen Fragen wäre es hilfreich, eine Funktion zu haben, um kurz Informationen zur Beantwortung der jeweiligen Frage anzuzeigen

##### Datenbank

##### Server

##### Authentifizierung

- Das System muss erkennen können, ob ein User den Fragebogen schon einmal ausgefüllt hat, damit dieser den Fragebogen kein zweites Mal bearbeiten darf.



#### Nichtfunktionale Anforderungen

- Die Seite soll einfach gestaltet und intuitiv nutzbar sein.
- Die Erledigung des Fragebogens sollte nicht viel Zeit in Anspruch nehmen (10 - 15 Minuten).



#### Detailbeschreibung

##### Webanwendung

- Die Anwendung muss über alle gängigen Browser (Chrome, Firefox, Safari) darstellbar sein.

##### Datenbank

- Die Datenbank wird in PostgreSQL realisiert.

##### Server

- Der Fragebogen muss am Ende über den FH-Server laufen.

##### Seitenaufbau

Es gibt zunächst eine Seite die mit Informationen zu dem Fragebogen gefüllt ist, das heißt welchen Zweck dieser erfüllt und wie viel Zeit die Bearbeitung in Anspruch nehmen wird. Am Ende enthält die Seite dann einen "Starten"-Button, welcher einen dann zu der eigentlichen Bearbeitung weiterleitet (siehe Abbildung). 



![Startseite](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/Startseite.png)



Der Fragebogen an sich ist dann so strukturiert, dass die Fragen in Kategorien eingeordnet sind und eine Seite dann eine Kategorie mit den jeweiligen Fragen beinhaltet. Die Kategorie steht oben links auf der Seite und die Fragen werden dann untereinander mit den Antwortmöglichkeiten abgebildet. Gegenüber von der Kategorie gibt es noch eine Fortschrittsanzeige, damit der User immer weiß wie viel er noch bearbeiten muss. Abschließend enthält die Seite unten links einen Button "Zurück", um die letzte Seite nochmal aufzurufen und einen Button "Weiter" unten rechts, um auf die nächste Seite zu springen beziehungsweise "Absenden", wenn man die letzte Seite erreicht hat und bereit ist den Fragebogen abzuschicken. (siehe Abbildung)



![FragebogenMockup](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/FragebogenMockup.png)



##### Funktionale Anforderungen



###### Aktivitätsdiagramm

![Aktivitätsdiagramm](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/Aktivit%C3%A4tsdiagramm.png)

###### Use-Case Diagramm

![UseCaseDiagram](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/UseCaseDiagram.png)

![SystemUseCase](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/SystemUseCase.png)

###### Use-Case

![UseCase](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/UseCase.png)

![UseCaseRelatedInformation](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/UseCaseRelatedInformation.png)

#### Komponentendiagramm

![Component Diagram](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/Component%20Diagram.png)

#### User Stories

###### Informationen erhalten

- Als User möchte ich zu Beginn Informationen zu dem Fragebogen erhalten, damit ich weiß welchen Zweck dieser erfüllt.

###### Fragebogen starten

- Als User möchte ich den Fragebogen über einen Button starten können, um diesen ausfüllen zu können.



###### Fragebogen bearbeiten

- Als User möchte ich den Fragebogen über Bedienelemente ausfüllen, um an der Befragung zum Status der Bauqualität teilnehmen zu können.



###### Fragebogen abschicken

- Als User möchte ich den Fragebogen absenden können, um die Daten dem IFB zu übermitteln.



###### Hilfe anzeigen

- Als User möchte ich zu einigen Fragen Information erhalten, um die richtigen Antworten abzugeben.
- Als User möchte ich meinen Fortschritt immer im Blick haben, damit ich weiß wie viele Fragen noch zu bearbeiten sind.



###### Zwischen den Seiten navigieren

- Als User sollte es mir möglich sein die letzte Seite nochmal aufzurufen, falls ich falsche Eingaben getätigt habe.
- Als User möchte ich auf die nächste Seite springen, wenn ich die aktuelle Seite komplett bearbeitet habe.





