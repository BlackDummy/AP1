# OSI-Modell Informationen

## Einführung in das OSI-Modell

Das OSI-Modell (Open Systems Interconnection Model) ist ein konzeptionelles Modell, das die Funktionen eines Kommunikationssystems in abstrahierte Schichten unterteilt. Es wurde von der International Organization for Standardization (ISO) entwickelt und dient als Referenzmodell für die Netzwerkkommunikation.

## Die sieben Schichten des OSI-Modells

### 1. Physikalische Schicht (Physical Layer)
- **Funktion**: Übertragung von rohen Bitströmen über ein physikalisches Medium.
- **Beispiele**: Kabel, Stecker, Netzwerkkarten, Hubs.
- **Protokolle**: Ethernet, Wi-Fi.

### 2. Sicherungsschicht (Data Link Layer)
- **Funktion**: Fehlererkennung und -korrektur, Rahmenbildung, MAC-Adressierung.
- **Beispiele**: Switches, Bridges.
- **Protokolle**: Ethernet, PPP, ARP.

### 3. Netzwerkschicht (Network Layer)
- **Funktion**: Routing von Datenpaketen zwischen verschiedenen Netzwerken.
- **Beispiele**: Router.
- **Protokolle**: IP (Internet Protocol), ICMP, ARP.

### 4. Transportschicht (Transport Layer)
- **Funktion**: Zuverlässige Datenübertragung, Flusskontrolle, Fehlerkorrektur.
- **Beispiele**: End-to-End-Kommunikation.
- **Protokolle**: TCP (Transmission Control Protocol), UDP (User Datagram Protocol).

### 5. Sitzungsschicht (Session Layer)
- **Funktion**: Verwaltung von Sitzungen oder Verbindungen zwischen Anwendungen.
- **Beispiele**: Sitzungsaufbau, -verwaltung und -abbau.
- **Protokolle**: NetBIOS, PPTP.

### 6. Darstellungsschicht (Presentation Layer)
- **Funktion**: Datenübersetzung, Verschlüsselung und Komprimierung.
- **Beispiele**: Datenformatierung, Datenverschlüsselung.
- **Protokolle**: SSL/TLS, JPEG, MPEG.

### 7. Anwendungsschicht (Application Layer)
- **Funktion**: Bereitstellung von Netzwerkdiensten direkt für Endbenutzeranwendungen.
- **Beispiele**: E-Mail, Web-Browser, Dateitransfer.
- **Protokolle**: HTTP, FTP, SMTP, DNS.

## Vorteile des OSI-Modells
- **Modularität**: Jede Schicht kann unabhängig voneinander entwickelt und gewartet werden.
- **Interoperabilität**: Verschiedene Systeme können miteinander kommunizieren, wenn sie die gleichen Protokolle verwenden.
- **Fehlerisolierung**: Probleme können leichter identifiziert und behoben werden, da sie auf eine bestimmte Schicht beschränkt sind.

| OSI-Schicht | Deutscher Name der Schicht    | Englischer Name der Schicht     | Begriff (z. B. TCP)      | Erkennungsmerkmale                                      |
|-------------|-------------------------------|----------------------------------|--------------------------|--------------------------------------------------------|
| 7           | Anwendungsschicht             | Application Layer               | HTTP, FTP, SMTP          | Anwendungen wie Browser oder E-Mail-Programme         |
| 6           | Darstellungsschicht           | Presentation Layer              | SSL/TLS, JPEG, MPEG      | Datenverschlüsselung oder -umwandlung                 |
| 5           | Sitzungsschicht               | Session Layer                   | NetBIOS, RPC             | Verbindungssteuerung (z. B. Sitzungsprotokollierung)  |
| 4           | Transportschicht              | Transport Layer                 | TCP, UDP                 | Ports (z. B. 80 für HTTP, 443 für HTTPS)              |
| 3           | Netzwerkschicht               | Network Layer                   | IP, ICMP, ARP            | IP-Adressen (z. B. IPv4, IPv6)                        |
| 2           | Sicherungsschicht             | Data Link Layer                 | Ethernet, MAC-Adressen   | MAC-Adressen (z. B. physische Adresse der Netzwerkkarte) |
| 1           | Bitübertragungsschicht        | Physical Layer                  | Kabel, WLAN, Bluetooth   | Physische Verbindungen (z. B. Netzwerkkabel, Signalstärke) |


## Zusammenfassung
Das OSI-Modell bietet eine strukturierte und standardisierte Methode zur Beschreibung der Netzwerkkommunikation. Es hilft Netzwerkadministratoren und Entwicklern, die Komplexität von Netzwerken zu verstehen und zu verwalten, indem es die Funktionen in sieben klar definierte Schichten unterteilt.