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
- Fachliches Ziel: ?
- Auslöser: Aufruf durch ein anderen Use-Case
- Akteure: /
- Vorbedingung: /
- Nachbedingung: ?
- Verwendete Informationen: Anleitung.Ersteller, Benutzer
- Ergebnis: Verhindert, das der Ersteller einer Anleitung, mit dem angegebenen Benutzer identisch ist.
- Verbindungen: Anleitung freigeben

### Ablauf
Der Use-Case bekommt eine Anleitung und einen Benutzer, er überprüft ob der Ersteller der Anleitung mit dem angegebenen Benutzer Identisch ist. Ist dies der Fall, wird "false" zurückgegeben, falls nicht wird "true" zurückgegeben.

### Kurzbeschreibung
Dieser Use-Case prüft, ob beim freigeben eines Produktes das 4 Augen Prizip gewart wird, also das eine Freigabe nicht vom Uploader erteilt wird.

Dieser Use-Case erfüllt eine unterstüzende Funktion für andere Use-Cases, um zu entscheiden, ob eine bestimmte Transaktion genemigt werden darf.

## Sichtbarkeit feststellen
- Fachliches Ziel: ?
- Auslöser: Aufruf durch ein anderen Use-Case
- Vorbedinung: /
- Nachbedingung: ?
- Verwendete Informationen: Fachprüfer.Produkt ODER Sprachprüfer.Sprache ODER Übersetzer.Sprach_Land_Kombination, Anleitung.Sprach_Land_Kombination, Anleitung.Sprach_Land_Kombination.Sprache, Produkt.Anleitung
- Ergebnis: Akteure erhalten nur Zugriff auf Anleitungen, für die sie eine Berechtigung haben.
- Verbindungen: Anleitung Zurückweisen, Freizugebende Anleitungen anzeigen, Produktstatus anzeigen, Anleitung hochladen, Anleitung freigeben

### Ablauf
Der Use-Case bekommt eine Rolle und eine Anleitung gegeben und Überprüft ob die Rolle Zugriff auf die Anleitung hat.

Ist die Rolle ein Übersetzer, wird die Sprach-Land-Kombination des Übersetzers mit der der Anleitung verglichen. Ist diese identisch wird der Zugriff gewärt. Ist diese nicht identisch wird der Zugriff verweigert. 

Ist die Rolle ein Fachprüfer, wird das Produkt des Fachprüfers mit dem Produkt, dem die Anleitung zugewiesen ist verglichen. Ist dieses identisch wird der Zugriff gewärt. Ist dieses nicht identisch wird der Zugriff verweigert. 

Ist die Rolle ein Sprachprüfer, wird die Sprache des Sprachprüfers mit der Sprache der Anleitung verglichen. Ist diese identisch wird der Zugriff gewärt. Ist diese nicht identisch wird der Zugriff verweigert. 

### Kurzbeschreibung
Dieser Use-Case soll sicherstellen, dass Benutzer nur auf Anleitungen zufreifen können, für welche sie zuvor implizit freigegeben wurden. Diese hängt unter anderem von zugewiesenem Land, Sprache und Produkt ab.

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

## Freizugebende Anleitungen anzeigen
- Fachliches Ziel: ?
- Auslöser: Aufruf durch einen Prüfer
- Akteure: Fachprüfer, Sachprüfer
- Vorbedingung: /
- Nachbedingung: ?
- Verwendete Informationen: Sprachprüfer.Sprache ODER Fachprüfer.Produkt, Anleitung.Sprach_Land_Kombination.Sprache, Produkt.Anleitung, Anleitung.sprachlicheFreigabe, Anleitung.technischeFreigabe
- Ergebnis: Alle Anleitungen, welche der Prüfer prüfen darf werden angezeigt
- Verbindungen: 4 Augen Prinzip Prüfen, Sichtbarkeit feststellen

### Ablauf
Ist der Prüfer ein Fachprüfer, wird sein zu Prüfendes Produkt ermittelt. Dann werden alle Anleitungen für dieses Produkt ermittelt und die Anleitungen ausgewählt, welche noch kein Ergebnis einer Fachprüfung haben (also kein Freigabe- oder Zurückweisungsobjekt hinterlegt wurde). Dann werden alle Anleitungen wo, dies der Fall ist dem Fachprüfer präsentiert.

Ist der Prüfer ein Sprachprüfer, werden alle Produkte nach Anleitungen in der Sprache des Prüfers durchsucht. Dann werden daraus alle Anleitungen ermittelt, welche noch kein Ergebnis einer Sprachprüfung haben (also kein Freigabe- oder Zurückweisungsobjekt hinterlegt wurde). Dann werden alle Anleitungen wo, dies der Fall ist dem Sprachprüfer präsentiert.

In beiden Fällen gilt, sollten keine Anleitungen vorhanden sein werden auch keine Angezeigt. Stattdessen wird ein Hinweis anzgezeigt, dass es nichts zu Prüfen gibt. 

### Kurzbeschreibung
Ermöglicht das Anzeigen von Anleitungen, welche durch den Prüfer noch freigegeben werden müssen. Bei einem Sprachprüfer sind das Anleitungen mit fehlender sprachlicher Freigabe/Zurückweisung, welche in seiner Sprache verfasst sind. Bei einem Fachprüfer sind das Anleitungen mit fehlender fachlicher Freigabe/Zurückweisung, welche zu seinem Produkt gehören.

## Anleitung freigeben
- Fachliches Ziel: ?
- Auslöser: Prüfer gibt eine Anleitung frei.
- Akteure: Fachprüfer, Sachrüfer
- Vorbedingung: Eine Anleitung wurde von einem Übersetzer Hochgeladen; Die Anleitung ist in der Sprache des Sprachprüfers verfasst oder die Anleitung ist für das Produkt des Fachprüfers verfasst; Die Anleitung darf noch nicht unter derselben Kategorie (Sprache oder Fachlich) geprüft worden sein
- Nachbedingung: ?
- Verwendete Informationen: Anleitung.Sprach_Land_Kombination.Sprache, Produkt.Anleitung, Begründung (Optional), Sprachprüfer.Sprache ODER Fachprüfer.Produkt
- Ergebnis: Die Anleitung hat eine neue Freigabe
- Verbindungen: Begründung Angeben (Optional, wenn der Prüfer eine Begründung angeben will), Sichtbarkeit feststellen

### Ablauf
Der Sprach oder Fachprüfer gibt eine Anleitung an, die er Freigeben will, außerdem kann er eine Begründung angeben. Mit dem Verweis auf die Anleitung und den Prüfer wird "Sichtbarkeit Prüfen" ausgeführt. Ist der Prüfer nicht berechtigt, diese Anleitung zu Prüfen wird ein Fehler geworfen und der Vorgang abgebrochen. Ist der Prüfer aber berechtigt eine Bewertung vorzunehmen, wird ein Freigabeobjekt mit generiert, welches entweder die Begründung oder den Wert "null" enthällt und ein Verweis in dem Anleitungsobjekt hinterlegt. Ob hier die Fachliche oder Sprachliche Freigabe angehängt wird, hängt von der Rolle des Prüfers ab. 

Sollte die angegebene Anleitung nicht mehr existieren wird ein Fehler geworfen und keine Änderung vorgenommen. Sollte die Anleitung bereits in dieser Kategroie (Fachlich/Sprachlich) Geprüft worden sein wird ebenfalls ein Fehler geworfen.

### Kurzbeschreibung
Ermöglicht das sprachliche/fachliche Freigeben einer Anleitung. Optional kann hier eine Begründung angefügt werden.

## Anleitung zurückweisen
- Fachliches Ziel: ?
- Auslöser: Prüfer weist eine Anleitung zurück.
- Akteure: Fachprüfer, Sachrüfer
- Vorbedingung: Eine Anleitung wurde von einem Übersetzer Hochgeladen; Die Anleitung ist in der Sprache des Sprachprüfers verfasst oder die Anleitung ist für das Produkt des Fachprüfers verfasst; Die Anleitung darf noch nicht unter derselben Kategorie (Sprache oder Fachlich) geprüft worden sein
- Nachbedingung: ?
- Verwendete Informationen: Anleitung.Sprach_Land_Kombination.Sprache, Produkt.Anleitung, Begründung, Sprachprüfer.Sprache ODER Fachprüfer.Produkt
- Ergebnis: Die Anleitung hat eine neue Zurückweisung
- Verbindungen: Begründung Angeben, Sichtbarkeit feststellen

### Ablauf
Der Sprach oder Fachprüfer gibt eine Anleitung an, die er Zurückweisen will, außerdem gibt er eine Begründung an. Mit dem Verweis auf die Anleitung und den Prüfer wird "Sichtbarkeit Prüfen" ausgeführt. Ist der Prüfer nicht berechtigt, diese Anleitung zu Prüfen wird ein Fehler geworfen und der Vorgang abgebrochen. Ist der Prüfer aber berechtigt eine Bewertung vorzunehmen, wird ein Zurückweisungsobjekt mit der Begründung generiert und ein Verweis in dem Anleitungsobjekt hinterlegt. Ob hier die Fachliche oder Sprachliche Zurückweisung angehängt wird, hängt von der Rolle des Prüfers ab. 

Sollte die angegebene Anleitung nicht mehr existieren oder sollte keine Begründung angegeben worden sein, wird ein Fehler geworfen und keine Änderung vorgenommen. Sollte die Anleitung bereits in dieser Kategroie (Fachlich/Sprachlich) Geprüft worden sein wird ebenfalls ein Fehler geworfen.

### Kurzbeschreibung
Ermöglicht das sprachliche/fachliche Zurückweisen einer Anleitung. Zwingend muss hier eine Begründung angefügt werden.

## Begründung angeben
- Fachliches Ziel: ?
- Auslöser: Aufruf durch ein anderen Use-Case
- Akteure: /
- Vorbedingung: /
- Nachbedingung: ?
- Verwendete Informationen: Zeichenkette
- Ergebnis: Es wurde ein Begründungsstring erzeugt.
- Verbindung: Anleitung freigeben, Anleitung zurückweisen

### Ablauf
Die Eingaben des Prüfers werden entegegengenommen und in einen String geschreiben, welcher zurückgegeben wird. Sollten keine Eingabe stattfinden wird ein Fehler geworfen.

### Kurzbeschreibung
Ermöglicht das formulieren einer Begründung für eine Zurückweisung oder Freigabe.
