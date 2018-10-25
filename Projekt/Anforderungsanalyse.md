### Anforderungsanalyse

#### Funktionale Anforderungen

##### Allgemein

- Fragebogen zum ausfüllen für Sachverständiger, Baugewerbe und Bauindustrien im Bezug auf Schadensdaten für das Institut für Bauforschung
- Abspeichern der Daten in einer Datenbank und anschließende Überführung in eine Excel-Datei



##### Eingabe-/Bedienelemente

- Checkbox (hauptsächliches Eingabeelement)
- Textfelder
- Schieberegler
- Buttons zum wechseln der Seiten und zum Starten/Absenden des Fragebogens



##### Navigation

- Dem User sollte es möglich sein die letzte Seite nochmal aufzurufen um Verbesserungen vorzunehmen



##### Hilfe

- Bei manchen Fragen wäre es hilfreich eine Funktion zu haben um kurz Informationen zur Beantwortung der jeweiligen Frage anzuzeigen



#### Nichtfunktionale Anforderungen

- einfache Gestaltung, intuitiv nutzbar
- schnelle Erledigung des Fragebogens (5 bis 10 Minuten)
- User muss sich nur um das Ausfüllen des Fragebogens kümmern, Daten werden direkt in Datenbank gespeichert
- Datenbankanbindung



#### Detailbeschreibung

##### Webanwendung

- Desktopversion

##### Datenbank

- PostgreSQL

##### Server

- FH-Server

##### Seitenaufbau

Es gibt zunächst eine Seite die mit Informationen zu dem Fragebogen gefüllt ist, das heißt welchen Zweck dieser erfüllt und wie viel Zeit die Bearbeitung in Anspruch nehmen wird. Am Ende enthält die Seite dann einen "Starten"-Button, welcher einen dann zu der eigentlichen Bearbeitung weiterleitet. (siehe Abbildung)



![Startseite](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/Startseite.png)



Der Fragebogen an sich ist dann so strukturiert dass die Fragen in Kategorien eingeordnet sind und eine Seite dann eine Kategorie mit den jeweiligen Fragen beinhaltet. Die Kategorie steht oben links auf der Seite und die Fragen werden dann untereinander mit den Antwortmöglichkeiten abgebildet. Gegenüber von der Kategorie gibt es noch eine Fortschrittsanzeige, damit der User immer weiß wie viel er noch bearbeiten muss. Abschließend enthält die Seite unten links einen Button "Zurück" um die letzte Seite nochmal aufzurufen und einen Button "Weiter" unten rechts um auf die nächste Seite zu springen beziehungsweise "Absenden" wenn man die letzte Seite erreicht hat und bereit ist den Fragebogen abzuschicken. (siehe Abbildung)



![FragebogenMockup](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/FragebogenMockup.png)



##### Funktionale Anforderungen



###### Aktivitätsdiagramm

![Aktivitätsdiagramm](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/Aktivit%C3%A4tsdiagramm.png)

###### Use-Case Diagramm

![UseCaseDiagram](https://raw.githubusercontent.com/WebEngineering18/Dokumentation/Anforderungsanalyse/Projekt/bilder/UseCaseDiagram.png)

###### Use-Case

![UseCase](F:\Info\GitHub\WebEngineering\Dokumentation\Projekt\bilder\UseCase.png)

![UseCaseRelatedInformation](F:\Info\GitHub\WebEngineering\Dokumentation\Projekt\bilder\UseCaseRelatedInformation.png)