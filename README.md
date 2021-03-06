## GhostBus API

###Intro

This is the Flask API part of a semester long project called "Ghost Bus" - an augmented reality experience for the MTA B54 bus route. The project involves augmenting the bus' real-time location for riders to be able to visualise how close/far the bus is from their stop. 

This simple web app will interact with the MTA SIRI API to grab B54 bus data. It will then parse the data and communicate with the Unity3D project in order to reflect the moving bus.

###Deploy in the Console 

```
python app.py
```

You'll probably need [python](https://www.python.org/) and [pip](https://github.com/pypa/pip) 

###Deploy the Flask API

The Flask API is still in testing!
To run:
```
python testappserver.py
```
which uses the methods in testapp.py.

###Usage

You can use this for any GTFS feed from the [SIRI API](http://bustime.mta.info/wiki/Developers/SIRIVehicleMonitoring)
though you'll have to handle parsing it accordingly.
```
response = urllib2.urlopen('the-API-call-URL')
```

###Inspiration

The GhostBus API was built using this [flask and python example for Playstation games](https://github.com/falfaro/flask-example)


