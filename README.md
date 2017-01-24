# maven-common-web-config-example

There are times where you need to build two or more WAR files with very minor variances and there are several options to achieve this:

* copy and paste 
* using maven-aeembly plugin
* multi-module project

This example showcases the multi-module project technique. Each module has a pom.xml which is responsible for building a unit of work that can be shared across another module(s).

Maven Project Structure

maven-common-web-config-example/

parent and root of the multi-module project, does not do anything significant other than dependency inheritance, properties inheritance etc

## Building

### SIT

```
mvn clean install -DskipTests=true
```
