# bw-cliutil [![Build Status](https://travis-ci.org/Bedework/bw-util.svg)](https://travis-ci.org/Bedework/bw-util)
This project provides a number of utility classes and methods used for clis

## Requirements

1. JDK 17
2. Maven 3

## Building Locally

> mvn clean install

## Releasing

Releases of this fork are published to Maven Central via Sonatype.

To create a release, you must have:

1. Permissions to publish to the `org.bedework` groupId.
2. `gpg` installed with a published key (release artifacts are signed).

To perform a new release:

> mvn -P bedework-dev release:clean release:prepare

When prompted, select the desired version; accept the defaults for scm tag and next development version.
When the build completes, and the changes are committed and pushed successfully, execute:

> mvn -P bedework-dev release:perform

For full details, see [Sonatype's documentation for using Maven to publish releases](http://central.sonatype.org/pages/apache-maven.html).

## Release Notes
### 4.1.0
* Initial release after extracting from bw-util

### 5.0.0
* Update library versions 
* Add commands to set and get tz attributes
* Pass class loader as parameter when creating new objects. JMX interactions were failing
* Use bedework-parent for builds.

### 5.0.1
* Update library versions 
* Message changes

### 5.0.2
* Update library versions 
* Pre-jakarta


