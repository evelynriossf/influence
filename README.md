Introduction
============
This is a fork of a collaborative project(https://github.com/IdeaHaven/influence). This project was developed on a three week timeline.
Below are some notes about code that I specifically contributed to this project.

D3, GeoJSON, and Data Visualization
-----------------------------------
Congressional District Map rendering methods in D3 using GeoJSON:
https://github.com/quetzaluz/influence/blob/master/app/scripts/controllers/district.coffee

Comparative Bar Chart Directive:
https://github.com/quetzaluz/influence/blob/master/app/scripts/directives/compare-bar-chart.coffee

Angular Directives 
------------------
API-Get directive for making AJAX calls to APIs:
https://github.com/quetzaluz/influence/blob/master/app/scripts/services/Api_get.coffee

Sub-template directive (deprecated in favor of ng-include):
https://github.com/quetzaluz/influence/blob/master/app/scripts/directives/sub-view.coffee

Angular Views and associated Stylus - Nib stylesheets
-----------------------------------------------------
Compare View (comparative bar chart directives only):
https://github.com/quetzaluz/influence/blob/master/app/views/compare.html
https://github.com/quetzaluz/influence/blob/master/app/styles/compare_bar_chart.styl

District Map View:
https://github.com/quetzaluz/influence/blob/master/app/views/district_map.html
https://github.com/quetzaluz/influence/blob/master/app/styles/district_map.styl

TDD and Continuous Integration
------------------------------
Karma configuration:
https://github.com/quetzaluz/influence/blob/master/karma.conf.js

Travis CI configuration:
https://github.com/quetzaluz/influence/blob/master/.travis.yml

Testing Package Declarations in package.json:
https://github.com/quetzaluz/influence/blob/master/package.json


Seed Generator
==============
This was created using the [Yeoman Angular Generator](https://github.com/yeoman/generator-angular).  The bootstrap files were replaced with [bootstrap-stylus](https://github.com/Acquisio/bootstrap-stylus) and [Angular UI Bootstrap Directives](http://angular-ui.github.io/bootstrap/)

Quick Start
===========
    `npm install -g bower grunt-cli` unless you have them already
    `npm install`
    `bower install`
    `grunt dev`
    `http://localhost:8080`

How to add new angular modules using yeoman
===========================================
Have [Yeoman](http://yeoman.io/) installed globally
Have [Yeoman Angular Generator](https://github.com/yeoman/generator-angular) installed
Follow the directions [here](https://github.com/yeoman/generator-angular) *USING* flags: `--coffee --minsafe`

Global Package Requirements
===========================
* [Node](http://nodejs.org/)
* after node is installed run: `npm install -g bower grunt-cli yo generator-angular`
 * [Bower](http://bower.io/)
 * [Grunt-CLI](http://gruntjs.com/)
 * yo and angular-generator info the Yeoman Section above

License
=========
Influence is licensed under the [Affero General Public License](LICENSE), which is like the GPL but *requires* you provide access to the source code for any modified versions that are running publicly (among other things). The [intent](http://www.gnu.org/licenses/why-affero-gpl.html) is to make sure that anyone improving the software makes those improvements available to others, as we have to them.
