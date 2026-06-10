# Testplan für GildedRose-Refactoring-Kata

Dieser Testplan beschreibt die Strategien und durchzuführenden Tests für das Repository GildedRose-Refactoring-Kata.

## Zielsetzung

Das Ziel dieses Testplans ist es, die Qualität und Korrektheit des Codes im GildedRose-Refactoring-Kata-Repository sicherzustellen. Wir werden verschiedene Teststrategien anwenden, um sicherzustellen, dass alle Funktionalitäten wie erwartet funktionieren und Refactoring-Änderungen keine Regressionen einführen.

## Teststrategien

1.  **Unit Tests:** Überprüfung einzelner Komponenten und Funktionen, um deren korrekte Ausführung sicherzustellen.
2.  **Integration Tests:** Sicherstellung, dass verschiedene Komponenten des Systems ordnungsgemäß zusammenarbeiten.
3.  **Regression Tests:** Erneutes Ausführen von Tests nach Codeänderungen (insbesondere nach Refactoring), um sicherzustellen, dass keine neuen Fehler eingeführt wurden.
4.  **Akzeptanztests:** Überprüfung, ob das System die Geschäftsanforderungen erfüllt.

## Testfälle

### 1. Unit Tests

*   **Artikel-Aktualisierung:**
    *   Überprüfen Sie die Aktualisierung des 'normalen' Artikels (Name, Verfallsdatum, Preis).
    *   Überprüfen Sie die Aktualisierung von 'Aged Brie'.
    *   Überprüfen Sie die Aktualisierung von 'Sulfuras, Hand of Ragnaros'.
    *   Überprüfen Sie die Aktualisierung von 'Backstage passes to a TAFKAL80ETC concert'.
    *   Überprüfen Sie die Aktualisierung von Artikeln, deren Verfallsdatum weniger als 0 Tage beträgt.
    *   Überprüfen Sie die Aktualisierung von Artikeln, deren Verfallsdatum zwischen 0 und 10 Tagen liegt.
    *   Überprüfen Sie die Aktualisierung von Artikeln, deren Verfallsdatum zwischen 10 und 15 Tagen liegt.
*   **Preis- und Verfallsdatumsbeschränkungen:**
    *   Sicherstellen, dass der Preis nicht über 50 steigt.
    *   Sicherstellen, dass der Preis nicht negativ wird (außer bei 'Sulfuras').
    *   Sicherstellen, dass das Verfallsdatum korrekt verringert wird.

### 2. Integration Tests

*   Überprüfen Sie den gesamten Aktualisierungsprozess für eine Liste von Artikeln.
*   Stellen Sie sicher, dass die Interaktion zwischen verschiedenen Artikeltypen korrekt gehandhabt wird.

### 3. Regression Tests

*   Führen Sie alle Unit- und Integrationstests nach jeder signifikanten Codeänderung oder jedem Refactoring aus.
*   Vergleichen Sie die Ergebnisse vor und nach der Änderung, um unerwünschte Nebenwirkungen zu erkennen.

### 4. Akzeptanztests

*   Simulieren Sie verschiedene Szenarien (z. B. tägliche Aktualisierungen über einen längeren Zeitraum) und überprüfen Sie die Endzustände der Artikel.
*   Vergleichen Sie die Ausgabe des Systems mit erwarteten Ergebnissen basierend auf den Geschäftsanforderungen.

## Fehlende Testfälle und Issues

Basierend auf einer ersten Untersuchung des Repositories scheint es, dass möglicherweise nicht alle oben genannten Testfälle explizit implementiert sind. Es wird empfohlen, die vorhandenen Tests zu überprüfen und gegebenenfalls Issues für fehlende Testfälle zu erstellen.

**Vorschläge für Issues (falls zutreffend):**

*   "Fehlender Unit Test: Überprüfung der Preisobergrenze von 50 für alle Artikeltypen."
*   "Fehlender Unit Test: Überprüfung, ob der Preis von 'Sulfuras' niemals geändert wird."
*   "Fehlender Integration Test: Umfassende Überprüfung des täglichen Aktualisierungsprozesses für eine gemischte Liste von Artikeln."
