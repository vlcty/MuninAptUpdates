MuninAptUpdates
===============

Monitor how many security and normal updates are pending

Generell
--------

Das Plugin erstellt zwei Graphen: Anzahl Security & Normale Updates, die auf dem Node verfügbar sind.

Das Script ist eigentlich so ausgelegt, dass es ohne root-Rechte auskommt.
Da meines Wissens nach alle Plugins ohne spezieller Konfiguration mit root-Rechten ausgeführt werden ist ein Update der Paketlisten integriert.

Installation
------------

Auf den Munin-Node einloggen, auf dem das Plugin laufen soll.
Danach die 3 Standardschritte ausführen:

1) Kopiere des Script in /usr/share/munin/plugins/
2) Softlink erstellen: ln -s /usr/share/munin/plugins/apt-updates /etc/munin/plugins
3) Service munin-node neustarten: service munin-node restart
