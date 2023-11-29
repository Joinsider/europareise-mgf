Europareise
======================

Hier gibt es eine Online Variante des Brettspiels Europareise<br>
This contains an online version of the board game Journey through Europe

------------
Diese App erstellt einen Flask (Python) Webserver

Um die App auszuführen, muss Python installiert und eine virtual environment aktiviert sein


```
pip install -r requirements.txt
cd src
python server.py
```
Das Spiel ist dann auf dem lokalen PC via port 5100 aufrufbar<br>
Um das Spiel auch im Netzwerk spielbar zu machen muss der Port in der Windows Firewall geöffnet werden

Als Alternative gibt es ein Dockerfile, womit ein Docker Container erstellt werden kann.<br>
Dieser führt den gleichen Code aus, jedoch nutzt dieser zusätzlich ein Shell Skript, 
um die alten, unbenutzten Spiele (älter als 3 Stunden) zu löschen
<br><br>
Für die Docker Instalation:

```
docker build -t jte .
docker run -d -p 5100:5100 jte
```
