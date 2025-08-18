# Barrierefreiheit auf Websites

**Barrierefreiheit (Accessibility, a11y)** bedeutet, dass Websites so gestaltet werden, dass sie für alle Menschen unabhängig von ihren körperlichen oder geistigen Einschränkungen zugänglich sind. Dies verbessert nicht nur die Nutzung für Menschen mit Behinderungen, sondern auch für ältere Nutzer und Personen mit temporären Einschränkungen.

## 1. Warum ist Barrierefreiheit wichtig?
- **Inklusion**: Alle Menschen sollten uneingeschränkt auf Informationen und Funktionen zugreifen können.
- **Rechtliche Anforderungen**: In vielen Ländern gibt es gesetzliche Vorgaben (z. B. die EU-Richtlinie für barrierefreie Websites).
- **SEO-Vorteile**: Suchmaschinen bewerten barrierefreie Websites oft besser.
- **Bessere Nutzererfahrung**: Klare Strukturen und gute Bedienbarkeit helfen allen Nutzern.

## 2. Grundlagen der Barrierefreiheit

### 2.1 Wahrnehmbarkeit
- **Alternativtexte für Bilder**: `<img src="bild.jpg" alt="Beschreibung des Bildes">`
- **Klare Farbkontraste**: Mindestens **4,5:1** für Text gegen den Hintergrund.
- **Text statt Bilder für wichtige Inhalte**: Vermeidung von reinen Bildinhalten für Navigation oder Überschriften.
- **Untertitel und Transkripte** für Audio- und Videoinhalte.

### 2.2 Bedienbarkeit
- **Tastatur-Navigation**: Alle Funktionen müssen per **Tab**, **Enter** und **Pfeiltasten** erreichbar sein.
- **Fokus-Management**: Aktuell fokussierte Elemente sollten visuell hervorgehoben sein.
- **Verzicht auf Zeitlimits**: Nutzer sollten nicht unter Zeitdruck stehen.
- **Sprungmarken und Skip-Links**: Ermöglichen direktes Springen zu Hauptinhalten (`<a href="#content" class="skip-link">Zum Inhalt springen</a>`).

### 2.3 Verständlichkeit
- **Klare und einfache Sprache**: Kurze Sätze, keine komplizierten Fachbegriffe.
- **Eindeutige Formulare**: Labels und Fehlermeldungen sollten klar verständlich sein.
- **Erwartungskonforme Navigation**: Einheitliche Menüführung und konsistentes Layout.

### 2.4 Robustheit
- **Semantisches HTML**: Verwendung von `<header>`, `<nav>`, `<main>`, `<footer>`, `<button>`, `<label>`, usw.
- **Kompatibilität mit Screenreadern**: Unterstützung für Assistenztechnologien wie NVDA oder JAWS.
- **ARIA-Attribute**: Falls notwendig, gezielter Einsatz von ARIA-Rollen (`role="alert"`, `aria-live="polite"`, etc.).

## 3. Best Practices für barrierefreies Webdesign

| Kategorie              | Best Practice |
|------------------------|--------------|
| **Texte & Inhalte**   | Klare Struktur, gut lesbare Schriftarten, ausreichender Zeilenabstand |
| **Farben & Kontraste** | Kontrastverhältnis mindestens **4,5:1**, keine Farbfehlerinformationen |
| **Navigation**        | Konsistente Menüführung, Tastaturbedienung möglich |
| **Formulare**        | Labels nutzen, Fehlermeldungen klar formulieren, Auto-Fill unterstützen |
| **Multimedia**       | Alternativtexte für Bilder, Untertitel für Videos, keine autoplay-Sounds |
| **Technische Umsetzung** | Semantisches HTML, ARIA sparsam und gezielt einsetzen |

## 4. Tools zur Barrierefreiheitsprüfung
- **WAVE** (Web Accessibility Evaluation Tool) – [wave.webaim.org](https://wave.webaim.org/)
- **Lighthouse** (Google Chrome DevTools) – Bewertet Barrierefreiheit, Leistung und SEO.
- **axe DevTools** – Erweiterung für Chrome und Firefox zur Barrierefreiheitsprüfung.
- **Contrast Checker** – Prüft Farbschemata auf ausreichenden Kontrast.

## 5. Fazit
Barrierefreiheit auf Websites ist nicht nur eine gesetzliche Anforderung, sondern verbessert auch die Benutzerfreundlichkeit und Reichweite. Durch den Einsatz von **semantischem HTML, guter Strukturierung und assistiven Technologien** kann eine Website für alle Menschen zugänglich gemacht werden.

---

💡 **Tipp:** Barrierefreiheit sollte von Anfang an in den Entwicklungsprozess integriert werden, um spätere Anpassungen zu vermeiden!
