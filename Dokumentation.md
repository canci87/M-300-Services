Dokumentation 
=============

### Übersicht
***

* 01 - [GitHub Account](#01---github-account)
* 01.01 - [Synchronistation Lokal -> Online](#0101---synchronisation-lokal---online)
* 01.02 - [Synchronisation Online -> Lokal](#0102---synchronisation-online---lokal)
* 02 - [SSH-Key hinzufügen](#02---SSH-Key-hinzufügen)
* 03 - [Client Konfigurieren](#03---Client-Konfigurieren)
* 04 - [Vagrant Befehle](#04---Vagrant-Befehle)
* 05 - [Vagrant Boxen](#05---Vagrant-Boxen)
* 06 - [Firewall Konfig](#06---firewall-konfig)


### 01 - GitHub Account 
***


1. Git-Bash öffnen
2. Folgenden Befehl mit der Account Mail von GitHub einfügen
      <br>`ssh-keygen -t rsa -b 4096 -C "githubmail"`
3. SSH-Key wird erstellt
      <br>`Generating public/private rsa key pair`
4. Schlüsselname eingeben oder direkt mit Enter bestätigen
      <br>`Enter a file in which to save the key (~/.ssh/id_rsa): [Press Enter]`
5. Nun wird ein Passwort für den Key festgelegt
      <br>`Enter passphrase (empty for no passphrase):`
      <br>`Enter same passphrase again:`


### 01.01 - Synchronisation Lokal -> Online
***


1. Git-Bash öffnen
2. Ins Verzechniss wechseln welches gesynct werden soll
3. Folgende Befehl eingeben
      <br>`git add -A`
      <br>`git commit -m "Kommentar"`
      <br>`git push`
4. Synchronisation erfolgreich


### 01.02 - Synchronisation Online -> Lokal
***

1. Git-Bash öffnen
2. Folgenden Befehl eingeben
      <br>`git pull`
3. Synchronisation Erfolgreich


1. Git-Bash öffnen
2. Ins Verzechniss wechseln welches gesynct werden soll
3. Folgende Befehl eingeben
      <br>`git add -A`
      <br>`git commit -m "Kommentar"`
      <br>`git push`
4. Synchronisation erfolgreich

### 02 - SSH Key hinzufügen
***


1. Auf www.github.com anmelden
2. Zu den Einstellungen wechseln
3. Bei den "personal settings" zu "SSH und GPG keys" wechseln
4. Unter "title" eine Bezeichnung angeben (z.B. EC_SSH_Key)
5. Datei "%HOME%/.ssh/id_rsa.pub" oder "$HOME/.ssh/id_rsa.pub" in Zwischenablage kopieren
6. Den Code auf GitHub einfügen und auf "Add SSH key" klicken
7. Der Schlüssel taucht nun in der übergeordneten Liste auf


### 03 - Client konfigurieren
***


1. Git-Bash öffnen
2. Git konfigurieren mit GitHub Account
      <br>`git config --global user.name "username"`
      <br>`git config --global user.email "email"`
3. Konfiguration abgeschlossen


### 04 - Vagrant Befehle
***

* vagrant up -> startet die aktuelle VM
* vagrant destroy -> stoppt und löscht die aktuelle VM
* vagrant init "boxname" -> erstellt vagrantfile mit angegebener Box
* vagrant suspend -> stoppt die aktuelle VM
* vagrant status -> zeigt den aktuelle Status der VM an


### 05 - Vagrant Boxen
***

[Web Server][1]


[1]: https://github.com/canci87/M-300-Services/tree/master/VagrantBox/Web%20Server


### 06 - Firewall Konfig
***


