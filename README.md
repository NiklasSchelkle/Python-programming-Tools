# Data Science Projekt: Analyse olympischer Erfolgsfaktoren

Dieses Projekt umfasst eine zweistufige quantitative Analyse der Faktoren, die den sportlichen Erfolg bei Olympischen Spielen beeinflussen. Die Untersuchung kombiniert athletenspezifische Biometrie mit makroökonomischen Indikatoren auf Länderebene.

Das Projekt ist in zwei dedizierte Jupyter Notebooks unterteilt:

| Datei | Fokus | Methodik |
| :--- | :--- | :--- |
| **SemesterProjekt_1.ipynb** | Biometrische Merkmale von Athleten und deren Korrelation zum Erfolg. | Explorative Datenanalyse (EDA), Deskriptive Statistik. |
| **SemesterProjekt_2.ipynb** | Prädiktion der Medaillenanzahl basierend auf sozioökonomischen Indikatoren. | Regressionsanalyse, World Bank Data Integration. |

---

## 1. Teilprojek: Athleten-Merkmale und Leistung (EDA)

Das primäre Ziel dieses Teilprojekts ist die Untersuchung der Korrelation zwischen physischen Attributen und dem Gewinn von Medaillen in verschiedenen Disziplinen.

### Zielsetzung
* Identifikation von Sportarten, in denen biometrische Merkmale (z. B. Körpergröße, Gewicht) einen signifikanten Wettbewerbsvorteil darstellen.
* Statistische Überprüfung, ob sich Medaillengewinner in ihren physischen Ausprägungen signifikant von Nicht-Gewinnern unterscheiden.

### Methodik
* **Datenbereinigung:** Prozessierung des olympischen Rohdatensatzes mit Fokus auf die Variablen *Height* (Körpergröße) und *Weight* (Gewicht).
* **Statistische Analyse:** Berechnung von Lagemaßen (Mittelwerte) und Streuungsmaßen (Standardabweichungen), differenziert nach Sportart und Erfolgskategorie.
* **Disziplinspezifische Untersuchung:** Detaillierte Analyse ausgewählter Sportarten wie Schwimmen, Moderner Fünfkampf und Kunstturnen zur Verifizierung signifikanter Abweichungen.

### Wesentliche Erkenntnisse
Die Analyse deutet darauf hin, dass Medaillengewinner tendenziell eine überdurchschnittliche Körpergröße aufweisen. Dieser Effekt variiert je nach Disziplin und ist beispielsweise im Schwimmsport deutlich ausgeprägter als in anderen Sportarten.

---

## 2. Teilprojekt: Ökonomische Faktoren und Medaillen-Vorhersage

Der zweite Teil nutzt Regressionsmodelle, um die Medaillenbilanz eines Landes auf Basis seiner ökonomischen und sozialen Entwicklung zu prognostizieren.

### Zielsetzung
* Bestimmung der einflussreichsten makroökonomischen Indikatoren (z. B. BIP, Bevölkerungszahl, Gesundheitsausgaben) auf die sportliche Performance.
* Entwicklung eines prädiktiven Modells zur Vorhersage der Anzahl gewonnener Goldmedaillen pro Nation.

### Methodik
* **Datenakquise:** Automatisierter Abruf sozioökonomischer Zeitreihen der Weltbank mittels der `wbgapi`-Schnittstelle.
* **Feature Engineering:** Zusammenführung der Weltbank-Indikatoren mit historischen Medaillendaten (Zielvariable: Anzahl Goldmedaillen).
* **Modellierung:** Training und Optimierung eines Regressionsmodells zur Abbildung linearer oder nicht-linearer Zusammenhänge.
* **Validierung:** Prüfung der Modellgüte durch konkrete Vorhersage-Szenarien (z. B. Validierung anhand der Resultate der Niederlande im Jahr 2012).

---

## Technologie-Stack

| Bibliothek / Tool | Verwendungszweck |
| :--- | :--- |
| **pandas** | Datenprozessierung und Transformation. |
| **wbgapi** | Programmatischer Zugriff auf die World Bank Datenbank. |
| **scikit-learn** | Implementierung, Training und Evaluation der Regressionsmodelle. |
| **jupyter** | Dokumentation und interaktive Entwicklungsumgebung. |

---
*Erstellt im Rahmen eines akademischen Projekts zur Statistischen Analyse.*
