# Angustrap

My personnal web app seed project. 
Uses: AngularJS, coffeescript, bootstrap, less, animate.css ... 

## Status

Not ready for use.
To start using:

* `git submodule init && git submodule update`

* `./scripts/web-server.js`

* App code is located in app/coffee

## Noted differences from angular-seed
* The use of coffeescript requires that Angular be [bootstrapped manually](http://docs.angularjs.org/guide/bootstrap).
	* `ng-app` has been removed from `html` element of `index.html`
	* `angular.bootstrap` called in  `app.coffee`
* In `angular-seed` controllers are defined as global functions.  Since coffeescript runs in an anonymous function, the controllers need to be attached directly to the `window` object

## TODOs

* include angular-ui lib
* use Require.js
* Port tests to coffeescript (currently still js)
* add build system
* add modernizr
