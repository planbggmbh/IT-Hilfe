IMAP, POP, SMTP
================

.. hint::
 Die nachfolgenden Ausführungen sind veraltet. Microsoft hat die Basisauthentifizierung (Benutzername und Passwort) in Microsoft 365 seit Oktober deaktiviert. Dadurch ist mit diesen Einstellungen ein Abrufen oder Senden
 von E-Mails mit E-Mailclients, die nur die Basisauthentifizierung unterstützen, nicht mehr möglich. Nur wenn der E-Mailclient OAuth unterstützt können Sie diesen weiter mit Micrrosoft 365 verwenden.
 Alternativ können Sie auf Outlook (Android und iOS - kostenfrei / Windows nur mit einer Outlook-Lizenz) oder den `Webclient <https:\\outlook.office.com>`_ zurückgreifen.

E-Mailprogrammeinstellungen
---------------------------

.. index:: POP, IMAP, SMTP

Sofern Sie über keine Outlook-Lizenz für die Desktopversion des Programmes verfügen und Outlook-Web nicht verwenden möchten, können Sie auch ein anderes E-Mail-Programm nutzen.
Dafür benötigen Sie die Einstellungen für den Posteingangsserver (POP oder IMAP) und die Einstellungen des Postausgangsservers (SMTP).

.. note::
	Die Benutzung des Kalenders oder eine aktive Syncronisation ist mit diesem Verfahren nicht möglich.
	
+-------------------------------+-------------------------------+-------------------------------+
| IMAP-Einstellung              | POP-Einstellung               | SMTP-Einstellung              |
+===============================+===============================+===============================+
| Server: outlook.office365.com | Server: outlook.office365.com | Server: smtp.office365.com    |
+-------------------------------+-------------------------------+-------------------------------+
| Port: 993                     | Port: 995                     | Port: 587                     |
+-------------------------------+-------------------------------+-------------------------------+
| Verschlüsselung: SSL/TLS      | Verschlüsselung: SSL/TLS      | Verschlüsselung: STARTTLS     |
+-------------------------------+-------------------------------+-------------------------------+

.. hint::
 Die Nutzung des Postausgangsservers (SMTP) ist in der Standardkonfiguration Ihres Nutzeraccounts deaktiviert. Sofern Sie SMTP 
 benötigen, können Sie über `help@dieetage.de <mailto:help.dieetage.de>`_ die Nutzung beauftragen. Der Dienst sollte spätestens 
 nach 24h aktiv sein. Der Administrator informiert Sie über die Aktivierung per E-Mail.

IMAP
-----

**IMAP** (Internet Message Access Protocoll) ist ein Netzwerkprotokoll, das ein Netzwerkdateisystem für 
E-Mails bereitstellt. IMAP wurde in den 1980er Jahren mit dem Aufkommen von Personal Computern entworfen, um bei der 
Mail-Kommunikation Abhängigkeiten von einzelnen Client-Rechnern aufzulösen. Zu diesem Zweck erweitert IMAP die Funktionen und 
Verfahren so, dass Benutzer ihre Mails, Ordnerstrukturen und Einstellungen auf den (Mail-)Servern speichern und belassen können. 
Die (PC-)Clients greifen direkt online auf die Informationen auf den Servern zu und müssen allenfalls Kopien davon beherbergen. 
Während ein Benutzer von POP nach Verlust seines PC entweder alle E-Mails verloren hat oder bereits gelöschte E-Mails erneut 
erhält, behält ein Benutzer von IMAP seine Mails auf den Servern und, auch über mehrere und verschiedene Clients hinweg, immer 
einen einheitlichen Zugriff. [#FN1]_
 
POP
-----

**POP** (Post Office Protokoll) ist ein Internet-Protokoll um E-Mails vom Mailserver auf den lokalen Rechner herunterzuladen.
In der Regel werden die E-Mails, im Gegensatz zu IMAP, auf dem Mailserver beim Abrufen der E-Mails mit einem E-Mail-Client 
(E-Mailprogramm) gelöscht.

.. note::
 POP3 ist in der Funktionalität sehr beschränkt und erlaubt nur das Auflisten, Abholen und Löschen von E-Mails am Mailserver. 
 Für weitere Funktionalitäten wie hierarchische Mailboxen direkt am Mailserver, Zugriff auf mehrere Mailboxen während 
 einer Sitzung, Vorselektion der E-Mails usw. müssen Protokolle wie IMAP Verwendung finden.

SMTP
-----

Während IMAP und POP dem E-Mailempfang dienen ist **SMTP** (Simple Mail Transfer Protocoll) ein Internet-Protokoll zum 
Versenden von E-Mails.

.. [#FN1] Seite „Internet Message Access Protocol“. In: Wikipedia – Die freie Enzyklopädie. Bearbeitungsstand: 5. Oktober 2020, 08:31 UTC. URL: https://de.wikipedia.org/w/index.php?title=Internet_Message_Access_Protocol&oldid=204276263 (Abgerufen: 28. Juli 2021, 08:44 UTC)
