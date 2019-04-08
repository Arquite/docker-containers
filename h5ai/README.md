# h5ai

This is a fork of h5ai from [smdion/docker-h5ai](https://github.com/smdion/docker-containers/tree/master/h5ai), with an updated version of h5ai, and is intended for use on unRAID docker.

[h5ai](http://larsjung.de/h5ai/) is a modern web server index.
This [docker](https://www.docker.io/) image makes it trivially easy to
spin up a webserver and start sharing your files through the web.

See also the [demo directory](http://larsjung.de/h5ai/sample).

## Usage

docker run -p 8888:80 --name=h5ai -v /path/of/directory/to/share:/var/www -v /path/to/config:/config virtike/docker-h5ai

## Reverse Proxy

I put it behind an nginx reverse proxy to manage & protect access
