Unsere Systemarchitektur:

+----------------+          +----------------+          +----------------+          +----------------+
| Datenquellen   |          | Kafka          |          | Spark          |          | Speicher       |
|                |          |                |          |                |          |                |
| +------------+ |          | +------------+ |          | +------------+ |          | +------------+ |
| | Yahoo      | |          | | Yahoo      | |          | | Bereinigung | |          | | Relationale | |
| | Finance    | |  ------> | | Finance    | |  ------> | | und         | |  ------> | | Datenbank   | |
| | Webscraping| |          | | Topic      | |          | | Analyse     | |          | | oder NoSQL  | |
| +------------+ |          | +------------+ |          | +------------+ |          | +------------+ |
| +------------+ |          | +------------+ |          | +------------+ |          | +------------+ |
| | Zillow API | |  ------> | | Zillow     | |  ------> | | Zeitreihen- | |  ------> | | Data Lake   | |
| +------------+ |          | | Topic      | |          | | analyse     | |          | +------------+ |
| +------------+ |          | +------------+ |          | +------------+ |          
| | CSV-Dateien| |  ------> | | HOUST      | |  ------> | | Korrelation | |          
| | (FRED)     | |          | | Topic      | |          | |             | |          
| +------------+ |          | +------------+ |          | +------------+ |          
+----------------+          +----------------+          +------------+ |          
                                                    +------------+ |
                                                    | Vorhersage  |
                                                    | Modelle     |
                                                    |Var od LSTM  |
                                                    +------------+
                                                

+----------------+          +----------------+          +----------------+          +----------------+
| Visualisierung |          | Dokumentation  |          | Multiuser-     |          | Infrastruktur  |
|                |          |                |          | fähige         |          |                |
| +------------+ |          | +------------+ |          | Infrastruktur  |          | +------------+ |
| | matplotlib | |          | | Jupyter     | |          |                |          | | Docker     | |
| | seaborn    | |  <------ | | Notebooks   | |  <------ | +------------+ |  <------ | | Kafka      | |
| | plotly     | |          | +------------+ |          | | Docker      | |          | | Spark      | |
| +------------+ |          |                |          | | Git         | |          | +------------+ |
+----------------+          +----------------+          +----------------+          +----------------+

Data sources:
https://finance.yahoo.com/
https://fred.stlouisfed.org/series/HOUST
https://www.zillow.com/research/data/
https://census.gov/economic-indicators




