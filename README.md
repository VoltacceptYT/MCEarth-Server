[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](LICENSE)

Introduction
-------------

This repo holds the code for the Project Earth server.
It is built on Cloudburst and has a few key advantages over other server software:

* Written in Java, Cloudburst is faster and more stable.
* Having a friendly structure, it's easy to contribute to Cloudburst's development and rewrite plugins from other platforms into Cloudburst plugins.

Cloudburst is **under improvement**.

Links
--------------------

* __[Download](#)__

Build JAR file
-------------
- `git clone https://github.com/CloudburstMC/Server.git`
- `cd Server`
- `git submodule update --init`
- `./mvnw clean package`

The compiled JAR can be found in the `target/` directory.

Running
-------------
Simply run `java -jar Cloudburst.jar`.

Plugin API
-------------
Information on Cloudburst's API can be found at the [wiki](https://cloudburstmc.org/wiki/cloudburst/).

Docker
-------------

Running Nukkit in [Docker](https://www.docker.com/) (17.05+ or higher).

Build image from source,

```
docker build -t nukkit .
```

Run once to generate the `/data` volume, default settings, and choose language,

```
docker run -it --rm -p 19132:19132 nukkit
```

Use [docker-compose](https://docs.docker.com/compose/overview/) to start server on port `19132` and with `./data` volume,

```
docker-compose up -d
```

Contributing
------------
Please read the [CONTRIBUTING](.github/CONTRIBUTING.md) guide before submitting any issue. Issues with insufficient information or in the wrong format will be closed and will not be reviewed.
