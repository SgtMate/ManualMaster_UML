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

## Anleitung hochladen

### Kurzbeschreibung
Ermöglicht das Hochladen einer Anleitung für ein bestimmtes (nicht gesperrtes) Produkt in einer bestimmten Land-Sprach-Kombination. Sollte bereits eine Anleitung hochgeladen worden sein, wird die alte Anleitung mit ihren Freigaben und Zurückweisungen gelöscht. Anleitungen dürfen nur von übersetztern in derseleben Land-Sprach-Kombination hochgeladen werden.

## 4 Augen Prinzip prüfen
> TODO: Ausbauen, da in Konzext zu Prüfern
### Kurzbeschreibung
Dieser Use-Case prüft, ob beim freigeben eines Produktes das 4 Augen Prizip gewart wird, also das eine Freigabe nicht vom Uploader erteilt wird.

Dieser Use-Case erfüllt eine unterstüzende Funktion für andere Use-Cases, um zu entscheiden, ob eine bestimmte Transaktion genemigt werden darf.

## Sichtbarkeit feststellen
> TODO: Ausbauen, da in Konzext zu Prüfern
### Kurzbeschreibung
Dieser Use-Case soll sicherstellen, dass Benutzer nur auf Systemobjekte (Anleitungen, Produkte), für welche sie zuvor implizit freigegeben wurden. Diese hängt unter anderem von zugewiesenem Land, Sprache und Produkt ab.

Dieser Use-Case erfüllt eine unterstüzende Funktion für andere Use-Cases, um zu entscheiden, welche Transaktionen und Anfragen genemigt werden dürfen.

## Begründung anzeigen

### Kurzbeschreibung
Dieser Usecase zeigt dem Benutzer die Begründungen für eine Freigabe oder Zurückweisung an, falls eine vorhanden ist.

## Produktstatus Anzeigen

### Kurzbeschreibung
Ermöglicht das Anzeigen welche Produkte in einer gegebenen Land-Sprach-Kombination über eine Anleitungsübersetzung verfügen und wie diese fehlt.

## Zurückgewiesene Anleitungen anzeigen

### Kurzbeschreibung
Ermlöglicht den Übersetzern das Anzeigen von Anleitungen, welche von ihnen verfasst wurden und von einem Prüfer zurückgewiesen wurden. Dabei wird auch die Begründung angezeigt. 

## Produkt sperren

### Kurzbeschreibung
Ermöglicht das Erstellen einer Produktsperre. Gesperrte Produkte können nicht gelöscht werden und das erneute Hochladen von finalen Anleitungen wird unterbunden. 

## Produkt entsperren

### Kurzbeschreibung
Ermöglicht das entsperren eines zuvor gesperrten Produktes. Nur derselbe Produkt Manager, der das Produkt gesperrt hat kann es wieder Entsperren.

## Produkt anlegen

### Kurzbeschreibung
Ermöglicht das einpflegen eines Produktes im System, jedes Produkt hat dabei eine Bezeichnung.

## Produkt bearbeiten

### Kurzbeschreibung
Ermöglicht das Pflegen aller, auf ein Produkt bezogene Parameter, wie z.B. die Bezeichnung.

## Produktübersicht anzeigen

### Kurzbeschreibung
Zeigt an für welche Produkte Anleitungen vorliegen und wie der Freigabestatus dieser Anleitungen ist.


