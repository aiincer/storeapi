# lokal
## bios
- ./assets/bios.json
- Inhalt:
```
- "name"      - str   - der name des ordners für das speichern von inhalten für die App
- "test-mode" - bol:1 - ob die app im entwiklungsmodus ist
```
## app-übersicht
- /db/apps.json
- Inhalt:
```
- <name>   - jso   - Übersicht über ein Programm (<name>)
  - "pos"  - lst:2 - Position (Ursprung  bei 0)
    - 0    - int   - X-Position
    - 1    - int   - Y-Position
  - "name" - str   - Name der App
  - "pic"  - lst:2 - position des Bildes
    - 0    - bol   - ist es vorinstalliert (-> im ./assets folder)
    - 1    - str   - der Name der Datei
  - "code" - str   - position des Codes
```

# online
## apps
- ~web/db/apps.json
- Inhalt:
```
- <name>             - jso  - Übersicht über ein Programm (<name>)
  - "card"           - jso  - die Karte der app
    - "title"        - str  - der anzeige-name der app
    - "sub-title"    - str  - die beschreibung der app
    - "icon"         - jso  - das icon der app
      - "text"       - str  - die Buchstaben auf dem logo
      - "bg-color"   - str+ - (+: hex) Hintergrungfarbe
      - "txt-clolor" - str+ - (+: hex) Schriftfarbe
    - "code"         - str+ - (+: url) der link zum code
    - "pic"          - str+ - (+: url -> png) der link zum Bild der App
    - "data"         - jso  - inhalt von app-übersicht mit *1
```

# inhalte
## apps..data
```
{
  <name>: {
    "pos": [0, 0],
    "name" : <name>,
    "pic": [false, "<name>.png"],
    "code": "code/<name>/<name>.py"
  }
}
```
