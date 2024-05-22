### Web Scraping und Analyse von Immobilienpreisen

#### Projektziele:
Unser Ziel ist es, die Immobilienpreisentwicklung in verschiedenen Städten zu analysieren. Wir möchten Muster und Trends identifizieren, um zukünftige Preise vorhersagen zu können. Zusätzlich wollen wir eine visualisierte Übersicht der Ergebnisse bereitstellen.

#### Datenquellen:
1. **Web Scraping:** Immobilien-Webseiten wie Zillow oder ImmobilienScout24.
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
- **Visualisierung:** Matplotlib, Seaborn, Plotly, Jupyter Notebook
