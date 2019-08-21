
# Docker Android Development Environment

<img src="https://miro.medium.com/max/1400/1*2xppr65aGJTVJGf-PJJlxQ.png"/>

## Official image on dockerhub can be found here [adamino/android](https://hub.docker.com/r/adamino/android)  
![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/adamino/android)
[![](https://images.microbadger.com/badges/version/adamino/android.svg)](https://microbadger.com/images/adamino/android)
[![](https://images.microbadger.com/badges/image/adamino/android.svg)](https://microbadger.com/images/adamino/android "Get your own image badge on microbadger.com")

## This project serves a Android ready development environment, based on openjdk 8 with Android SDK 8 installed and set in path!

## Requirements
In order to utilize this image, you only need to have the latest version of docker installed!

## Includes
- APIs: android-28
- Android SDK 25.2.5
- Build-Tools: 25.0.2
- Gradle 4.10.3

## Tagging scheme
- ${HIGHEST_ANDROID_API_VERSION}-  
${HIGHEST_ANDROID_SDK_VERSION}-  
${BUILD_TOOLS_VERSION}-  
${GRADLE_VERSION}
- e.g. 28-25.2.5-25.0.2-4.10.3

## Usage
### Pull from Docker Hub
```
docker pull beevelop/android:latest
```  
### Build from GitHub
```
docker build -t beevelop/android github.com/adamino/docker-android
```  
### Run image
```
docker run -it adamino/android bash
```  
### Use as base image
```
FROM adamino/android:latest
```
