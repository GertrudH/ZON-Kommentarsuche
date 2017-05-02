# ZON-Kommentarsuche
Durchsuche Kommentare eines Benutzers auf ZON

## Beschreibung

Diese Webapplikation durchsucht die Kommentare eines Benutzers der [ZEIT Online](http://www.zeit.de/index) nach einem Suchbegriff. Weglassen des Suchbegriffes zeigt alle Kommentare des Benutzers an. 

## Benutzung
Diese Webapplikation benutzt [CORS](https://de.wikipedia.org/wiki/Cross-Origin_Resource_Sharing) zum Abrufen der Kommentare. Daher muss die Restriktion des Browsers umgangen werden. Dies geht entweder durch einen Parameter beim Starten des Browsers (Chrome/Cromium), oder durch den Betrieb eines Webservers.

### Parameter (Chrome, Chromium)

#### Chrome unter Windows:
    "C:\PathTo\Chrome.exe" --allow-file-access-from-files
    
#### Chrome unter Linux / MacOSX:
    chrome --allow-file-access-from-files
    
#### Chromium unter Linux / MacOSX:
    chromium --allow-file-access-from-files
    
### Webserver

Hierzu muss man erst in das Verzeichnis wechseln, in dem die index.html liegt. Je nach installierter Programmiersprache/Umgebung kann man den Server dann folgendermassen starten:

#### Python
    python -m SimpleHTTPServer
    
URL:
    http://localhost:8000
    
#### Python 3
    python3 -m http.server
    
URL:
    http://localhost:8000
    
#### Node.js
Server installieren:
    npm install -g http-server
    
Server ausführen:
    http-server -c-1
    
URL:
    http://localhost:8080
    
#### Ruby
    ruby -run -e httpd . -p 8080

URL:
    http://localhost:8080
    
#### PHP
    php -S localhost:8000
    
URL:
    http://localhost:8000
    
#### PIKE
    pike -x httpserver
    
URL:
    http://localhost:8080
