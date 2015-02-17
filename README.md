# executable-java-container

Simple binary executable **container for java applications**. Allows you to run your java code as a service or a console program
in **windows, linux, mac, etc**.


### Disclaimer
This project is a mavenized bundle of a simple configuration of the great and powerful Tanuki's wrapper (community edition).
http://wrapper.tanukisoftware.com/doc/english/download.jsp
For commercial/professional license or advanced configurations options check the documentation at Tanuki's site.

## Introduction
One of the problems I face with Java applications is the inability to run them as standalone applications.
While the Java VM does a great job at abstracting the execution model, in order to run your apps as services,
or simple console commands you need to fill the gap between the VM executable and the platform details.  

That's where Tanuki's wrapper comes in and works as a JVM wrapper that can be executed as a native application with your code.
It still needs the JVM to run, but it abstracts you from the details of finding, executing, and restarting it.

This project builds **on top of tanuki's wrapper** to simplify its configuration and convert it to maven, so
you can use it as a dependency to build **your own portable application** that can be executed in *windows,
linux, mac, etc* without any extra code.

## Usage
There are two options to use this project: as an app container (similar to tomcat without the web part), or as a maven dependency
that wraps your code into an executable package.

### Standalone container
Very much like tomcat, to use it as a container you need to:  

1. download the latest release zip
2. unzip it in your computer
3. replace the example app with yours
4. run the script file according to your platform (i.e. linux bin/wrapper.sh)

[Check the tutorial for more details](https://github.com/kfgodel/executable-java-container/wiki/Using-executable-java-container-as-a-standalone-container)
  
  
### Maven dependency
When using it as a dependency instead of building a war, or jar, we will build a zip file that contains everything need to run your code in different platforms.
In order to do that you need to configure your project pom to include the dependency, but also to modify how the final artifact is done.  
Without going into much detail the steps needed are:  

1. Include this project as a dependency
2. Ensure that your project generates an executable uber-jar
3. Replace the example app that comes in this container with your jar
4. Pack everything in a zip file that containes this container with your app
5. Distribute as neede ;-)

There's a tutorial on the wiki page that guides you through the process for these steps.  
And you can also [check an example project here](https://github.com/kfgodel/executable-java)
[Check the tutorial for more details](https://github.com/kfgodel/executable-java-container/wiki/Using-executable-java-container-as-a-maven-dependency)


## Contact
You can contact me for any problems or suggestion in the setup at dario.garcia at 10pines.com  
(but please make the effort of figuring it out first) 

