# Beschreibung der Use-Cases

## Sprache bearbeiten

### Kurzbeschreibung
Ermögicht das Pflegen aller, auf eine Sprache bezogene Parameter, wie z.B. die Bezeichnung.

## Land und Sprache Zuordnen

### Kurzbeschreibung
Ermöglicht es Kombinationen aus Land und Sprache zu erstellen, welche dann den Übersetzern zugewiesen werden.

## Bericht erzeugen

### Kurzbeschreibung
Ermöglicht das Erzeugen eines Berichtes zu einem bestimmten Produkt. Der Bericht enthällt, welcher Benutzer welche Anleitungen hochgeladen hat und welcher Benutzer welche Sperre/Freigabe veranlasst hat.

## Land anlegen

### Kurzbeschreibung
Ermöglicht das erstellen eines Landes im System, jedes Land hat dabei eine Bezeichnung.

## Land bearbeiten

### Kurzbeschreibung
Ermöglicht das Pflegen aller, auf ein Land bezogene Parameter, wie z.B. die Bezeichnung.

## Sprache anlegen

### Kurzbeschreibung
Ermöglicht das erstellen einer Sprache im System, jede Sprache hat dabei eine eigene Bezeichnung.

## Produktstatus feststellen

### Kurzbeschreibung
Dieser Use-Case überprüft ob ein gegebenes Produkt von einem Produkt Manager gesprerrt wurde.

Dieser Use-Case erfüllt eine unterstüzende Funktion für andere Use-Cases, um zu entscheiden, ob eine bestimmte Transaktion genemigt werden darf.

## Anleitungsstatus feststellen

### Kurzbeschreibung
Dieser Use-Case überprüft ob eine gegebene Anleitung vollständig freigegeben wurde und somit als Final gilt.

Dieser Use-Case erfüllt eine unterstüzende Funktion für andere Use-Cases, um zu entscheiden, ob eine bestimmte Transaktion genemigt werden darf.

## Anleitung löschen

### Kurzbeschreibung
Ermöglicht das Löschen einer Anleitung aus dem System. Hierbei werden auch die Freigaben und Zurückweisungen der Anleitung mitgelöscht. Das Löschen ist nur möglich wenn die Anleitung nicht Final und nicht Teil eines gesperrten Produktes ist!

## Produkt löschen

### Kurzbeschreibung
Ermöglicht das Löschen eines Produktes aus dem System. Hierbei werden alle Anleitungen des Produktes mitgelöscht (falls welche vorhanden sind). Produkte können nur gelöscht werden, wenn diese nicht gesperrt sind.


