---
title: Install Sinch SMS Java Library 
excerpt: >-
The Sinch SMS Java SDK help you interact with the SMS API from your Java Application. This guide helps you set up SMS SDK in your application.
hidden: true
---
## Installing with Maven/Gradle

Using Maven/Gradle is the recommended way to install the SDK. You can add this sdk to your existing project.

In **Maven**, please put the lines below in your **pom.xml**

```javascript
<dependency>
  <dependency>
      <groupId>com.sinch</groupId>
      <artifactId>sdk-sms</artifactId>
      <version>1.0.3</version>
  </dependency>
```

In **Gradle**, please put the lines below in your **build.gradle**

```javascript
implementation 'com.sinch:sdk-sms:1.0.3'
```

Because Sinch SDK Library is hosted on Maven Central Repository, please make sure you have **mavenCentral()** in your **build.gradle**.

```javascript
repositories {
    mavenCentral()
}
```

## Installing the SDK locally

It is possible to download and use the Java SDK manually by [downloading a pre-built jar file](https://repo1.maven.org/maven2/com/sinch/sdk-sms/1.0.3/). 

Please have [Maven](http://maven.apache.org/download.html) install in your environment in advance.

[Clone the source code](https://github.com/sinch/sinch-java-sms), and install the library. 

```javascript
git clone https://github.com/sinch/sinch-java-sms.git
cd sinch-java-sms    
mvn clean install
```

If you encounter "Permission Denied", please run 

    $ sudo mvn clean install

If you need to skip local tests

    $ mvn package -Dmaven.test.skip=true

The jar file is under **target** folder 

There are two available jar

```javascript
sdk-sms-1.0.3-SNAPSHOT-jar-with-dependencies.jar 
sdk-sms-1.0.3-SNAPSHOT.jar -- Use this if you need to include version dependencies on your own.
```

## Importing jar with Intellij

Follow this step

```
File -> Project Structure -> Modules -> Plus Sign -> Browse the SDK SMS Jar.
```

## Importing jar with Eclipse

Follow this step

```
Project -> Build Path -> Configure Build Path -> Libraries -> Add Jar.
```