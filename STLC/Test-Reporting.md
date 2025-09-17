Dieses Dokument enthält zwei Beispiel-Szenarien. Verwende eine ähnliche Vorlage für dein eigenes Portfolio, aber decke alle notwendigen Szenarien ab!

### Szenario 1: Gültiges Geburtsdatum

Als Nutzer von FindMate kann ich mich registrieren und einloggen, wenn ich 16 Jahre alt bin.

| Schritt | Aktion                                                                                    | Erwartetes Ergebnis                                                                      | OK/NOK | URL                                                                      | Link zum Issue |
| ------- | ----------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------ | -------------- |
| 1       | Gehe zur Login-Seite von FindMate                                                         | Login-Seite erscheint                                                                    | OK     | [https://findmate.masterschool.com/](https://findmate.masterschool.com/) |                |
| 2       | Klicke auf „Sign up“                                                                      | Du wirst auf die Registrierungsseite weitergeleitet                                      | OK     | /auth                                                                    |                |
| 3a      | Fülle „RandomUsername“ ein                                                                |                                                                                          |        |                                                                          |                |
| 3b      | Geburtsdatum „18-08-2008“ eingeben                                                        |                                                                                          |        |                                                                          |                |
| 3c      | Schreibe „This is my Bio“                                                                 |                                                                                          |        |                                                                          |                |
| 3d      | E-Mail „[karin@faculty.masterschool.com](mailto:karin@faculty.masterschool.com)“ eingeben |                                                                                          |        |                                                                          |                |
| 3e      | Passwort „RandomPassword1“                                                                |                                                                                          |        |                                                                          |                |
| 4       | Klicke auf „Sign up“                                                                      | Du wirst zur Login-Seite weitergeleitet. E-Mail und Passwort sind automatisch ausgefüllt | OK     |                                                                          |                |
| 5       | Klicke auf „Log in“                                                                       | Du wirst erfolgreich eingeloggt                                                          | OK     |                                                                          |                |


![image](https://github.com/user-attachments/assets/a593d7b6-456f-4094-9c8a-dc88f4b4ef4c)
![image](https://github.com/user-attachments/assets/4c8dafd1-dd9b-4ee7-9779-0525cade6d46)
![image](https://github.com/user-attachments/assets/2972e9bd-76fc-421f-8d4f-2d175d9a2a2d)
![image](https://github.com/user-attachments/assets/f210f720-d67f-41d7-a94e-454b1142d5c0)


### Szenario 2: Ungültiges Geburtsdatum

Als Nutzer von FindMate kann ich mich nicht registrieren, wenn ich ein ungültiges Geburtsdatum angebe.

| Schritt | Aktion                                                                                    | Erwartetes Ergebnis                                                        | OK/NOK | URL                                                                      | Link zum Issue                                                                      |
| ------- | ----------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------ | ----------------------------------------------------------------------------------- |
| 1       | Gehe zur Login-Seite von FindMate                                                         | Login-Seite erscheint                                                      | OK     | [https://findmate.masterschool.com/](https://findmate.masterschool.com/) |                                                                                     |
| 2       | Klicke auf „Sign up“                                                                      | Du wirst auf die Registrierungsseite weitergeleitet                        | OK     | /auth                                                                    |                                                                                     |
| 3a      | Fülle „InputValidationTest“ als Username ein                                              |                                                                            |        |                                                                          |                                                                                     |
| 3b      | Geburtsdatum „19-08-1820“ eingeben                                                        |                                                                            |        |                                                                          |                                                                                     |
| 3c      | Schreibe „This is my Bio“                                                                 |                                                                            |        |                                                                          |                                                                                     |
| 3d      | E-Mail „[karin@faculty.masterschool.com](mailto:karin@faculty.masterschool.com)“ eingeben |                                                                            |        |                                                                          |                                                                                     |
| 3e      | Passwort „RandomPassword1“                                                                |                                                                            |        |                                                                          |                                                                                     |
| 4       | Klicke auf „Sign up“                                                                      | Du kannst nicht 200 Jahre alt sein, daher wird eine Fehlermeldung erwartet | NOK    |                                                                          | [Issue-Link](https://github.com/software-engineering-ms/example-portfolio/issues/2) |
