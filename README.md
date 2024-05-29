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
