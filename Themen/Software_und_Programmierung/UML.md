# UML (Unified Modeling Language)

Die **Unified Modeling Language (UML)** ist eine standardisierte Modellierungssprache zur Visualisierung, Spezifikation, Konstruktion und Dokumentation von Software-Systemen. Sie wird vor allem in der Softwareentwicklung eingesetzt, um komplexe Systeme verständlich darzustellen.

## 1. UML-Diagrammtypen

UML besteht aus verschiedenen Diagrammtypen, die in **strukturbezogene**, **verhaltensbezogene** und **interaktionsbezogene** Diagramme unterteilt werden.

### 1.1 Strukturdiagramme (Structural Diagrams)
Strukturdiagramme beschreiben die statische Architektur eines Systems.

- **Klassendiagramm** – Darstellung von Klassen, deren Eigenschaften und Beziehungen.
- **Objektdiagramm** – Konkrete Instanzen von Klassen zu einem bestimmten Zeitpunkt.
- **Komponentendiagramm** – Struktur von Software-Komponenten und deren Abhängigkeiten.
- **Verteilungsdiagramm (Deployment Diagram)** – Physische Verteilung der Software auf Hardware.
- **Paketdiagramm** – Gruppierung von Elementen in Pakete zur Organisation.
- **Kompositionsstrukturdiagramm** – Detaillierte Darstellung interner Strukturen einer Klasse oder eines Objekts.

### 1.2 Verhaltensdiagramme (Behavioral Diagrams)
Diese Diagramme zeigen, wie sich ein System verhält.

- **Anwendungsfalldiagramm (Use Case Diagram)** – Darstellung der Interaktion von Akteuren mit dem System.
- **Zustandsdiagramm (State Machine Diagram)** – Beschreibt Zustände eines Objekts und deren Übergänge.
- **Aktivitätsdiagramm (Activity Diagram)** – Modellierung von Abläufen und Workflows.

### 1.3 Interaktionsdiagramme (Interaction Diagrams)
Diese spezialisieren Verhaltensdiagramme und beschreiben den Informationsfluss zwischen Objekten.

- **Sequenzdiagramm (Sequence Diagram)** – Zeigt den zeitlichen Ablauf der Interaktion zwischen Objekten.
- **Kommunikationsdiagramm (Communication Diagram)** – Fokus auf den Nachrichtenfluss zwischen Objekten.
- **Zeitverlaufsdiagramm (Timing Diagram)** – Modelliert zeitliche Abläufe und Zustandsänderungen.
- **Interaktionsübersichtsdiagramm** – Kombination aus Sequenz- und Aktivitätsdiagrammen.

## 2. UML-Notationen

In UML werden verschiedene Notationen verwendet, um Elemente und Beziehungen darzustellen:

- **Klassen**: Rechtecke mit drei Abschnitten (Name, Attribute, Methoden).
- **Assoziationen**: Linien zwischen Klassen mit Kardinalitäten (`1..*`, `0..1`).
- **Vererbungen**: Pfeile mit leerer Dreiecksspitze (`▶`).
- **Abhängigkeiten**: Strichlierte Linien mit Pfeil (`- - -▶`).
- **Zustände**: Kreise mit Bezeichnungen für Zustände und Übergänge.

## 3. Anwendungsgebiete von UML

- Software-Entwicklung
- Systemarchitektur
- Geschäftsprozessmodellierung
- Dokumentation und Analyse bestehender Systeme

## 4. Beispiel: Klassendiagramm

```plaintext
+------------------+
|   Person        |
+------------------+
| -name: String   |
| -alter: int     |
+------------------+
|+getInfo(): String|
+------------------+
        |
        ▼
+------------------+
|   Student       |
+------------------+
| -matrikelNr: int|
+------------------+
|+studieren(): void|
+------------------+
