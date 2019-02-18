# Debian packages for AdoptOpenJDK

This repository contains scripts used by the Scottish Government Digital
Publishing team to package AdoptOpenJDK builds as Debian packages.

## Usage

To build a Debian package, run the `adoptopenjdk` script as follows:

    ./adoptopenjdk <product> <implementation>

The `product` should be one of:

* openjdk8
* openjdk11

The `implementation` should be one of:

* hotspot
* openj9

The WORK_DIR environment variable can be used to specify a working directory
into which JDKs are downloaded and unpacked.

Example:

    WORK_DIR=/tmp ./adoptopenjdk openjdk8 hotspot
