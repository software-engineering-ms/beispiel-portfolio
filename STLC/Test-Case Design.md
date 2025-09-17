
**Entwirf Deine Testfälle basierend auf den Features, die für das kommende Release der Social-Media-Website entwickelt werden!**

**Du musst sie nur *entwerfen*, die Ausführung erfolgt in einer späteren Phase.**

**Füge, falls zutreffend, die Test-Design-Technik hinzu.**

### **1. Altersbeschränkung für die Kontoerstellung**

**Test-Design-Techniken**: Boundary Value Analysis (BVA), Equivalence Partitioning (EP), Error Guessing

### Testfälle:

1. **Boundary Value Analysis**:
    - **Testfall**: Kontoerstellung für einen Nutzer genau 16 Jahre alt überprüfen.
        - **Input**: Geburtsdatum = (Heute - 16 Jahre)
        - **Erwartetes Ergebnis**: Kontoerstellung erfolgreich.
2. **Boundary Value Analysis**:
    - **Testfall**: Kontoerstellung für einen Nutzer knapp unter 16 Jahren überprüfen.
        - **Input**: Geburtsdatum = (Heute - 16 Jahre + 1 Tag)
        - **Erwartetes Ergebnis**: Fehlermeldung „Du musst mindestens 16 Jahre alt sein, um ein Konto zu erstellen.“
3. **Equivalence Partitioning**:
    - **Testfall**: Kontoerstellung für Nutzer unter 16 Jahren überprüfen.
        - **Input**: Geburtsdatum = (Heute - 15 Jahre)
        - **Erwartetes Ergebnis**: Fehlermeldung wird angezeigt.
4. **Equivalence Partitioning**:
    - **Testfall**: Kontoerstellung für Nutzer über 16 Jahren überprüfen.
        - **Input**: Geburtsdatum = (Heute - 17 Jahre)
        - **Erwartetes Ergebnis**: Kontoerstellung erfolgreich.
5. **Error Guessing**:
    - **Testfall**: Systemverhalten überprüfen, wenn kein Geburtsdatum eingegeben wird.
        - **Input**: Feld „Geburtsdatum“ leer lassen.
        - **Erwartetes Ergebnis**: Fehlermeldung „Geburtsdatum ist erforderlich.“
6. **Error Guessing**:
    - **Testfall**: Systemverhalten überprüfen, wenn ein ungültiges Datumsformat eingegeben wird.
        - **Input**: Geburtsdatum = „13/25/2008“
        - **Erwartetes Ergebnis**: Fehlermeldung „Ungültiges Geburtsdatum-Format. Bitte MM/TT/JJJJ verwenden.“

### **2. Kostenpflichtiges Abonnement zur Werbefreiheit**

**Test-Design-Techniken**: Use Case Testing, Boundary Value Analysis (BVA), Error Guessing

### Testfälle:

1. **Use Case Testing**:
    - **Testfall**: Option zum Abonnieren eines kostenpflichtigen Plans in den Kontoeinstellungen überprüfen.
        - **Input**: Navigation zu den Kontoeinstellungen.
        - **Erwartetes Ergebnis**: Abonnement-Option ist sichtbar.
2. **Boundary Value Analysis**:
    - **Testfall**: Erfolgreiches Abonnement mit gültigen Zahlungsdaten überprüfen.
        - **Input**: Gültige Kreditkartendaten.
        - **Erwartetes Ergebnis**: Abonnement erfolgreich, Werbung deaktiviert.
3. **Error Guessing**:
    - **Testfall**: Systemverhalten bei fehlerhafter Zahlung überprüfen.
        - **Input**: Ungültige Kreditkartendaten.
        - **Erwartetes Ergebnis**: Fehlermeldung „Zahlung fehlgeschlagen. Bitte erneut versuchen.“
4. **Use Case Testing**:
    - **Testfall**: Systemverhalten bei Abonnement-Verlängerung überprüfen.
        - **Input**: Verlängerungsdatum erreicht, gültige Zahlungsdaten.
        - **Erwartetes Ergebnis**: Abonnement verlängert, Werbung bleibt deaktiviert.
5. **Error Guessing**:
    - **Testfall**: Systemverhalten bei Abonnement-Kündigung überprüfen.
        - **Input**: Abonnement kündigen.
        - **Erwartetes Ergebnis**: Abonnement gekündigt, Werbung wieder angezeigt.
6. **Use Case Testing:**
    - **Testfall**: Verfügbarkeit der Abo-Option während des Registrierungsprozesses überprüfen.
        - **Input**: Alle Pflichtfelder ausfüllen, zur Abo-Option navigieren.
        - **Erwartetes Ergebnis**: Option zum Premium-Abo sichtbar, Zahlung möglich, Konto wird erstellt und Werbung deaktiviert.

### **3. Profilgeschichte**

**Test-Design-Techniken**: Boundary Value Analysis (BVA), Equivalence Partitioning (EP), Error Guessing

### Testfälle:

1. **Boundary Value Analysis**:
    - **Testfall**: Profilgeschichte mit genau 100 Zeichen überprüfen.
        - **Input**: Text mit 100 Zeichen.
        - **Erwartetes Ergebnis**: Geschichte erfolgreich gespeichert und angezeigt.
2. **Boundary Value Analysis**:
    - **Testfall**: Profilgeschichte mit mehr als 100 Zeichen überprüfen.
        - **Input**: Text mit 101 Zeichen.
        - **Erwartetes Ergebnis**: Fehlermeldung „Profilgeschichte darf maximal 100 Zeichen haben.“
3. **Equivalence Partitioning**:
    - **Testfall**: Profilgeschichte mit weniger als 100 Zeichen überprüfen.
        - **Input**: Text mit 50 Zeichen.
        - **Erwartetes Ergebnis**: Geschichte erfolgreich gespeichert und angezeigt.
4. **Error Guessing**:
    - **Testfall**: Profilgeschichte ohne Eingabe überprüfen.
        - **Input**: Feld leer lassen.
        - **Erwartetes Ergebnis**: Geschichte erfolgreich gespeichert (falls leere Eingabe erlaubt).
5. **Error Guessing**:
    - **Testfall**: Profilgeschichte mit unzulässigen Zeichen oder Schimpfwörtern überprüfen.
        - **Input**: Text mit verbotenen Wörtern.
        - **Erwartetes Ergebnis**: Fehlermeldung „Profilgeschichte enthält unzulässigen Inhalt.“
6. **Use Case Testing**:
    - **Testfall**: Anzeige der Profilgeschichte direkt unter dem Kontonamen überprüfen.
        - **Input**: Zur Profilseite navigieren.
        - **Erwartetes Ergebnis**: Geschichte korrekt angezeigt und ausgerichtet.
7. **Use Case Testing**:
    - **Testfall**: Sichtbarkeit der Profilgeschichte für registrierte Nutzer überprüfen.
        - **Input**: Registrierter Nutzer ruft Profilseite auf.
        - **Erwartetes Ergebnis**: Profilgeschichte sichtbar.
8. **Use Case Testing**:
    - **Testfall**: Unsichtbarkeit der Profilgeschichte für nicht registrierte Nutzer überprüfen.
        - **Input**: Nicht registrierter Nutzer ruft Profilseite auf.
        - **Erwartetes Ergebnis**: Profilgeschichte nicht sichtbar; ggf. Hinweis „Bitte anmelden, um Inhalte zu sehen.“
9. **Boundary Value Analysis (Input-Validierung)**:
    - **Testfall**: Systemverhalten bei leerem Eingabefeld überprüfen.
        - **Input**: Eingabefeld leer lassen, speichern versuchen.
        - **Erwartetes Ergebnis**: Je nach Vorgabe entweder erfolgreich gespeichert oder Fehlermeldung.
10. **Use Case Testing (Session-Timeout)**:
    - **Testfall**: Verhalten beim Bearbeiten der Profilgeschichte nach Session-Ablauf überprüfen.
        - **Input**: Session läuft beim Bearbeiten ab, dann neu einloggen.
        - **Erwartetes Ergebnis**: Änderungen nicht gespeichert, alter Stand sichtbar, ungesicherte Änderungen verloren.