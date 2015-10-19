WebPack Fundementals

Why build client code (JavaScript) - since it's interpreted by browswer
	- Combining files - better to send one .js file instead of bunch http request (transmission size)
	- Minification
	- Maintaining file order
	- Transilation
	- linting - getting rid of unnecessary params in functions etc

WebPack - specialized task runner
	- processing input files into output files
	- send one or more files and webpack will perform minification, transilation, combining etc (even combine css + js into one file)

Module System - express dependencies on files
	Concerts.js depends on => Bands.js => Backbone.js => jQuery.js etc

	Concerts.js
		var bands = require('./Bands');
		var backbone = require('./Backbone');

Runnig WebPack

> npm install webpack -g
> webpack ./app.js bundle.js => take my app.js file and bundle it to bundle.js file
> webpack => webpack.config.js configuration file settings

watchmode => webpack automatically re-runs build
> webpack --watch // first way

Dev Server => refreshes browser whenever an update is made to app.js
> webpack-dev-server

