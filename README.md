# Angustrap

My personnal web app seed project. 
- It's based on AngularJS, coffeescript and less. 
- Uses git submodules inside /lib directory for project dependencies
- Customizable scripts for rapid web development 


## Status

To start using, just clone this repo then init the submodules. 

* `git submodule init && git submodule update`

To run the dev server:

`./scripts/web-server.js`

- Application code is located in app/coffee

## Noted differences from angular-seed
* The use of coffeescript requires that Angular be [bootstrapped manually](http://docs.angularjs.org/guide/bootstrap).
	* `ng-app` has been removed from `html` element of `index.html`
	* `angular.bootstrap` called in  `app.coffee`
* In `angular-seed` controllers are defined as global functions.  Since coffeescript runs in an anonymous function, the controllers need to be attached directly to the `window` object

## TODOs

- include angular-ui lib
- use Require.js
- Port tests to coffeescript (currently still js)
- add build system
- add modernizr
- Update loader.js/$script.js | [@angular/angular-seed #40](https://github.com/angular/angular-seed/issues/40)
