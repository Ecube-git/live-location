# live-location
It is coded in python 3.8 
this is the following code


import googelmaps
from datetime import datetime

gmaps = googlemaps.Client(key='your client id ')

# Geocoding an address
geocode_result = gmaps.geocode('1600 Amphitheatre 
                                  Parkway, Mountain
                                  View, CA')

# Look up an address with reverse geocoding
reverse_geocode_result = gmaps.reverse_geocode((40.714224, -73.961452))

# Request directions via public transit
now = datetime.now()
directions_result = gmaps.directions("Sydney Town Hall",
                                     "Parramatta, NSW",
                                     mode="transit",
                                     departure_time=now)
