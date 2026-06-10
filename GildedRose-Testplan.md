
# Testplan: Gilded Rose Refactoring Kata

## 1. Einleitung

Dieses Dokument beschreibt den Testplan für die Gilded Rose Refactoring Kata. Das Ziel des Refactorings ist es, die Codequalität zu verbessern, ohne das Verhalten des Programms zu ändern.

## 2. Testziele

* Sicherstellen, dass das Refactoring keine Fehler einführt.
* Überprüfen, ob das Verhalten des Programms nach dem Refactoring unverändert bleibt.
* Sicherstellen, dass der refaktorisierte Code besser lesbar, wartbar und erweiterbar ist.

## 3. Teststrategie

Wir werden eine Kombination aus manuellen und automatisierten Tests verwenden.

### 3.1. Manuelle Tests

* **Code-Review:** Ein erfahrener Entwickler wird den refaktorierten Code überprüfen, um sicherzustellen, dass er den Best Practices entspricht und keine offensichtlichen Fehler enthält.
* **Exploratives Testen:** Tester werden das Programm manuell verwenden, um unerwartete Fehler zu finden.

### 3.2. Automatisierte Tests

* **Unit-Tests:** Sicherstellen, dass einzelne Komponenten des Programms korrekt funktionieren.
* **Integrationstests:** Überprüfen, ob verschiedene Komponenten des Programms zusammenarbeiten.
* **Akzeptanztests:** Sicherstellen, dass das Programm die Anforderungen des Kunden erfüllt.

## 4. Testfälle

Die folgenden Testfälle werden durchgeführt:

| Testfall-ID | Beschreibung | Erwartetes Ergebnis | Tatsächliches Ergebnis | Status |
|---|---|---|---|---|
| TC001 | Überprüfung der Funktionalität für normale Artikel | Korrektes Verhalten |  |  |
| TC002 | Überprüfung der Funktionalität für "Aged Brie" | Korrektes Verhalten |  |  |
| TC003 | Überprüfung der Funktionalität für "Sulfuras" | Korrektes Verhalten |  |  |
| TC004 | Überprüfung der Funktionalität für Backstage-Pässe | Korrektes Verhalten |  |  |
| TC005 | Überprüfung der Funktionalität für abgelaufene Artikel | Korrektes Verhalten |  |  |
| TC006 | Überprüfung der Funktionalität für maximale Qualität | Korrektes Verhalten |  |  |
| TC007 | Überprüfung der Funktionalität für minimale Qualität | Korrektes Verhalten |  |  |

## 5. Testumgebung

* **Betriebssystem:** [Betriebssystem]
* **Programmiersprache:** [Programmiersprache]
* **Laufzeitumgebung:** [Laufzeitumgebung]

## 6. Testwerkzeuge

* **Unit-Testing-Framework:** [Framework]
* **Testmanagement-Tool:** [Tool]

## 7. Zeitplan

* **Testbeginn:** [Datum]
* **Testende:** [Datum]

## 8. Rollen und Verantwortlichkeiten

* **Testmanager:** [Name]
* **Tester:** [Name]
* **Entwickler:** [Name]

## 9. Abnahmekriterien

* Alle kritischen und hohen Prioritätsfehler sind behoben.
* 95% aller Testfälle sind erfolgreich bestanden.
* Der Code wurde erfolgreich refaktoriert und entspricht den Qualitätsstandards.

## 10. Risiken und Minderungsmaßnahmen

| Risiko | Minderungsmaßnahme |
|---|---|
| Unentdeckte Fehler nach dem Refactoring | Umfassende Testabdeckung, Code-Reviews |
| Zeitüberschreitung des Zeitplans | Priorisierung von Testfällen, zusätzliche Ressourcen |

## 11. Genehmigung

* **Getestet von:** [Name]
* **Datum:** [Datum]
* **Genehmigt von:** [Name]
* **Datum:** [Datum]
