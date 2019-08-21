
# Docker Android Development Environment

<img src="https://miro.medium.com/max/1400/1*2xppr65aGJTVJGf-PJJlxQ.png"/>

## Official image on dockerhub can be found here [adamino/android](https://hub.docker.com/r/adamino/android)  
![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/adamino/android)
[![](https://images.microbadger.com/badges/version/adamino/android.svg)](https://microbadger.com/images/adamino/android)
[![](https://images.microbadger.com/badges/image/adamino/android.svg)](https://microbadger.com/images/adamino/android "Get your own image badge on microbadger.com")

## This project serves a Android ready development environment, based on openjdk 8 with Android SDK 8 installed and set in path!

## Requirements
In order to utilize this image, you only need to have the latest version of docker installed!

## Usage

1. Download the docker-compose file to the root of your Ionic project.
2. Add the following line to your package.json scripts array:  
``` 
"scripts": {
    "ionic-serve": "ng run app:ionic-cordova-serve --host=0.0.0.0 --port=8100 --cordova-mock", 
}
```
3. Run the following command

```
docker compose-up
```

This way you will see the output of the container.
The app will be served at 
[localhost:8100 ](http://localhost:8100)

If you want to run the container without seeing the output simply run:
```
docker-compose up -d
```

If you want to attach a shell execute the the following command:
```
docker exec -it {NameOfYouContainer} /bin/sh
```
E.g. 
``` 
docker exec -it myAwesomeApp_ionic_1 /bin/sh 
```
