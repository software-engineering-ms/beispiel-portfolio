# **Testplan für Erweiterungen der Social-Media-Plattform**

## **1. Produktanalyse**

### **Zielsetzung**

Das primäre Ziel des Produkts ist die Erweiterung der bestehenden Social-Media-Plattform durch die Einführung neuer Funktionen sowie die Sicherstellung der fehlerfreien Nutzung der bestehenden Funktionalitäten.

### **Zielgruppe**

Das Produkt wird von bestehenden und neuen Nutzern der Social-Media-Plattform verwendet, einschließlich Personen ab 16 Jahren. Nutzer können ein Premium-Abo abschließen, um Werbung zu entfernen, und persönliche Geschichten in ihrem Profil teilen.

### **Hardware- und Software-Spezifikationen**

- **Hardware-Anforderungen:**
    - Geräte: PCs, Laptops, Smartphones, Tablets
    - Spezifikationen: Standardkonfigurationen für Android- und iOS-Geräte, Desktops mit mindestens 4 GB RAM, 2 GHz Prozessor
- **Software-Anforderungen:**
    - Betriebssysteme: Windows, macOS, Android, iOS
    - Browser: Chrome, Firefox, Safari, Edge
    - Abhängigkeiten: Backend-Services, externe Werbedienste, Zahlungs-Gateways

### **Produktfunktionalität**

- Die Plattform ermöglicht Nutzern:
- Registrierung und Login
- Bilder zum Profil hinzufügen
- Freunde finden und zu Favoriten hinzufügen
- Werbung durch ein kostenpflichtiges Abo zu entfernen
- Profilgeschichten zu erstellen und anzuzeigen

## **2. Teststrategie-Entwurf**

### **Testumfang**

- **Im Testumfang:**
    - Registrierung und Login
    - Bilder zum Profil hinzufügen
    - Freunde finden
    - Freunde zu Favoriten hinzufügen
    - Altersbeschränkung bei Kontoerstellung
    - Kostenpflichtiges Abo zur Werbefreiheit
    - Profilgeschichte
- **Außerhalb des Testumfangs:**
    - Backend-Datenbankoperationen ohne UI-Auswirkung
    - Externe Werbedienst-Integration (außer bei Werbefreiheit für Premium-Nutzer)

### **Arten des Testens**

- Functional Testing
- Regression Testing
- Performance Testing
- Security Testing
- Usability Testing

### **Risiken und Probleme**

- **Entwicklungsverzögerungen**
    - Maßnahme: Pufferzeiten im Zeitplan einplanen.
- **Mangel an Testdaten**
    - Maßnahme: Erstellung von Mock-Datensätzen für Testzwecke.
- **Ressourcenengpässe**
    - Maßnahme: Ersatzressourcen identifizieren.

### **Testlogistik**

- **Jane Smith** - Test Manager
- **John Doe** - QA Engineer (Functional und Regression Testing)
- **Alice Johnson** - QA Engineer (Performance und Security Testing)
- **Robert Brown** - QA Engineer (Usability Testing)
- **Maria Garcia** - End User für UAT

## **3. Testziele**

### **Ziele**

- **Funktionalität:** Neue Features und bestehende Funktionen arbeiten wie vorgesehen.
- **GUI:** Benutzeroberfläche ist benutzerfreundlich und konsistent.
- **Performance:** Plattform erfüllt Performance-Anforderungen unter Last.
- **Sicherheit:** Sicherheitslücken werden erkannt und minimiert.
- **Usability:** Plattform ist leicht verständlich und bedienbar.

### **Erwartete Ergebnisse**

- **Funktionalität:** Alle Features entsprechen den Spezifikationen.
- **GUI:** Oberfläche ist intuitiv, reaktionsschnell und fehlerfrei.
- **Performance:** Plattform erreicht definierte Benchmarks.
- **Sicherheit:** Keine kritischen Schwachstellen vorhanden.
- **Usability:** Nutzer können problemlos navigieren und interagieren.

## **4. Testkriterien**

### **Abbruchkriterien**

- Tests werden ausgesetzt, wenn kritische Defekte auftreten, die weitere Tests blockieren.
- Mangel an Ressourcen oder Ausfälle der Testumgebung.

### **Ausstiegskriterien**

- Alle geplanten Tests wurden ausgeführt.
- Run Rate: Mindestens 95 % aller Testfälle wurden durchgeführt.
- Pass Rate: Mindestens 90 % der ausgeführten Tests wurden bestanden.
- Alle kritischen und hochpriorisierten Defekte sind behoben und geschlossen.
- Keine offenen Defekte mit Schweregrad 1 oder 2.
- Performance-Kennzahlen entsprechen den Vorgaben.
- Alle relevanten Sicherheitslücken wurden adressiert.
- UAT abgeschlossen und durch Endnutzer freigegeben.

## **5. Ressourcenplanung**

- **Human Resources:** QA-Team, Development-Team, Enduser für UAT
- **Hardware:** PCs, Laptops, Smartphones, Tablets
- **Software:** Browser (Chrome, Firefox, Safari, Edge), Betriebssysteme (Windows, macOS, Android, iOS)
- **Infrastruktur:** Testumgebungen, Automatisierungstools, Performance-Testtools

## **6. Testumgebung planen**

- **Testumgebungen:** Reale Geräte mit realen Betriebssystemen und Browsern zur Simulation von Nutzerbedingungen.
- **Umgebungen:** Development (DEV), Testing (TEST), Acceptance (ACC), Production (PROD)

## **7. Zeitplan und Schätzung**

| Aktivität           | Startdatum | Enddatum   | Umgebung | Verantwortlich   | Geschätzter Aufwand |
| ------------------- | ---------- | ---------- | -------- | ---------------- | ------------------- |
| Testplanung         | 01.08.2024 | 05.08.2024 | Alle     | Test Manager     | 20 Std.             |
| Testfall-Design     | 06.08.2024 | 15.08.2024 | Alle     | QA Team          | 40 Std.             |
| Unit Tests          | 16.08.2024 | 25.08.2024 | DEV      | Entwicklungsteam | 60 Std.             |
| Integrationstests   | 26.08.2024 | 30.08.2024 | TEST     | QA Team          | 30 Std.             |
| Systemtests         | 01.09.2024 | 10.09.2024 | TEST     | QA Team          | 80 Std.             |
| Regressionstests    | 11.09.2024 | 15.09.2024 | TEST     | QA Team          | 40 Std.             |
| Performance-Tests   | 16.09.2024 | 18.09.2024 | TEST     | QA Team          | 20 Std.             |
| Sicherheitstests    | 19.09.2024 | 21.09.2024 | TEST     | QA Team          | 20 Std.             |
| UAT                 | 22.09.2024 | 30.09.2024 | ACC      | Endnutzer        | 50 Std.             |
| Produktions-Release | 01.10.2024 | 01.10.2024 | PROD     | DevOps Team      | 10 Std.             |

## **8. Test-Deliverables**

Dokumente/Tools, die zur Unterstützung der Testaktivitäten erstellt werden müssen:

- **Testplan-Dokument**
- **Testfälle und Testskripte**
- **Testdaten**
- **Testberichte**
- **Defektberichte**
- **UAT-Freigabedokument**