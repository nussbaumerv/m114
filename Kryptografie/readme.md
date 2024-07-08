# KRYPTOGRAFIE PGP (Pretty Good Privacy)

## Aufgaben

### 1. Wie kann ich einen Public Key verifizieren?

Zur Verifizierung eines Public Keys benötigen Sie den dazugehörigen **Fingerabdruck (Fingerprint)**. Dieser ist ein eindeutiger Hashwert des Public Keys und dient zur Überprüfung seiner Integrität. Sie können den Fingerabdruck mit dem vom Ersteller des Schlüssels veröffentlichten Wert vergleichen. Eine weitere Möglichkeit ist die Überprüfung durch eine vertrauenswürdige Zertifizierungsstelle (CA), die die Echtheit des Schlüssels bestätigt.

### 2. Was versteht man unter Public Key Infrastruktur (PKI)?

**Public Key Infrastruktur (PKI)** ist ein System aus Hardware, Software, Personen, Richtlinien und Verfahren, das zur Verwaltung von Public-Key-Zertifikaten und zur sicheren Kommunikation zwischen zwei Parteien dient. Es ermöglicht die Ausstellung, Verteilung und Überprüfung digitaler Zertifikate, die die Identität von Personen, Organisationen oder Geräten bestätigen.

### 3. Was bedeutet Certification Authority (CA) und was Trust Center (TC)?

**Certification Authority (CA)** ist eine vertrauenswürdige Instanz, die digitale Zertifikate ausstellt und die Identität von Personen oder Organisationen überprüft. Sie bestätigt, dass der Public Key im Zertifikat tatsächlich dem Inhaber gehört.

**Trust Center (TC)** ist ein sicherer Ort, an dem digitale Zertifikate und Schlüssel sicher aufbewahrt und verwaltet werden. Es kann auch als CA fungieren und digitale Zertifikate ausstellen.

### 4. Wer hat das Zertifikat für die Bankwebseite [www.ubs.com](https://www.ubs.com/) ausgestellt und wie lange ist es gültig?

Das Zertifikat für [www.ubs.com](https://www.ubs.com) wurde von DigiCert Inc. ausgestellt und ist gültig bis Freitag, 13. Dezember 2024 um 00:59:59 Uhr.

### 5. Wer hat das Zertifikat für die Schulwebseite [www.tbz.ch](https://tbz.ch/) ausgestellt und wie lange ist es gültig?

Das Zertifikat für www.tbz.ch wurde von Let's Encrypt ausgestellt und ist gültig bis Sonntag, 30. Juni 2024 um 19:35:24 Uhr.

### 6. Wer hat das Zertifikat für die Webseite [www.example.ch] ausgestellt und wie lange ist es gültig?

Die Webseite www.example.ch hat kein gültiges Zertifikat.

### 7. Wählen Sie irgendeine Applikation aus, die auf Ihrem PC installiert ist. Stellen Sie sich nun vor, Sie müssten diese von Hand aktualisieren oder aus Kompatibilitätsgründen auf eine frühere Version zurückstufen. Wo finden Sie aktuelle und frühere Versionen Ihrer Software und wie wird sichergestellt, dass die dort angebotene SW-Version auch wirklich echt ist bzw. vom SW-Entwickler stammt?

Aktuelle und frühere Versionen von Software finden Sie in der Regel auf der offiziellen Webseite des Softwareherstellers. Um sicherzustellen, dass die heruntergeladene Software echt ist, können Sie die digitale Signatur der Datei überprüfen. Diese Signatur bestätigt, dass die Datei vom Hersteller stammt und nicht verändert wurde.

### 8. Erstellen Sie eine virtuelle Linux-Maschine mit z.B. VirtualBox und Ubuntu. Richten Sie nun auf Ihrem WIN-PC eine Remoteverbindung via SSH zu Ihrem Linux-PC ein. Überprüfen Sie die Verbindung. Wäre auch eine graphische Anbindung möglich?

Ja, nach der Einrichtung der SSH-Verbindung ist auch eine graphische Anbindung über Tools wie X11-Forwarding oder VNC (Virtual Network Computing) möglich.

### 10. Öffnen Sie die beiden folgenden Webseiten und achten Sie auf die Unterschiede in der Webadresszeile. Was stellen Sie bezüglich Protokoll und Zertifikat fest?

- [https://juergarnold.ch](https://juergarnold.ch)
- [https://www.zkb.ch](https://www.zkb.ch)

Beide Webseiten verwenden das HTTPS-Protokoll, aber sie verwenden unterschiedliche Zertifikate, die von verschiedenen Zertifizierungsstellen ausgestellt wurden.

### 11. Wenn Sie sich mit Zertifikaten befassen, fallen Ihnen früher oder später folgende Anbieter bzw. Webseiten auf:

- [http://www.cacert.org](http://www.cacert.org/)
- [https://letsencrypt.org/de](https://letsencrypt.org/de)

#### Was genau wird hier zu welchen Konditionen angeboten?

- **CAcert:** Bietet kostenlose Zertifikate an, basiert auf einem Web of Trust-Modell. Die Identität des Antragstellers wird überprüft, aber nicht so streng wie bei kommerziellen CAs.
- **Let's Encrypt:** Bietet kostenlose Domain-Validated-Zertifikate an. Die Ausstellung erfolgt automatisiert und die Gültigkeit ist auf 90 Tage begrenzt.

### 12. Folgende TLS-Zertifikatsarten werden unterschieden: Domain Validated, Organization Validated und Extended Validation. Sie möchten einen Webshop betreiben, wo mit Kreditkarte bezahlt werden kann. Welcher Zertifikatstyp ist der richtige?

Für einen Webshop mit Kreditkartenzahlung ist ein **Extended Validation (EV)**-Zertifikat empfehlenswert. Es bietet die höchste Validierungsebene und stärkt das Vertrauen der Kunden, da der Name des Unternehmens in der Adressleiste des Browsers angezeigt wird.

### 13. Studieren Sie den Beitrag auf der Webseite Let's Encrypt "Wie es funktioniert":

[https://letsencrypt.org/de/how-it-works/](https://letsencrypt.org/de/how-it-works/)

#### Was ist der Unterschied zwischen OpenPGP und X.509?

- **OpenPGP:** Ein dezentraler Standard für die Verschlüsselung und digitale Signatur von E-Mails und Dateien. Verwendet das Web of Trust-Modell zur Vertrauensbildung.
- **X.509:** Ein hierarchischer Standard für digitale Zertifikate, der hauptsächlich zur Authentifizierung von Webseiten und Servern verwendet wird. Verwendet eine zentrale Vertrauenskette von Zertifizierungsstellen.

### 14. Erklären Sie den Aufruf einer sicheren Webseite (HTTPS). Wie ist der Ablauf beim Protokoll TLS? Wo genau kommen die Zertifikate ins Spiel?

Beim Aufruf einer sicheren Webseite (HTTPS) wird das TLS-Protokoll verwendet, um eine verschlüsselte Verbindung zwischen Client und Server herzustellen. Der Ablauf umfasst:

1. **Handshake:** Client und Server einigen sich auf die zu verwendende TLS-Version und Verschlüsselungsalgorithmen.
2. **Authentifizierung:** Der Server sendet sein X.509-Zertifikat an den Client. Der Client überprüft die Gültigkeit des Zertifikats und die Identität des Servers.
3. **Schlüsselaustausch:** Client und Server tauschen kryptografische Schlüssel aus, um die Kommunikation zu verschlüsseln.
4. **Verschlüsselte Datenübertragung:** Die Daten werden verschlüsselt übertragen, um sie vor unbefugtem Zugriff zu schützen.

### 15. Was bedeutet S/MIME?

**S/MIME (Secure/Multipurpose Internet Mail Extensions)** ist ein Standard für die sichere Übertragung von E-Mails. Es ermöglicht die Verschlüsselung, digitale Signatur und Authentifizierung von E-Mails.

### 16. Aus gesetzlichen Gründen sind Sie verpflichtet, den gesamten geschäftlichen E-Mail-Verkehr zu archivieren, auch den verschlüsselten. Was ist das Problem dabei und wie könnte man dies lösen?

Das Problem beim Archivieren verschlüsselter E-Mails besteht darin, dass der Inhalt ohne den privaten Schlüssel nicht lesbar ist. Lösungen:

- **Archivierung vor Verschlüsselung:** E-Mails werden vor der Verschlüsselung archiviert.
- **Schlüsselarchivierung:** Private Schlüssel werden sicher zusammen mit den verschlüsselten E-Mails archiviert.
- **Verwendung von Hardware-Sicherheitsmodulen (HSM):** HSMs ermöglichen die sichere Speicherung und Verwendung von Schlüsseln für die Entschlüsselung bei Bedarf.