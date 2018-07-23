## SWRLAPI Example

This project provides a simple example of a Java application that uses the [SWRLAPI](https://github.com/protegeproject/swrlapi/wiki)
to create and execute SWRL rules and SQWRL queries. 

You can import this project into your favourite IDE using its Maven-based project creation facility.

### Building and Running

To build and run this project you must have the following items installed:

+ [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
+ A tool for checking out a [Git](http://git-scm.com/) repository
+ Apache's [Maven](http://maven.apache.org/index.html)

Get a copy of the latest code:

    git clone https://github.com/protegeproject/swrlapi-example.git 

Change into the swrlapi-example directory:

    cd swrlapi-example

Build it with Maven:

    mvn clean install

On build completion, your local Maven repository will contain generated ```swrlapi-example-${version}.jar```
and ```swrlapi-example-${version}-jar-with-dependencies.jar``` files.
The ```./target``` directory will also contain these JARs.

You can then run the application as follows:

    mvn exec:java

#### Questions

If you have questions about this library, please go to the main
Protégé website and subscribe to the [Protégé Developer Support
mailing list](http://protege.stanford.edu/support.php#mailingListSupport).
After subscribing, send messages to protege-dev at lists.stanford.edu.
