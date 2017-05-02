# ZON-Kommentarsuche
Durchsuche Kommentare eines Benutzers auf ZON

## Beschreibung

Diese Webapplikation für Chrome/Chromium durchsucht die Kommentare eines Benutzers der [ZEIT Online](http://www.zeit.de/index) nach einem Suchbegriff. Weglassen des Suchbegriffes zeigt alle Kommentare des Benutzers an. 

## Benutzung
Diese Webapplikation benutzt [CORS](https://de.wikipedia.org/wiki/Cross-Origin_Resource_Sharing) zum Abrufen der Kommentare. Daher muss die Restriktion des Browsers umgangen werden:

#### Chrome unter Windows:
    "C:\PathTo\Chrome.exe" --allow-file-access-from-files --user-data-dir --disable-web-security
    
#### Chrome unter Linux / MacOSX:
    chrome --allow-file-access-from-files --user-data-dir --disable-web-security
    
#### Chromium unter Linux / MacOSX:
    chromium --allow-file-access-from-files --user-data-dir --disable-web-security
