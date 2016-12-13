### Getting started
>  **Todo:** Add q quick getting started guide that covers:
>
	>	1. Project directory Structure
	>	2. How to install [npm gulp,](https://www.npmjs.com/package/gulp "'gulp installation")[gulp - sass,](https://www.npmjs.com/package/gulp-sass "intall scss")[npm bootraps](https://forums.meteor.com/t/the-way-to-use-bootstrap-4-from-npm-including-js-and-tether/23159 "download bootraps")
	>	3. Guideline for [npm](https://www.npmjs.com/package/npm) 
		
		
### Installation

 ``` npm install  ``` or   ```npm install --production ```
#####This will install node modules needed by app(adding  ``` --production  ``` param is optional if you will not use nodes as the server) Post install will execute these commands automatically:  ``` bower install  ``` and  ``` gulp uikit:install  ```

### Gulp - sass
```npm install gulp-sass --save-dev```
> **basic usage**
> Something like this will compile your Sass files:
>  > 'use strict';
		var gulp = require('gulp');
		var sass = require('gulp-sass');
		 gulp.task('sass', function () {
		  return gulp.src('./sass/**/*.scss')
	    .pipe(sass().on('error', sass.logError))
	    .pipe(gulp.dest('./css'));
	}); 
		gulp.task('sass:watch', function () {
	  gulp.watch('./sass/**/*.scss', ['sass']);
	});
	
> You can also compile synchronously, doing something like this:
>   >'use strict';
	var gulp = require('gulp');
	var sass = require('gulp-sass');
	gulp.task('sass', function () {
	 return gulp.src('./sass/**/*.scss')
	   .pipe(sass.sync().on('error', sass.logError))
	   .pipe(gulp.dest('./css'));
	});
	gulp.task('sass:watch', function () {
	 gulp.watch('./sass/**/*.scss', ['sass']);
	});


### Npm - bootrap
```npm install --save bootstrap@4.0.0-alpha.2```
> **1. To use Bootstrap 4 styles: **
	>Run this in your terminal or secure shell:
	> >npm install --save bootstrap@4.0.0-alpha.2
		meteor add fourseven:scss
		
>Create a main.scss in any place in client folder like client/styles/main.scss.
	Inside of main.scss, write
	> >@import "{}/node_modules/bootstrap/scss/bootstrap.scss";
	
>on top
### Gulp Build tasks
 ``` gulp  ``` or  ``` gulp default  ```
##### This task builds the bare necessary to run the app. No minifications or whatsoever.
 ``` gulp watch  ```
##### Development mode on, watches the source directories and run tasks on file change.
**Task that makes up  ``` default  ``` and  ``` watch tas  ```

1. ``` gulp  bower  ```   Project how to
2.  ``` gulp angular  ```  Yes
3.  ``` gulp uikit ```  First ordered list item
4.  ``` gulp test ```  First ordered list item


for all task , you may  optionally pass parameters succh as:			
	 ``` --clean:  ``` to wipe application files from the targer directoryasa

  

