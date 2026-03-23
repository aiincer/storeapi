# bios
- ./assets/bios.json
- Inhalt:
```
- "name"      - str   - der name des ordners für das speichern von inhalten für die App
- "test-mode" - bol:1 - ob die app im entwiklungsmodus ist
```
# app-übersicht
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
  - "code" - lst:2 - position des Codes
    - 0    - bol   - ist es vorinstalliert (-> im ./assets folder)
    - 1    - str   - der Name der Datei
```
