<!--TIMEWASTED: 8h-->

## spracheAnlegen

Ein Administrator kann eine Sprache im System anlegen.
Die Sprache ist von da an für alle anderen Tätigkeiten 
im System verfügbar und kann nicht mehr gelöscht werden.

## landAnlegen

Ein Administrator kann ein Land im System anlegen.
Das Land ist von da an für alle anderen Tätigkeiten 
im System verfügbar und kann nicht mehr gelöscht werden.


## landSpracheZuordnen

Einem Land wird eine Sprache zugeordnet, 
die in diesem Land gesprochen werden.
Das kann mehrfach ausgeführt werden, 
sodass einem Land mehrere Sprachen zugeordnet sein können.
Sobald diese Zuordnung gemacht ist, ist diese Kombination im System vorhanden und kann nicht mehr gelöscht werden.

## benutzerPflegen

Benutzer pflegen beinhaltet das Erstellen von Nutzern,
das Löschen von Nutzern, vergeben von Benutzernamen
und Vergebung von Rollen.
Ein Benutzer kann mehrere Rollen haben.

## berichtErzeugen

es kann ein Bericht erzeugt werden, der beinhaltet,
welcher Benutzer welche Anleitungen hochgeladen hat
und welche Benutzer welche Freigaben und Sperrungen veranlasst haben.

## anleitungLöschen

Anleitungen könne gelöscht werden.
Das kann allerdings nicht geschehen, wenn die Anleitung final
und Teil eines gesperrten Produkts ist.

## produktLöschen

Produkte können gelöscht werden.
Das geht allerdings nur, wenn das Produkt nicht gesperrt ist.

## produktAnlegen

Produkte können angelegt werden.
Ein Produkt muss immer einen Namen bekommen, wenn es angelegt wird.
Außerdem muss angelegt werden in welchen Ländern das Produkt vertrieben werden soll.

## produktBearbeiten

Ein Produkt kann bearbeitet werden.
Das bedeutet, es können die Länder angepasst werden,
in denen das Produkt vertrieben wird.

## produktSperren

Produkte können gesperrt werden.
Gesperrte Produkte können nicht gelöscht werden,
genauso können Finale Anleitungen für gesperrte Produkte nicht gelöscht werden.
Finale Anleitungen für gesperrte Produkte können auch nicht erneut hochgeladen werden.

## produktSperreAufheben

Eine Sperre für ein Produkt kann durch den Produktmanager,
der die Sperre veranlasst hat, wieder aufgehoben werden.
Alle durch die Sperre eingeschränkten Tätigkeiten
können dann wieder durchgeführt werden.

## fehlendeAnleitungenAnzeigen für Produkte

Produktmanager können sich anzeigen lassen
für welche Produkte noch welche Anleitungen fehlen.

## freigabestatusAnzeigen

Es kann der Freigabestatus für die Produkte angezeigt werden.


## fehlendeAnleitungenAnzeigen für Land-Sprach Kombinationen

Übersetzer können sich anzeigen lassen für welche Produkte
noch Anleitungen in der ihnen zugewiesenen Land-Sprach Kombination fehlen. 

## vorhandeneAnleitungenAnzeigen

Es kann angezeigt werden, für welche Produkte
Anleitungen in der einem Übersetzer zugewiesenen Land-Sprach Kombination vorhanden sind.

## zurückgewieseneAnleitungenAnzeigen

Übersetzer können die zurückgewiesenen Anleitungen,
die sie hochgeladen haben anzeigen.

## anleitungHochladen

Übersetzer können Anleitungen in der ihnen zugeordneten Land-Sprach
Kombination hochladen 

## sprachlich freizugebendeAnleitungenAnzeigen

### Kurzbeschreibung
Sprachprüfer können sich Anleitungen in der ihnen zugeordneten Sprache Anzeigen lassen, die noch zu prüfen sind.
### Fachliches Ziel
Anleitungen Anzeigen
### Akteure
ein Sprachprüfer
### Auslöser
Aufruf durch einen Sprachprüfer
### Vorbedingungen
keine
### Nachbedingungen
keine
### verwendete Informationen
* Alle Anleitungen
* Freigabestati der Anleitungen
* Sprache der Anleitungen
### Ablauf
Es werden alle Anleitungen gesucht die noch keinen
Freigabestatus haben, dann werden diese nach der Sprache des Sprachprüfers gefiltert.
Zuletzt werden die passenden Anleitungen angezeigt
### Abläufe in Ausnahmefällen
keine Angabe
### verbundene Anwendungsfälle
keine

## sprachlich anleitungFreigeben

### Kurzbeschreibung
Sprachprüfer können Anleitungen eine sprachliche Freigabe erteilen.
Wichtig ist dabei, dass Benutzer niemals eine Freigabe für Anleitungen erteilen, die sie selbst hochgeladen haben
### Fachliches Ziel
einer Anleitung den Status sprachtlich Freigegeben zuteilen
### Akteure
Sprachprüfer
### Auslöser
Aufruf der sprachlichen Freigabe durch einen Sprachprüfer 
### Vorbedingungen
* Anleitung muss vorhanden sein
* Sprachprüfer muss Sprache der Anleitung zugeordnet sein.
* die Anleitung darf keine fachliche Zurückweisung haben
* die Anleitung darf nicht schon sprachlich freigegeben sein
### Nachbedingungen
keine
### verwendete Informationen
die freizugebene Anleitung
### Ablauf
es wird der Status SprachlicheFreigabe erstellt und der Anleitung hinzugefügt
### Abläufe in Ausnahmefällen
keine Angabe
### verbundene Anwendungsfälle
keine


## sprachlich anleitungZurückweisen

### Kurzbeschreibung
Sprachprüfer können Anleitungen eine sprachliche Zurückweisung erteilen.
### Fachliches Ziel
einer Anleitung den Status sprachlich Zurückgewiesen zuteilen
### Akteure
Sprachprüfer
### Auslöser
Aufruf der sprachlichen Zurückweisung durch einen Sprachprüfer
### Vorbedingungen
* Anleitung muss vorhanden sein
* Sprachprüfer muss Sprache der Anleitung zugeordnet sein.
* die Anleitung darf nicht schon sprachlich zurückgewiesen sein.
### Nachbedingungen
keine
### verwendete Informationen
die zurückzuweisende Anleitung
### Ablauf
es wird der Status SprachlicheZurückweisung erstellt und der Anleitung hinzugefügt.
### Abläufe in Ausnahmefällen
keine Angabe
### verbundene Anwendungsfälle
keine

## fachlich freizugebendeAnleitungenAnzeigen

Fachprüfer können sich Anleitungen von dem ihnen zugeordneten Produkt Anzeigen lassen, die noch zu prüfen sind.

## anleitungFreigeben

### Kurzbeschreibung
Fachprüfer können Anleitungen eine fachliche Freigabe erteilen.
Wichtig ist dabei, dass Benutzer niemals eine Freigabe für Anleitungen erteilen, die sie selbst hochgeladen haben
### Fachliches Ziel
einer Anleitung den Status fachlich freigegeben zuteilen
### Akteure
Fachprüfer
### Auslöser
Aufruf der fachlichen Freigabe durch den Fachprüfer
### Vorbedingungen
* Anleitung muss vorhanden sein
* Fachprüfer muss dem Produkt, auf das sich die Anleitung bezieht zugeordnet sein.
* die Anleitung darf keine sprachliche Zurückweisung haben
* die Anleitung darf nicht schon fachlich freigegeben sein
### Nachbedingungen
keine
### verwendete Informationen
die freizugebende Anleitung
### Ablauf
es wird der Status FachlicheFreigabe erstellt und der Anleitung hinzugefügt
### Abläufe in Ausnahmefällen
keine angabe
### verbundene Anwendungsfälle
keine

## fachlich anleitungZurückweisen

### Kurzbeschreibung
Fachprüfer können Anleitungen eine fachliche Zurückweisung erteilen.
### Fachliches Ziel
einer Anleitung den Status fachlich Zurückgewiesen zuteilen
### Akteure
Fachprüfer
### Auslöser
Aufruf der fachlichen Zurückweisung durch einen Fachprüfer
### Vorbedingungen
* Anleitung muss vorhanden sein
* Fachprüfer muss dem Produkt, auf das siech die Anleitung bezieht zugeordnet sein.
* die Anleitung darf nicht schon fachlich zurückgewiesen sein.
### Nachbedingungen
keine
### verwendete Informationen
die zurückzuweisende Anleitung
### Ablauf
es wird der Status FachlicheZurückweisung erstellt und der Anleitung hinzugefügt.
### Abläufe in Ausnahmefällen
keine Angabe
### verbundene Anwendungsfälle
keine