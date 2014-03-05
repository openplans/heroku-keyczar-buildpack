Heroku buildpack: keyczar
=========================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that
vendors [keyczar](http://www.keyczar.org/) requirements.

It is meant to be used in conjunction with other buildpacks as part of a
[multi-buildpack](https://github.com/ddollar/heroku-buildpack-multi).

This buildpack is based on the 
[Heroku geo buildpack](https://github.com/cyberdelia/heroku-geo-buildpack).

Usage
-----

Example usage:

    $ heroku config:add BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git

    $ cat .buildpacks
    https://github.com/openplans/heroku-keyczar-buildpack.git#v1
    https://github.com/heroku/heroku-buildpack-ruby.git#v79


Don't forget to pin buildpack versions you want to use in your .buildpacks file.
