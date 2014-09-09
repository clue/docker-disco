# docker-disco

[Disco](https://github.com/carlwoodward/disco) is a simple visual GitHub browser.
This is a [docker](https://www.docker.io) image that eases setup.

## Usage

This docker image is available as a [trusted build on the docker index](https://index.docker.io/u/clue/disco/),
so there's no setup required.
Using this image for the first time will start a download automatically.
Further runs will be immediate, as the image will be cached locally.

The recommended way to run this container looks like this:

```bash
$ docker run -d -p 80:8080 clue/disco
```

The above example exposes the Disco webinterface on port 80, so that you can now browse to:

```
http://localhost/#/clue/graph
```

This is a rather common setup following docker's conventions:

* `-d` will run a detached instance in the background
* `-p {OutsidePort}:8080` will bind the webserver to the given outside port
* `clue/disco` the name of this docker image

