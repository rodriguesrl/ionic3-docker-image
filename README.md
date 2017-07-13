# Ionic 3 Docker Image

Pulling image from Docker Hub:
```sh
$ docker pull rodriguesrl/ionic3
```

Creating Container for quick ionic tests:
```sh
$ docker run -it --privileged -v /dev/bus/usb:/dev/bus/usb -p 8100:8100 -p 35729:35729 -p 53703:53703 --name quickTest -P rodriguesrl/ionic3
```

For a detailed explanation of the `$ docker run` command, please check this [Gist](https://gist.github.com/rodriguesrl/c30dbaeb05d72c9980872080e48a47fb).

This container will start on `/tmp` directory and already haves the Android SDK and support to ADB deploy.

To start an ionic project check this [Tutorial](http://ionicframework.com/docs/intro/tutorial/).
