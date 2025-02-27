# Heroku_Buildpack_-ffmpeg_ffprobe

======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks)
for adding ffmpeg and ffprobe to your application.

Multipacks
----------

More likely, you'll want to use it as part of a larger project, which needs to use ffmpeg and ffprobe. The easiest way to do this is with a [multipack](https://github.com/ddollar/heroku-buildpack-multi),
where this is just one of the buildpacks you'll be working with.

Thanks to [jonathanong](https://github.com/jonathanong) for static build of [ffmpeg](https://johnvansickle.com/ffmpeg/)

    $ cat .buildpacks
    git://github.com/heroku/heroku-buildpack-ruby.git
    git://github.com/EthernaxD/Heroku_Buildpack_-ffmpeg_ffprobe.git

    $ heroku buildpacks:add https://github.com/ddollar/heroku-buildpack-multi

By this you can use ffmpeg and ffprobe command.

### Another method
    heroku buildpacks:add https://github.com/EthernaxD/Heroku_Buildpack_-ffmpeg_ffprobe
