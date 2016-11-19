# XWebGo V1

### What is it?

XWebGo is a web framework written in Javascript (NodeJS) for easy creation and deployment of custom maps (crowdsourced, private...). Its first purpose was the agregate data from users to provide a live an accurate map visualization. It has then been extended to handle more use case and to be easlily deployable by someone with 0 developping skills.

See [XWebGo] for more informations.

### Specifications

NodeJS V XX.XXX
MongoDB V XX.XX

The V1 of XWebGo Open Source is the core of the original [https://www.pokewebgo.com] website from PokeWebGo Team. As such, it contains a subset of the original application features.

### Features

Custom type of data that can be filtered
Data Expiration
Vote system
Account creation support with email confirmation
Simple UI set
Sample data
Google Maps Support

### Sample data

You can test XWebGo with a provided sample data set, courtesy of XWebGo Team.

The sample data is here : https://github.com/XWebGo/XWebGo-sample-data

It includes :

DataSet for Pokemon Go
4 types of data : Pokemons that can be filter/multifiltered by type, Pokestops (static), Gyms (Who's specific info can be change from time to time), Meetings (links with expiration date)
Sample UI
Database dump

### Getting started

Instructions below will differ depending on whether you just want to run the demo locally, or start developping (and then run the demo in development mode).

### Running the demo locally

Be sure to have a working NodeJS server [https://nodejs.org/en/download/] and MongoDB server [https://www.mongodb.com/download-center] before continuing.

To get a quick idea of what XWebGo is, just type in what follows in the command line:

```
git clone -b gh-pages https://github.com/XWebGo/master.git
git clone https://github.com/XWebGo/XWebGo-sample-data
```

The first command just clones this repository. The second one clones the sample data repository then launch a simple HTTP serveur on your machine on port 8000 (choose another available port if 8000 is already in use).

Then just point your web browser at http://localhost:8000/XWebGo-sample-data/ and enjoy!

### Building XWebGo

To build XWebGo, make sure you have Node.js and NPM [https://nodejs.org/en/download/] installed, clone the repository, then open a console and type (from the directory you cloned the XWebGo repository into):

```
npm install
npm run build
```

This will produce an optimized, bundled XWebGo.js in the dist/ directory.

Note that if you already cloned the repository from the “Running the demo locally” instructions, you'll have to checkout the master branch (above instructions did checkout the gh-pages instead, which contains a prebuilt version of XWebGo).

### Run the demo in development mode

To run the demo in development mode, you need to clone the sample data repository next to the XWebGo repository.

If you initially followed the “Running the demo locally” instructions, you're all setup; otherwise, run the following commands:ito

```
cd ..
git clone https//github.com/XWebGo/XWebGo-sample-data.git
cd -
```

Then run:

```
npm start
```
and open http://localhost:8080/XWebGo-sample-data/ (note that the port is different from the “Running the demo locally” instructions)

Any change to a source file will automatically trigger a reload of the demo in the browser. The webpack-dev-server that is launched by the npm start command builds the project on-the-fly (and in-memory) and generates source-maps for easy debugging in your browser. Note however that the code you run in the browser is not directory the code from the source files, it has been processed by webpack.

To change the port the server listens on, pass additional -- --port PORT arguments, e.g.

```
npm start -- --port 8000
```

### Roadmap items

The following tasks are currently worked on :

Code simplification
Documentation
Offline examples
3rd parties maps integration (OpenStreetMap, Bing Maps, Ersi
Module System


### Support

XWebGo is an original work from XWebGo, it is self founded by the PokeWebGo founders.

XWebGo is currently maintained by XWebGo Team.
