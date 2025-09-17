## **Die Software**

Soziale Medien Plattform mit den folgenden bestehenden Funktionalitäten:

- Registrierungs- und Login-Funktionalität
- Bilder zum Profil hinzufügen
- Freunde finden
- Freunde zu Favoriten hinzufügen
- Soziale Medien Plattform enthält Werbung

## **Neue Funktionen**

### **1. Altersbeschränkung für die Kontoerstellung**

**Unklare Anforderung:**

- Nutzer sollten nur dann ein Konto erstellen können, wenn sie das Mindestalter von 16 Jahren erreicht haben.

**Fragen:**

1. Wie soll die Altersüberprüfung implementiert werden? (z. B. Eingabe des Geburtsdatums)
2. In welchem Format soll das Geburtsdatum eingegeben werden? (z. B. MM/TT/JJJJ)
3. Welche Fehlermeldung soll angezeigt werden, wenn der Nutzer unter 16 ist?
4. Gibt es spezifische rechtliche Hinweise oder Datenschutzhinweise, die für die Altersüberprüfung erforderlich sind?

**Detaillierte Anforderung:**

- Während des Registrierungsprozesses müssen Nutzer ihr Geburtsdatum angeben. Das System sollte validieren, dass der Nutzer zum Zeitpunkt der Kontoerstellung mindestens 16 Jahre alt ist. Wenn der Nutzer jünger als 16 ist, soll eine Fehlermeldung angezeigt werden, und das Konto darf nicht erstellt werden.

### **2. Kostenpflichtiges Abonnement zur Werbefreiheit**

**Unklare Anforderung:**

- Es sollte eine Option geben, mit der Nutzer ein kostenpflichtiges Abo abschließen können, das ihnen ermöglicht, die Plattform ohne Werbung zu nutzen.

**Fragen:**

1. Wo soll die Option zum Abonnieren des kostenpflichtigen Plans angezeigt werden? (z. B. Kontoeinstellungen, Startseite)
2. Welche Zahlungsmethoden werden unterstützt?
3. Was soll passieren, wenn die Zahlung fehlschlägt?
4. Wie soll das System Abonnementverlängerungen und -kündigungen handhaben?
5. Welche Preismodelle sollen für das Abonnement angeboten werden?

**Detaillierte Anforderung:**

- Nutzer sollten in ihren Kontoeinstellungen die Möglichkeit haben, ein Premium-Abo abzuschließen. Nach erfolgreichem Abschluss und Zahlung sollen auf der gesamten Plattform keine Werbeanzeigen mehr angezeigt werden. Das System sollte außerdem den Abonnementstatus verwalten, Erinnerungen zur Verlängerung bereitstellen sowie Szenarien handhaben, in denen das Abonnement abläuft oder gekündigt wird.

### **3. Profilgeschichte**

**Unklare Anforderung:**

- Nutzer sollten die Möglichkeit haben, eine kurze Geschichte über sich selbst zu verfassen, die unter ihrem Kontonamen im Profil angezeigt wird. Diese Geschichte sollte ein Zeichenlimit haben.

**Fragen:**

1. Wo soll das Eingabefeld für die Profilgeschichte platziert werden?
2. Soll es Formatierungsoptionen geben? (z. B. fett, kursiv)
3. Was soll passieren, wenn der Nutzer das Zeichenlimit überschreitet? (z. B. Fehlermeldung, Text wird abgeschnitten)
4. Gibt es Einschränkungen für den Inhalt der Geschichte? (z. B. Filter für vulgäre Sprache)

**Detaillierte Anforderung:**

- Nutzer sollten in ihren Profileinstellungen ein Eingabefeld haben, in das sie eine persönliche Geschichte oder Biografie eintragen können. Dieses Feld sollte maximal 100 Zeichen zulassen. Die Geschichte wird unter dem Kontonamen auf der Profilseite des Nutzers angezeigt. Das System sollte eine Rückmeldung geben, wenn der Nutzer versucht, mehr als 100 Zeichen einzugeben, und verhindern, dass die überschüssigen Zeichen gespeichert werden. Für das MVP wird es keinen Filter für vulgäre Sprache geben; dieser wird später implementiert.