# Opal

![Opal](https://codedead.com/Software/Opal/opal.png)

![GitHub release (latest by date)](https://img.shields.io/github/v/release/CodeDead/opal)
![GitHub](https://img.shields.io/badge/language-Java-green)
![GitHub](https://img.shields.io/github/license/CodeDead/opal)

Opal is a free and open-source JavaFX application that can play relaxing music in the background.

## Building

### Windows

#### Installer

You can create an executable installer by running the `jpackage` Gradle task:
```shell
./gradlew jpackage
```
*Do note that you will need the [WiX Toolset](https://wixtoolset.org/) in order to create MSI packages.*

#### Portable image

You can create a portable image by running the `jpackageImage` Gradle task:
```shell
./gradlew jpackageImage
```

### Linux

#### rpm

You can create an RPM, by running the `jpackage` Gradle task:
```shell
./gradlew jpackage
```
*Do note that you will need the `rpm-build` package in order to create an RPM.*

#### AppImage

You can create an [AppImage](https://appimage.github.io/) by executing the `AppImage` Gradle task:
```shell
./gradlew AppImage
```
*Do note that running this task will execute a shell script in order to download and run the [appimagetool](https://appimage.github.io/appimagetool/) in order to create the AppImage file.*

#### Portable image

You can create a portable image by running the `jpackageImage` Gradle task:
```shell
./gradlew jpackageImage
```

## Dependencies

A couple of dependencies are required in order to build Opal:

* [JDK16](https://openjdk.java.net/projects/jdk/16/)
* [JavaFX](https://openjfx.io/)
* [Gradle](https://gradle.org)
* [FasterXML/jackson](https://github.com/FasterXML/jackson)
* [badass-jlink-plugin](https://github.com/beryx/badass-jlink-plugin)
* [Log4j2](https://logging.apache.org/log4j/2.x/)

### Windows

#### MSI
In order to build an installer (*MSI*) of Opal on Windows, you will need:

* [WiX Toolset](https://wixtoolset.org/)

### Linux

#### rpm

In order to create an [RPM](https://en.wikipedia.org/wiki/RPM_Package_Manager), you will need to have the following package(s) installed:

* rpm-build (`dnf install rpm-build`)

## About

This library is maintained by CodeDead. You can find more about us using the following links:
* [Website](https://codedead.com)
* [Twitter](https://twitter.com/C0DEDEAD)
* [Facebook](https://facebook.com/deadlinecodedead)
* [Reddit](https://reddit.com/r/CodeDead/)

The audio that was included with this project was provided by [ZapSplat](https://www.zapsplat.com/).

Copyright © 2021 CodeDead
