# Optimal-Electric-Vehicle-Charging-Location-Finder
Constructed an app-based solution aimed at delivering optimal charging locations for EV users in the city of New York leveraging Google Maps data, Flask API, PySpark, and MongoDB in Python.
#Connection to database

import pandas as pd
ev_data_primary = pd.read_csv ('Electric_Vehicle_Charging_Stations_in_New_York.csv')
ev_data_primary

ev_data = ev_data_primary[['Station Name', 'Street Address', 'Latitude', 'Longitude']].copy()
ev_data
