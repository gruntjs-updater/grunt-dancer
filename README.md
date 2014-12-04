# grunt-dancer

> Control your dancer server via Grunt

## Getting Started
This plugin requires Grunt `~0.4.1` 

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-dancer --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-dancer');
```

## The "dancer" task

### Overview
The dancer:serve task can run without configuration by default

####Dancer:serve
Launches the server and whenever the the parent process ends, it terminates the server.

####Dancer:start
Launches the server and leaves it running even when the parent process is no longer running.

####Dancer:kill
Terminates an already running server.

###Options
pidFile

Type: `String`
Default: `'/tmp/dancerServer.pid'`

Path to the pid file in case you wanna run the server by itself.

### Getting Started
In your project's Gruntfile, add `dancer:serve` to the taskList object passed into `grunt.registerTask`.

```js
	grunt.registerTask('local', [
		'concat',
		'uglify',
		'sass',
		'autoprefixer',
		'cssmin',
		'assemble',
		'imagemin',
		'copy',
		'dancer:serve',
		'open:chromium',
		'watch'
	]);
```

##Running tests
To run the test suite, first invoke the following command within the repo, installing the development dependencies:
```shell
$ npm install
```
Then run the tests:
```shell
$ make tests
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Special thanks to 
https://github.com/vjustov for grunt-sinatra
## Release History
_(Nothing yet)_