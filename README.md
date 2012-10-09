Apache + PHP + Grunt
====================

This is a buildpack combining the [PHP](https://github.com/heroku/heroku-buildpack-php) and [NodeJS](https://github.com/heroku/heroku-buildpack-nodejs) buildpacks, which allows for an on-deploy Grunt build.

Configuration
-------------

Refer to [this repo](https://github.com/gcpantazis/template-heroku-php-gruntjs) for a working template that utilizes this project.

Use the following command (more info [here](https://devcenter.heroku.com/articles/buildpacks#using-a-custom-buildpack)) to initialize heroku with the buildpack:

`$ heroku create --buildpack https://github.com/gcpantazis/heroku-buildpack-php-gruntjs.git`

The buildpack expects that you set a package.json file at your project's root for node/npm configuration, and keep a separate package.json alongside your gruntfile in `/build`.

License
-------

Copyright (c) 2012 George Pantazis Licensed under the MIT license.
