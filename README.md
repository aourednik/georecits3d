# GéoRécits3D: mapping journeys in space-time

![GéoRécits journeys](img/georecits3d.png)

Spatial mobility always involves at least two types of distances:

- the _topographical distance_ traveled on the surface of the Earth and
- the _time distance_ taken to do so.

GéoRécits3D allows you to map both in a space-time cuboid. 

## D3js and threejs

It is written using HTML5 and JavaScript, and uses the visualisation frameworks [D3js](https://github.com/d3/d3),version 5 and [threejs](https://github.com/mrdoob/three.js).

## Documentation

To run the app, simply __open _index.html___ with a web browser. With Firefox, the app can run locally.

By default, the app fetches its data from the _/data_ folder. You can specify another folder in your navigator by adding a ```?datafolder=your/datafolder```to the url. Example :

http://your.host/georecits3d/index.html?datafolder=data_examples/migration

or, locally

file:///your/path/to/georecits3d/index.html?datafolder=data_examples/migration

### Configuration files

Configuration csv files for journeys identical to those of [GéoRécits](https://github.com/aourednik/georecits) can be used.

- [Full documentation HERE](https://ourednik.info/georecits3d/)

- [Running example HERE](https://ourednik.info/georecits3d/v01/)

![GéoRécits journeys](img/georecits3d.gif)

### Chrome and Safari

Géorectis3D needs to access local files. This is not allowed in Chrome and Safari. This means it either needs to be uploaded to a server _or_ you can also run a local server, for instance with the following commands in your terminal:

```bash
cd your/path/to/georecits3d/
python3 -m http.server
```

The terminal should then aswer

```bash
Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/) ...
```
The app can then be run by accessing the given url, i.e. http://0.0.0.0:8000/.