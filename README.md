# HoneyTrap![light.png](img/light.png)
HoneyTrap is a cybersecurity system used to trap, get, and analyze attacker data. Depends on the integration of SIEM solutions and the Honeypot system.
Honeypots are a system that is built and configured in order to be hacked, so they
are deployed within the system in order to help consume the attacker's resources,
exploit his time, and divert his attention away from the systems.
It also provides a working environment for studying the techniques and methods
used by attackers on the system.
It is important to monitor all activities in this area, and by definition, every activity
in this area is an attack.![Screenshot 2024-10-01 103728.png](img/Screenshot%202024-10-01%20103728.png)
# Here are some of the key motivations that led to the development of the honeytrap:
1. Threat Detection and Analysis
2. Incident Response and Forensics
3. Research and Threat Intelligence
4. Vulnerability Identification
5. Training and Skill Development



# DATA
## Phases of manipulating the data:
1. searching for the data sources
![Picture1.png](img/Picture1.png)
2. data access and authorization
3. data extraction.  
![Picture2.png](img/Picture2.png)
4. data exploration
5. data selection
6. data preprocessing: [ETL , Data cleaning and Web scraping]
![Picture3.png](img/Picture3.png)
7. data syncronization
8. data visualization
# Code
## data_syncronyzer.py:
### Data Synchronizer Script
This Python script is designed to synchronize data between various sources and a local SQLite database. It includes several key functionalities to ensure efficient and accurate data management:

Key Features:
1. IP location using Web scraping:
  Geolocation Retrieval: Utilizes the IP2Location API to fetch geographical coordinates (latitude and longitude) for given IP addresses.
  Data Storage: Stores the retrieved geolocation data in the local SQLite database for future reference and analysis.
  Data Extraction:
2. Source Database Connection: Connects to an external database to extract relevant data.
  Incremental Data Extraction: Ensures only new or updated data is extracted by comparing timestamps or unique identifiers.
3.  Data Transformation:
  Normalization: Normalizes IP addresses and other data fields to ensure consistency.
  Preprocessing: Preprocesses the extracted data to remove duplicates, handle missing values, and format data appropriately.
4.  Data Loading:
  Local Database Integration: Loads the transformed data into a local SQLite database.
5.  Error Handling: Implements robust error handling to manage issues during data extraction, transformation, and loading processes.
6. Synchronization and early detection .
   
Dependencies:
Python 3.x
SQLite
IP2Location API
Other dependencies listed in requirements.txt

## Honeydash.py Dashboard

This project is a comprehensive web-based dashboard designed for monitoring and visualizing data from a honeypot system. It leverages **Dash** and **Plotly** for creating interactive visualizations and **SQLite** for data storage.
![Screenshot 2024-10-01 103728.png](img/Screenshot%202024-10-01%20103728.png)

### Key Features

1. **Real-time Data Visualization**:
   - **Dynamic Updates**: Continuously updates the dashboard with real-time data from the honeypot system.
   - **Log Display**: Shows detailed logs of events captured by the honeypot, including timestamps, IP addresses, and event types.

2. **Risk Assessment**:
   - **Risk Gauges**: Displays risk levels using interactive gauges and indicators.
   - **Alert System**: Highlights critical events and potential threats in real-time.

3. **Interactive Charts**:
   - **Bar Charts**: Visualizes the frequency of different types of events.
   - **Line Charts**: Tracks trends over time, such as the number of attacks per day.
   - **Geographical Maps**: Plots the origin of attacks on a world map for geographical analysis.

4. **Ping Indicators**:
   - **Network Status Monitoring**: Monitors the status of various network components and displays their current state.
   - **Health Indicators**: Provides visual indicators for the health and performance of the honeypot system.


### Dependencies

- **Python 3.x**
- **Dash**
- **Plotly**
- **SQLite**
- **Other dependencies listed in `requirements.txt`

