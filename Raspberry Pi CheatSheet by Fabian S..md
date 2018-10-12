Raspberry Pi CheatSheet by Fabian S.

Grundlegende Befehle
User/Rechte
System
LAMP/Webservice
Python



Linux Version
→ `cat /proc/version`

Raspberry Pi Version
→`cat /proc/device-tree/model`

Raspberry CPU Temp
→`vcgencmd measure_temp`

Texteditor Nano
→ `nano [Name.xx]`

Verzeichnis wechseln
→ `cd <Pfad>`

Homeverzeichnis mit einem Befehl
→ `cd ..`

Ordner anlegen
→ `mkdir <Name>`

Ordner löschen (if leer)
→ `rm -d <Ordnername>`

Datei löschen
→ `rm <Dateiname>`

Ordernstruktur anzeigen
→ `ls`

Python Script starten
→ `python <Name.py>`

Python installieren
→ `apt-get install python-dev`

Python Version checken
→ `python --version`

Datei Downloaden
→ `wget <link>`

IP Info/Netzwerk
→ `ifconfig`/`iwconfig`

Hostname anzeigen
→ `hostname`

Hostname ändern
→ `nano /etc/hostname`

USB Schnittstellen anzeigen
→ `lsusb`

Raspberry Config (Camera/Mount)
→ `raspi-config`

Reboot
→ `reboot`

Shutdown
→ `shutdown -h now`

Raspberry Pi Headless
Wenn das System auf der SD Karte ist, werden 2 Dateien in das root Verzeichnis der SD Karte verschoben.

Datei 1: ssh.dat
→ Einfach eine leere Datei, für den SSH Zugriff

Datei 2: wpa_supplicant.conf
→ Sie regelt das mit dem W-Lan

    country=DE 
    ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
    update_config=1
    network={
        ssid="Wlan SSID"
        psk="Passwort"
        key_mgmt=WPA-PSK
        }

Python PIP installation
→ `apt-get install python-pip`

Gits von Github clonen
install:
→ `apt-get install git`
clonen:
→ `git clone git://github.com/ ... .git`

Python Scripte abbrechen
→ `STRG + C`

Screen

Installieren
→ `apt-get install screen`

Session starten
→`screen bash`

Session beenden
→`STRG + D`

Session verlassen
→ `STRG + A und D`

Auflistung der Sessions
→ `screen -list`

Session reconnect
→ `screen -r ... <listennummer>`

Statische IP hinzufügen

→ `sudo ifconfig`
Um zu schauen, welche Internetschnittstelle vorhanden ist eth0 or ENX

→ `sudo nano /etc/dhcpd.conf`

Dort wird dieser Text geändert oder die # Zeichen weg 







