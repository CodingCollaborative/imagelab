# ImageLab

ImageLab is a framework that allows students to develop
image modification processors (filters) and to experience
the results visually and aurally.

## Contents
The __imagelab__ and __sound__ packages may be provided in an `imagelab.jar` file.
The `imagelab.jar` file also includes the class __Run__ with a `public static void main` method in the unnamed package, used to facilitate running the ImageLab application.
(This version may also be used directly as a [BlueJ](http://bluej.org) project.)

The __filter__ package is generally provided as a folder with source (`.java`) and compiled (`.class`) files, with the source versions serving as examples for students.

A sample set of images are provided in an __"images"__ directory.

## To use from command line:  
* Make sure the __filters__ directory is _in the same directory_ as the __imagelab.jar__ file.
* Then issue the command  
`java -jar imagelab.jar`  
  
An alternative command is:
`java -cp ".:imagelab.jar" Run`  
Note that on Windows platforms, the ":" character in the classpath must be changed to the ";" character.

## Build Instructions 

### Introduction

This document's intent is to support developers in understanding how to 
build the ImageLab project. This document offers support on key useful commands and error solutions that can make building Image Lab a smoother process.

### Before You Build
- Install Gradle
 sudo apt install gradle
- Install Canberra
 Sudo apt install libcanberra-gtk-module libcanberra-gtk3-module


### What is Gradle

Gradle is a automated build system that makes working with large projects easier.
It streamlines the build process by skipping re-execution and allows developers to preform tasks using one line of code in the command line.



### How does Gradle Work?

▪️Project 
- A project is a depiction of what needs to be built and how we get an artifact at the end of a build.

settings.gradle - Where projects are registered.
build.gradle - constructs commands that can be used to execute tasks.


▪️Task
-A task is used to execute an action during the build process. For example,
    ./gradlew compileJava
 will compile the main class in the build. 



◾️Possible Errors and Solutions During Build
Error
-Failed to load module "canberra-gtk-module"
Solution
-Sudo apt install libcanberra-gtk-module libcanberra-gtk3-module


◾️Key Commands
./gradlew tasks --all | Displays the full list of commands that can be excecuted
./gradlew run | Runs the program
./gradlew compileJava | Compiles the main java source
./gradlew clean | Deletes the build Directory
./gradlew classes | Assembles the main classes
./gradlew build | Assembles and tests the project.
./gradlew testClasses | Assembles the test classes
./gradlew checkstyle | generates checkstyle reports
./gradlew test | Runs the unit tests.
./gradlew compileTestJava | Compiles the Unit Tests
./gradlew check | Runs all checks


### Resources and References

https://gradle.org/guides/


## License

ImageLab is a framework for student exploration of image processing.  
Copyright (C) 2016,2019 by Aaron Gordon & Jody Paul  
The software comes with ABSOLUTELY NO WARRANTY.
 
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see https://www.gnu.org/licenses/

___

Project Website: https://metrocs.github.io/imagelab/

