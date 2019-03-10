Dokumentation 
=============

### Übersicht
***

* 1. [SSH Key erstellen] (#-01-SSH-Key-erstellen)
2. SSH Key hinzufügen
3. Client Konfigurieren


01 SSH Key erstellen
===


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


02 SSH Key hinzufügen
===


1. Auf www.github.com anmelden
2. Zu den Einstellungen wechseln
3. Bei den "personal settings" zu "SSH und GPG keys" wechseln
4. Unter "title" eine Bezeichnung angeben (z.B. EC_SSH_Key)
5. Datei "%HOME%/.ssh/id_rsa.pub" oder "$HOME/.ssh/id_rsa.pub" in Zwischenablage kopieren
6. Den Code auf GitHub einfügen und auf "Add SSH key" klicken
7. Der Schlüssel taucht nun in der übergeordneten Liste auf


03 Client konfigurieren
===


1. Git-Bash öffnen
2. Git konfigurieren mit GitHub Account
      <br>`git config --global user.name "username"`
      <br>`git config --global user.email "email"`
3. Konfiguration abgeschlossen
