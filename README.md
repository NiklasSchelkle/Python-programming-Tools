🥇 Data Science Projekt: Analyse Olympischer Erfolgsfaktoren

Dieses Projekt ist eine zweiteilige Datenanalyse, die sich mit verschiedenen Faktoren befasst, die den Erfolg bei Olympischen Spielen beeinflussen. Es nutzt sowohl Athleten-spezifische Daten als auch makroökonomische Indikatoren von Ländern.

Das Projekt ist in zwei separate Jupyter Notebooks unterteilt, die jeweils einen Schwerpunkt beleuchten:
Notebook	Fokus	Methode
SemesterProjekt_1.ipynb	Analyse von Athleten-Merkmalen und deren Zusammenhang mit dem Erfolg.	Explorative Datenanalyse (EDA), deskriptive Statistik.
SemesterProjekt_2.ipynb	Vorhersage der Medaillenanzahl basierend auf sozioökonomischen Indikatoren.	Regressionsanalyse, Nutzung von World Bank Daten.
1. Teil 1: Athleten-Merkmale und Leistung (EDA)

Das erste Projektziel war die Explorative Datenanalyse (EDA), um Korrelationen zwischen den körperlichen Merkmalen von Athleten und ihrem Erfolg (Medaillengewinn) in verschiedenen Sportarten zu untersuchen.
🎯 Zielsetzung

    Identifizieren, in welchen Sportarten bestimmte physische Merkmale (z.B. Körpergröße, Gewicht) einen signifikanten Wettbewerbsvorteil darstellen.

    Beurteilen, ob diese Merkmale bei Medaillengewinnern signifikant von denen der Nicht-Gewinner abweichen.

🛠️ Methodik

    Datenbereinigung: Verarbeitung des Rohdatensatzes der Olympischen Spiele, Fokus auf die Merkmale Height (Größe) und Weight (Gewicht).

    Statistische Analyse: Berechnung von Mittelwerten und Standardabweichungen der Athleten-Merkmale, aufgeschlüsselt nach Sportart und Erfolgsstatus (Gewinner/Nicht-Gewinner).

    Ergebnisanalyse: Spezifische Untersuchung von Sportarten wie Schwimmen, Fünfkampf (Pentathlon) und Kunstturnen (Artistic Gymnastics), um signifikante Abweichungen zu identifizieren.

🔑 Wesentliche Erkenntnisse

Es wurde die vorsichtige Schlussfolgerung gezogen, dass Athleten, die Medaillen gewinnen, tendenziell eher größer sind als der Durchschnitt, wobei in einigen Sportarten (z.B. Schwimmen) die Größe einen deutlicheren Vorteil darstellt als in anderen.
2. Teil 2: Ökonomische Faktoren und Medaillen-Vorhersage

Der zweite Teil konzentriert sich auf die Regressionsanalyse, um den Medaillenspiegel eines Landes auf Basis seiner ökonomischen und sozialen Entwicklung vorherzusagen.
🎯 Zielsetzung

    Ermitteln, welche makroökonomischen Indikatoren (z.B. BIP, Bevölkerungsgröße, Gesundheitsausgaben) die Medaillenleistung eines Landes am stärksten beeinflussen.

    Entwicklung eines Regressionsmodells zur Vorhersage der Anzahl an gewonnenen Goldmedaillen.

🛠️ Methodik

    Datenbeschaffung: Verwendung der wbgapi-Bibliothek, um aktuelle und historische sozioökonomische Indikatoren von der World Bank abzurufen.

    Datenzusammenführung: Verknüpfung der World Bank Indikatoren mit dem historischen Medaillenspiegel der Olympischen Spiele (Zielvariable: Goldmedaillen).

    Modelltraining: Training eines Regressionsmodells (vermutlich Lineare Regression oder ein ähnliches Verfahren) auf den aufbereiteten Daten.

    Validierung: Anwendung des trainierten Modells für eine konkrete Vorhersage (z.B. Goldmedaillen für die Niederlande 2012) zur Überprüfung der Modellgenauigkeit.

💡 Technologie-Stack
Bibliothek/Tool	Zweck
pandas	Datenverarbeitung und -manipulation.
wbgapi	Abrufen von World Bank Daten.
scikit-learn	Regressionsmodelle (Modelltraining und -bewertung).
jupyter	Interaktive Entwicklungs- und Dokumentationsumgebung.
