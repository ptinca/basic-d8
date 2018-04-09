
DRUPAL 8 BASIC THEME
--------------------

 * About this theme
 * Installation
 * Structure
 * Fonts


ABOUT THIS THEME
----------------
This is a basic Drupal 8 theme to get you quickly started with theming.


INSTALLATION
------------
1. Download this theme into your themes directory and rename all instances of 
   "themename" to your theme name. 
2. Install node modules to get Gulp tasks working (the lines below will install
   all needed modules and run all initial tasks including the watcher task):
   
   cd .npm
   npm install
   gulp


STRUCTURE
---------

Gulp
----
.npm
    |-- gulp
        |-- tasks
            |-- scripts.js
            |-- styles.js
            |-- watch.js
        |-- config.json
    |-- gulpfile.js
    |-- package.json

Inside the .npm/gulp folder are .js files for each task and a config.json file
which contains notification messages, input/output file names for compiler,
autoprefixer settings, etc. All these files are then pulled into the gulpfile.js
file where we define the dependencies, load modules and prepare the tasks.

Gulp tasks:
  gulp scripts
  gulp styles
  gulp build
  gulp watch


Source files
------------
sass
    |-- base
        |-- grid
    |-- design
    |-- vendor
    |-- style.scss
scripts
    |-- app
        |-- main.js

All source files are located inside sass and scripts folders. Any JS vendor
files should go directly into assets/scripts/vendor folder. Any SCSS vendor
files should go into sass/vendor folder and should also be imported into
sass/vendor/vendor.scss file so they can be compiled with the rest of the files.


Assets
------
assets
    |-- fonts
    |-- images
    |-- scripts
        |-- vendor
    |-- stylesheets


FONTS
-----
Use rem
1rem is 10px
