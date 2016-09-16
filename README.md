this is a [FountainJS](http://fountainjs.io/doc) starter set for a new home for Badass. It is built around Gulp,
Webpack and Babel.

All Es6 features in [Babel](https://babeljs.io/docs/learn-es2015/) can be used herein.

Note, global state is no longer accessible in code; all communication must use the
 [Es6 module loader](https://www.sitepoint.com/understanding-es6-modules/).
 
This overhaul comes with a "version bump" for the core packages we are using: specifically,

* Angular 1.5
* ui-router 1.x
* Bootstrap 3.0

The `package.json` is now used in place of Bower to acquire and update packages. 

Also there are command line imperatives to create packages in Angular. an example: 

```` bash

yo fountain-angular2:component --name myComponent --dir components/game

````

# Components

[Components](https://docs.angularjs.org/guide/component) are an Angular feature developed to bridge
Angular 1.5 and Angular 2.x. They are significantly simplfied directives. Use components
over directives going forward, unless direct DOM manipulation is required. They have slightly different binding
rules including one-time (on load) binding.