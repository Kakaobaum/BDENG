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
| | Zillow CSV | |  ------> | | Zillow     | |  ------> | | Zeitreihen- | |  ------> | | Data Lake   | |
| +------------+ |          | | Topic      | |          | | analyse     | |          | +------------+ |
| +------------+ |          | +------------+ |          | +------------+ |          
| | FRED-API   | |  ------> | | HOUST      | |  ------> | | Korrelation | |          
| | indicators | |          | | Topic      | |          | |             | |          
| +------------+ |          | +------------+ |          | +------------+ |          
+----------------+          +----------------+          +------------+ |          
                                                    +--------------+ 
                                                    | Vorhersage   |
                                                    | Modelle      |
                                                    |Random Forest |
                                                    +--------------+
                                                

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
https://www.datacamp.com/tutorial/lstm-python-stock-market
https://machinelearningmastery.com/time-series-prediction-lstm-recurrent-neural-networks-python-keras/
https://de.wikipedia.org/wiki/Vektorautoregressive_Modelle
https://scikit-learn.org/


