# Hash-Verfahren

Ein **Hash-Verfahren** ist eine mathematische Funktion, die eine Eingabe beliebiger Länge in eine **feste** Ausgabelänge umwandelt. Das Ergebnis wird als **Hash-Wert** oder **Hash** bezeichnet. Hashes spielen eine zentrale Rolle in der Informatik, insbesondere in Kryptografie, Datenbanken und Prüfsummen.

## 1. Eigenschaften von Hash-Funktionen

Ein gutes Hash-Verfahren sollte folgende Eigenschaften besitzen:

- **Deterministisch**: Die gleiche Eingabe liefert immer denselben Hash-Wert.
- **Schnell berechenbar**: Die Berechnung des Hash-Werts sollte effizient sein.
- **Kollisionsresistenz**: Es sollte schwierig sein, zwei unterschiedliche Eingaben mit demselben Hash-Wert zu finden.
- **Veränderungsresistenz (Avalanche-Effekt)**: Kleine Änderungen der Eingabe sollten den Hash stark verändern.
- **Einweg-Funktion**: Die ursprüngliche Eingabe sollte aus dem Hash-Wert nicht rekonstruiert werden können.

## 2. Anwendungsgebiete

| Bereich                  | Verwendung von Hashes |
|--------------------------|----------------------|
| **Passwort-Speicherung** | Speicherung als Hash statt Klartext (z. B. mit `bcrypt`, `PBKDF2`, `Argon2`) |
| **Datenintegrität** | Prüfsummen (z. B. `SHA-256` zur Dateiüberprüfung) |
| **Digitale Signaturen** | Absicherung von digitalen Dokumenten |
| **Blockchain** | Hashing zur Verknüpfung von Blöcken (`SHA-256` in Bitcoin) |
| **Datenbanken** | Hash-Indexes für schnelle Suche |

## 3. Bekannte Hash-Algorithmen

| Algorithmus  | Länge (Bits) | Eigenschaften & Anwendungsfälle |
|-------------|-------------|---------------------------------|
| **MD5**     | 128         | Veraltet, nicht mehr sicher wegen Kollisionen |
| **SHA-1**   | 160         | Veraltet, anfällig für Angriffe |
| **SHA-256** | 256         | Sicher, häufig in Kryptografie und Blockchain verwendet |
| **SHA-512** | 512         | Sicher, aber größere Ausgabe |
| **bcrypt**  | Variabel    | Geeignet für Passwort-Hashing, langsame Berechnung für mehr Sicherheit |
| **Argon2**  | Variabel    | Moderner Passwort-Hashing-Algorithmus mit hoher Sicherheit |

## 4. Beispiel: SHA-256 in JavaScript

Hier ein einfaches Beispiel zur Berechnung eines SHA-256-Hashes mit JavaScript:

```javascript
async function generateHash(message) {
    const msgUint8 = new TextEncoder().encode(message);
    const hashBuffer = await crypto.subtle.digest("SHA-256", msgUint8);
    const hashArray = Array.from(new Uint8Array(hashBuffer));
    return hashArray.map(b => b.toString(16).padStart(2, '0')).join('');
}

generateHash("Hallo Welt").then(console.log);
