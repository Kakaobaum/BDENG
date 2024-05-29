### Web Scraping und Analyse von Immobilienpreisen

#### Projektziele:
Unser Ziel ist es, die Immobilienpreisentwicklung in verschiedenen Städten zu analysieren. Wir möchten Muster und Trends identifizieren, um zukünftige Preise vorhersagen zu können. Zusätzlich wollen wir eine visualisierte Übersicht der Ergebnisse bereitstellen.

#### Datenquellen:
1. **Web Scraping:** Immobilien-Webseiten wie Zillow.
2. **API-Daten:** Geografische Daten von OpenStreetMap.
3. **Historische Daten:** Download von Immobilienpreisdaten aus öffentlichen Datenbanken wie Kaggle.

#### Schritte zur Umsetzung:
1. **Datenbeschaffung:**
   - **Web Scraping:** Wir entwickeln ein Python-Skript mit BeautifulSoup oder Scrapy, um aktuelle Immobilienanzeigen zu extrahieren. Diese Daten speichern wir in Kafka.
   - **API-Daten:** Wir nutzen die OpenStreetMap API, um geografische Daten wie Koordinaten, Stadtteile und Infrastruktureinrichtungen zu sammeln und ebenfalls in Kafka zu speichern.
   - **Historische Daten:** Wir laden historische Preisdaten von Kaggle herunter und speichern sie in einer Datenbank.

2. **Datenverarbeitung:**
   - Wir richten eine Kafka-Instanz ein, um die gesammelten Daten zu speichern und zu verwalten.
   - Mit Spark verarbeiten und integrieren wir die verschiedenen Datenquellen.
   - Wir bereinigen und normalisieren die Daten, um eine einheitliche Struktur zu gewährleisten.

3. **Datenanalyse:**
   - Wir führen eine explorative Datenanalyse (EDA) mit Spark durch, um erste Muster und Trends zu identifizieren.
   - Anschließend entwickeln wir Modelle zur Vorhersage zukünftiger Immobilienpreise unter Verwendung von Spark MLlib.

4. **Speicherung und Visualisierung:**
   - Wir speichern die verarbeiteten und analysierten Daten in einer relationalen Datenbank wie PostgreSQL.
   - In einem Jupyter Notebook erstellen wir interaktive Visualisierungen, um die Ergebnisse darzustellen und zu präsentieren.

5. **Dokumentation und Präsentation:**
   - Alle Schritte dokumentieren wir in Jupyter Notebooks, einschließlich Code, Analysen und Visualisierungen.
   - Abschließend präsentieren wir die Ergebnisse in einer Abschlusspräsentation, die unsere Methodik und die gefundenen Erkenntnisse beschreibt.

#### Nützliche Tools und Technologien:
- **Web Scraping:** BeautifulSoup, Scrapy
- **API-Zugriff:** Requests, OpenStreetMap API
- **Datenverarbeitung:** Apache Kafka, Apache Spark
- **Datenanalyse:** Spark MLlib
- **Datenbank:** PostgreSQL

......
.....
...
...
..
.

## PLAN B 
**Analyse der Preisentwicklung bei McDonald's**

**Projektziele:**
Das Ziel dieses Projektes ist es, die Preisentwicklung von McDonald's-Produkten in verschiedenen Regionen zu untersuchen. Durch die Identifizierung von Mustern und Trends in den Preisänderungen über die Zeit streben wir an, zukünftige Preisentwicklungen vorherzusagen. Zusätzlich soll eine visualisierte Darstellung der Analyseergebnisse erstellt werden, um Einsichten leicht zugänglich zu machen.

**Datenquellen:**
- **Web Scraping:** Extraktion von Preisdaten von McDonald's-Produkten von verschiedenen Online-Menüs und Werbeaktionen.
- **API-Daten:** Sammlung geografischer Daten und Standortinformationen von McDonald's-Filialen über Google Maps API.
- **Historische Daten:** Analyse öffentlich zugänglicher Datenbanken und Berichte zu historischen Preisen von McDonald's-Produkten.

**Schritte zur Umsetzung:**
- **Datenbeschaffung:**
  - **Web Scraping:** Entwicklung eines Python-Skripts mit BeautifulSoup oder Scrapy, um aktuelle Preisinformationen zu McDonald's-Produkten zu erfassen. Diese Daten werden in Kafka gespeichert.
  - **API-Daten:** Nutzung der Google Maps API, um Informationen zu Standorten von McDonald's-Filialen zu sammeln.
  - **Historische Daten:** Herunterladen von historischen Preisdaten aus verschiedenen öffentlichen Datenquellen.

- **Datenverarbeitung:**
  - Einrichtung einer Kafka-Instanz zur Speicherung und Verwaltung der gesammelten Daten.
  - Verwendung von Apache Spark zur Verarbeitung und Integration der verschiedenen Datenquellen.
  - Bereinigung und Normalisierung der Daten für eine einheitliche Datenstruktur.

- **Datenanalyse:**
  - Durchführung einer explorativen Datenanalyse (EDA) mit Apache Spark, um erste Muster und Trends aufzudecken.
  - Entwicklung von Prognosemodellen für zukünftige Preise mittels Spark MLlib.

- **Speicherung und Visualisierung:**
  - Speicherung der verarbeiteten und analysierten Daten in einer relationalen Datenbank wie PostgreSQL.
  - Erstellung interaktiver Visualisierungen in einem Jupyter Notebook, um die Ergebnisse zu präsentieren.

- **Dokumentation und Präsentation:**
  - Dokumentation aller Projektschritte in Jupyter Notebooks, einschließlich des Codes, der Analysen und der Visualisierungen.
  - Präsentation der Ergebnisse in einer Abschlusspräsentation, die unsere Methodik und die gewonnenen Erkenntnisse beschreibt.

**Nützliche Tools und Technologien:**
- **Web Scraping:** BeautifulSoup, Scrapy
- **API-Zugriff:** Requests, Google Maps API
- **Datenverarbeitung:** Apache Kafka, Apache Spark
- **Datenanalyse:** Spark MLlib
- **Datenbank:** PostgreSQL
- **Visualisierung:** Matplotlib, Seaborn, Plotly, Jupyter Notebook

## PLAN C
Projektziele:
Unser Ziel ist es, die Entwicklungen auf dem österreichischen Online-Arbeitsmarkt zu analysieren. Wir möchten Muster und Trends in Jobangeboten identifizieren, um Vorhersagen über zukünftige Arbeitsmarkttrends machen zu können. Zusätzlich wollen wir eine visualisierte Übersicht der Ergebnisse bereitstellen.

Datenquellen:
Web Scraping: Jobportale wie karriere.at, willhaben.at.
API-Daten: Geografische Daten von OpenStreetMap.
Historische Daten: Download von Arbeitsmarktdaten aus öffentlichen Datenbanken wie AMS (Arbeitsmarktservice Österreich).

Schritte zur Umsetzung:
Datenbeschaffung:

Web Scraping: Wir entwickeln ein Python-Skript mit BeautifulSoup oder Scrapy, um aktuelle Jobanzeigen zu extrahieren. Diese Daten speichern wir in Kafka.
API-Daten: Wir nutzen die OpenStreetMap API, um geografische Daten wie Koordinaten, Stadtteile und Infrastruktureinrichtungen zu sammeln und ebenfalls in Kafka zu speichern.
Historische Daten: Wir laden historische Arbeitsmarktdaten vom AMS und anderen öffentlichen Quellen herunter und speichern sie in einer Datenbank.
Datenverarbeitung:

Wir richten eine Kafka-Instanz ein, um die gesammelten Daten zu speichern und zu verwalten.
Mit Spark verarbeiten und integrieren wir die verschiedenen Datenquellen.
Wir bereinigen und normalisieren die Daten, um eine einheitliche Struktur zu gewährleisten.
Datenanalyse:

Wir führen eine explorative Datenanalyse (EDA) mit Spark durch, um erste Muster und Trends zu identifizieren.
Anschließend entwickeln wir Modelle zur Vorhersage zukünftiger Trends auf dem Arbeitsmarkt unter Verwendung von Spark MLlib.
Speicherung und Visualisierung:

Wir speichern die verarbeiteten und analysierten Daten in einer relationalen Datenbank wie PostgreSQL.
In einem Jupyter Notebook erstellen wir interaktive Visualisierungen, um die Ergebnisse darzustellen und zu präsentieren.
Dokumentation und Präsentation:

Alle Schritte dokumentieren wir in Jupyter Notebooks, einschließlich Code, Analysen und Visualisierungen.
Abschließend präsentieren wir die Ergebnisse in einer Abschlusspräsentation, die unsere Methodik und die gefundenen Erkenntnisse beschreibt.
Nützliche Tools und Technologien:
Web Scraping: BeautifulSoup, Scrapy
API-Zugriff: Requests, OpenStreetMap API
Datenverarbeitung: Apache Kafka, Apache Spark
Datenanalyse: Spark MLlib
Datenbank: PostgreSQL

Zusätzliche Details zu den einzelnen Schritten:
1. Datenbeschaffung:
   - Web Scraping: Spezielle Parser entwickeln, um relevante Informationen wie Jobtitel, Unternehmen, Standort, Gehalt und Anforderungen aus den Jobportalen zu extrahieren.
   - API-Daten: Abruf von Geodaten und infrastrukturellen Informationen zur besseren geografischen Analyse der Jobdaten.
   - Historische Daten: Sammlung und Strukturierung der historischen Arbeitsmarktdaten, um Trends im Zeitverlauf zu analysieren.

2. Datenverarbeitung:
   - Kafka-Instanz: Einrichtung einer Kafka-Pipeline zur kontinuierlichen Erfassung und Speicherung der Daten.
   - Datenintegration: Zusammenführung der verschiedenen Datenquellen in einer kohärenten und strukturierten Form.
   - Datenbereinigung: Umgang mit fehlenden Werten, Duplikaten und Inkonsistenzen, um die Datenqualität zu gewährleisten.

3. Datenanalyse:
   - EDA: Untersuchung der Daten mit statistischen Methoden und Visualisierungen, um erste Erkenntnisse zu gewinnen.
   - Modellierung: Anwendung von Machine Learning Modellen zur Prognose zukünftiger Arbeitsmarkttrends basierend auf historischen und aktuellen Daten.

4. Speicherung und Visualisierung:
   - Datenbank: Aufbau einer robusten Datenbankstruktur zur Speicherung der bereinigten und analysierten Daten.
   - Visualisierung: Entwicklung interaktiver Dashboards und Grafiken in Jupyter Notebooks, um die Ergebnisse verständlich zu präsentieren.

5. Dokumentation und Präsentation:
   - Jupyter Notebooks: Detaillierte Dokumentation aller Schritte und Ergebnisse, um die Reproduzierbarkeit und Nachvollziehbarkeit zu gewährleisten.
   - Präsentation: Erstellung einer abschließenden Präsentation zur Vorstellung der Methodik und der gewonnenen Erkenntnisse.

Durch die strukturierte Vorgehensweise und den Einsatz moderner Technologien schaffen wir eine fundierte Basis für die Analyse und Vorhersage von Trends auf dem österreichischen Online-Arbeitsmarkt.
