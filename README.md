# business-card-ocr

## Motivation
This application is a solution to an [Asymmetrik programming challenge](http://asymmetrik.com/programming-challenges/) 

## About 
The business-card-ocr tool takes a .txt file with information about a person and parses that file for a name, phone number, and email address

## Requirements
This application requires Java to run, and uses Gradle as a build tool.

## Application Inputs
This program takes a single txt file as input via the command line. The file should contain info normally found on a business card, seperated by new lines. 

Example: 
``` 
Bob Evans
Software Engineer
1685 Scotland Drive, Baltimore, MD 11111
Phone: (717) 762-8401
bevans@gmail.site
```

## Installation
To create the Jar run
```console
foo@business-card-ocr
> ./gradlew shadowJar
```
A jar will be created in build/libs

Note: if you get the error
```console
Error: Could not find or load main class org.gradle.wrapper.GradleWrapperMain
```
then try running the following command before running shadowJar 
```console
gradle wrapper 
```


## Running the Application
After creating the jar, to run the application simply navigate to build/libs and run
```console
foo@business-card-ocr/build/libs
> java -jar BusinessCardParser-all.jar path/to/BusinessCardfile.txt
```

## Testing
In the root directory of the project run
```console
foo@business-card-ocr
> ./gradlew test
```
## Licence
[MIT License](https://github.com/NeradaXsinZ/business-card-ocr/blob/master/LICENSE)