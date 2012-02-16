# [HTML5 Boilerplate](http://html5boilerplate.com) with [Twitter Bootstrap](http://twitter.github.com/bootstrap/)

This is my quick hack of combining these two projects and some additional bits that I tend to reuse. This may be of use to someone else, but more likely than not you will want something similar for your own use.

## Prereqs

	npm install uglify-js
	gem install lessc

## Quick start

Clone the git repo - `git clone git://github.com/pelted/html5-boilerplate.git` - or [download it](https://github.com/pelted/html5-boilerplate/zipball/master)

	git submodule init
	git submodule update

	cd lib/vendor/bootstrap/less/
	lessc bootstrap.less > ../../../../css/bootstrap.css
	lessc responsive.less > ../../../../css/bootstrap-responsive.css
	
	cd ..
	cat js/bootstrap-transition.js js/bootstrap-alert.js js/bootstrap-button.js js/bootstrap-carousel.js js/bootstrap-collapse.js js/bootstrap-dropdown.js js/bootstrap-modal.js js/bootstrap-tooltip.js js/bootstrap-popover.js js/bootstrap-scrollspy.js js/bootstrap-tab.js js/bootstrap-typeahead.js > ../../../js/libs/bootstrap.js
	uglifyjs -nc ../../../js/libs/bootstrap.js > ../../../js/libs/bootstrap.min.js

## Features

* All this bits from HTML5 Boilerplate
* Plus Twitter's Bootstrap css toolkit (as a submodule)


## Project information

* Source: http://github.com/h5bp/html5-boilerplate
* Source: http://github.com/twitter/bootstrap


### Major components:

* jQuery: MIT/GPL license
* Modernizr: MIT/BSD license
* Normalize.css: Public Domain

### Everything else:

The Unlicense (aka: public domain)
