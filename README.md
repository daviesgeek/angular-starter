##Angular Starter app

This is a super simple starter app for getting started with Angular.

### Installation

To install this, first clone this repository:

```bash
git clone git@github.com:daviesgeek/angular-starter.git
cd angular-starter
```

Then install the npm dependencies:

```bash
npm install
```

And the Bower dependencies:

```bash
bower install
```

### Features

Technology:
 - Brunch - For compiling the source
 - Bower - For managing frontend dependencies
 - LESS - Instead of CSS (though CSS is also supported)
 - Jade - Instead of HTML (though HTML is also supported)

Frontend:
 - AngularJS (~1.2.25)
 - jQuery (~2.1.1)
 - UI Router - Instead of ngRoute
 - Restangular - Instead of $http

###Directory Structure

```
_public              --> This is where Brunch compiles your app (no need to touch this)
  css
  js
  index.html
app                  --> This is where all the magic happens. All your source files for the app go here
  assets             --> Assets in this folder will be copied (unmodified) into the '_public' folder
  common
    directives       --> Directives are placed here
    resources        --> Restangular resources belong here
      cool-thing.js  --> A test service to show off what Restangular can do
    services         --> Angular factories/singletons (that are not Restangular resources)
  configuration      --> This is the configuration object that is globally available within your app
  routes             --> All of the routing goes here
    controllers
    views
  styles             --> Stylesheets
    main.less
bower_components     --> The directory to which Bower installs all the necessary dependencies
node_modules         --> The directory to which npm installs all the necessary dependencies
bower.json           --> Bower dependency configuration
config.js            --> Brunch compiling configuration
package.json         --> Npm dependency configuration
```