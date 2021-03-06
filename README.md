# Tracker App

Tracker App is a WebSocket based, event-driven live tracker which helps you track the user in a Google map

### Technologies

Tracker App uses a number of open source projects to work properly:

* [VueJS](https://vuejs.org/) - for Client side programming
* [Twitter Bootstrap](http://twitter.github.com/bootstrap/) - great UI boilerplate for modern web apps
* [WebPack](https://webpack.js.org/) for building the Single Page Application (SPA) and local dev
* [Ratcher PHP](http://socketo.me/) - For Server side websocket connections
* [GoogleMaps](https://developers.google.com/maps/documentation/) - for Maps and user location markers
* [PHP](http://php.net) - for server side programming


### Info
- WebSocket Port: 9090
- WebSocker are being ran by Supervisor 
- [Demo](http://tracker.mycodesamples.com) 

### Config
- Add Google Map API Key in `dist/index.html` or `src/index.html`
- WebSocket port can be changed in `bin/server.php`

### Installation

Tracker App requires [Node.js](https://nodejs.org/) v8+ and [PHP](http://php.net) 7.2+. to run 

Cloning the project source code
```sh
git clone https://github.com/saurabhsrb/live-location-app.git
```
Install the dependencies and devDependencies and start the server.

For Client app
```sh
$ cd live-location-app/public
$ npm install -d
$ node run serve
```

For Building Client app

```sh
$ cd public
$ npm run webpack
```

For Server app 

```sh
$ composer install
$ php bin/server.php
```

Or you can use Supervisor to keep the server app running.
Use `supervisor.conf` for supervisor config

### Todos

 - Write tests for Services and Traits
 - Use Google Map Marker Clusture
 - Saving state of logged in user
 - Use [Radar](https://codepen.io/netsi1964/pen/NALXar/) feature to make it look cool

License
----

MIT
**Free Software, Hell Yeah!**