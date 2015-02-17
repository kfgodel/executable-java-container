# executable-java-container

Simple binary executable container for java applications. Allowing to run them as standard applications or services
in many platforms.

### Disclaimer
This project is a mavenized bundle of a simple configuration of the great and powerful Tanuki's wrapper (community edition).
http://wrapper.tanukisoftware.com/doc/english/download.jsp
For commercial/professional license or advanced configurations options check the documentation at Tanuki's site.

## Introduction
One of the problems I face with Java applications is the inability to run them as standalone applications.
While the Java VM does a great job at abstracting the execution model, in order to run your apps as services,
or simple console commands you need to fill the gap between the VM executable and the platform details.  

That's where Tanuki's wrapper comes in and works as a JVM wrapper that can be executed as a native application with your code.
It still needs the JVM to run, but it abstracts you from the details of figuring that out.

This project builds **on top of tanuki's wrapper** to simplify its configuration and convert it to maven, so
you can use it as a dependency to build **your own portable application** that can be executed in **windows,
linux, mac, etc** without any extra code.

## Usage
There are two options to use this executable container: as a app container (like tomcat), or as a maven dependency
to build you own executable.

### Standalone container
Very much like tomcat, to use it as a container you need to:
1. download the latest release zip
2. unzip it in your computer
3. replace the example app with yours
4. run the script file according to your platform (i.e. linux bin/wrapper.sh)

