Das Skript template.py ist für python3 geschrieben.
  es werden zusätzlich pakete benötigt:
     python3-ezodf (https://bitbucket.org/mozman/ezodf/overview)
     python3-lxml
  
  lxml kann über die paketquellen oder pip geladen werden
  
  ezodf kann über pip geladen werden (pip install ezodf) oder via hand von bitbucket geladen und installiert werden
  
  bei beiden ist darauf zu achten, dass die installation sich auf die aktuelle python variante bezieht und ins richtige verzeichnis installiert wurde  

1. Verändern der arbeitskreis.ods
  ja wie man so ein ods halt editiert (speichern nicht vergessen)

2. Ausführen von template.py
  Befehl: python3.X template.py bzw. python template.py

3. commit
  Befehl: git commit -am 'aussagekräftiger text zur veränderung'
  
4. push
  Befehl: git push origin gh-pages
  Dann BenutzerInnen-Name + Passwort eingeben
  
Alternativ kann man das Ganze automatisieren:

#!/bin/sh

cd /pfad/zur/psyfako-app/template && python template.py && git commit -am 'aussagekräftiger text zur veränderung' &


Dann noch Befehl 4 anhängen...
