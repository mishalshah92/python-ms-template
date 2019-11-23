# python-ms-template

![](https://github.com/zero-templates/python-ms-template/workflows/python-ms-template-ci/badge.svg)

This is java python-service template. This template allows to build and deploy docker image simply.
This template is very basic having integration of Django application.

Basic knowledge of the [Gradle](https://gradle.org) and [Docker](https://www.docker.com) is 
require.

## Building and Generating docker image
We uses the [Avast plugins](https://github.com/avast/gradle-docker-compose-plugin) 
that allows to configure and manager docker images.

All configurations are present into the `configs/docker.gradle`

## Build
Below command will generate the distribution zip under `build/distributions/{app_name}.zip` directory

###### Build the Application
~~~~
$ ./gradlew build
~~~~

###### Build the docker image
~~~~
$ ./gradlew composeBuild
~~~~

###### Running Docker image
~~~~
$ ./gradlew composeUp
~~~~