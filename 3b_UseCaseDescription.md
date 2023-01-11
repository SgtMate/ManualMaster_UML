# admin

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

## übersetzungLöschen

Übersetzungen könne gelöscht werden.
Das kann allerdings nicht geschehen, wenn die Übersetzung final
und Teil eines gesperrten Produkts ist.

## produktLöschen

Produkte können gelöscht werden.
Das geht allerdings nur, wenn das Produkt nicht gesperrt ist.

# Produkt Manager

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

## fehlendeÜbersetzungenAnzeigen

Produktmanager können sich anzeigen lassen
für welche Produkte noch welche Anleitungen fehlen.

## freigabestatusAnzeigen

Es kann der Freigabestatus für die Produkte angezeigt werden.

# Übersetzer

## fehlendeÜbersetzungenAnzeigen

Übersetzer können sich anzeigen lassen für welche Produkte
noch Übersetzungen in der ihnen zugewiesenen Land-Sprach Kombination fehlen. 

## vorhandeneÜbersetzungenAnzeigen

Es kann angezeigt werden, für welche Produkte
Übersetzungen in der einem Übersetzer zugewiesenen Land-Sprach Kombination vorhanden sind.

## zurückgewieseneÜbersetzungenAnzeigen

Übersetzer können die zurückgewiesenen Übersetzungen,
die sie hochgeladen haben anzeigen.

## anleitungHochladen

Übersetzer können Anleitungen in der ihnen zugeordneten Land-Sprach
Kombination hochladen 

# Sprachprüfer

## freizugebendeAnleitungenAnzeigen
<!--TODO-->
Sprachprüfer können sich Anleitungen in der ihnen zugeordneten Sprache Anzeigen lassen, die noch zu prüfen sind.
### Kurzbeschreibung
### Fachliches Ziel
### Akteure
### Auslöser
### Vorbedingungen
### Nachbedingungen
### verwendete Informationen
### Ablauf
### Abläufe in Ausnahmefällen
### verbundene Anwendungsfälle

## anleitungFreigeben
<!--TODO-->
### Kurzbeschreibung
Sprachprüfer können Anleitungen eine sprachliche Freigabe erteilen.
Wichtig ist dabei, dass Benutzer niemals eine Freigabe für Anleitungen erteilen, die sie selbst hochgeladen haben
### Fachliches Ziel
### Akteure
### Auslöser
### Vorbedingungen
### Nachbedingungen
### verwendete Informationen
### Ablauf
### Abläufe in Ausnahmefällen
### verbundene Anwendungsfälle



## anleitungZurückweisen
<!--TODO-->
### Kurzbeschreibung
Sprachprüfer können Anleitungen eine sprachliche Zurückweisung erteilen.
### Fachliches Ziel
### Akteure
### Auslöser
### Vorbedingungen
### Nachbedingungen
### verwendete Informationen
### Ablauf
### Abläufe in Ausnahmefällen
### verbundene Anwendungsfälle



# Fachprüfer
## freizugebendeAnleitungenAnzeigen

Fachprüfer können sich Anleitungen von dem ihnen zugeordneten Produkt Anzeigen lassen, die noch zu prüfen sind.

## anleitungFreigeben
<!--TODO-->

### Kurzbeschreibung
Fachprüfer können Anleitungen eine fachliche Freigabe erteilen.
Wichtig ist dabei, dass Benutzer niemals eine Freigabe für Anleitungen erteilen, die sie selbst hochgeladen haben
### Fachliches Ziel
### Akteure
### Auslöser
### Vorbedingungen
### Nachbedingungen
### verwendete Informationen
### Ablauf
### Abläufe in Ausnahmefällen
### verbundene Anwendungsfälle


## anleitungZurückweisen
<!--TODO-->

### Kurzbeschreibung
Sprachprüfer können Anleitungen eine sprachliche Zurückweisung erteilen.
### Fachliches Ziel
### Akteure
### Auslöser
### Vorbedingungen
### Nachbedingungen
### verwendete Informationen
### Ablauf
### Abläufe in Ausnahmefällen
### verbundene Anwendungsfälle
