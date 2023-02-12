# Installation
## Building Apache Flink from Source

Prerequisites for building Flink:

* Unix-like environment (we use Linux, Mac OS X, Cygwin, WSL)
* Git
* Maven (we recommend version 3.2.5 and require at least 3.1.1)
* Java 11
* For Flink, we branched out from Flink 1.15.2-rc2 as it is the latest that Stateful Fun can support

```shell
# use the maven wrapper provided by Flink
./mvnw clean package -DskipTests -Dcheckstyle.skip -Drat.skip=true -Dos.arch=x86_64 # this will take up to 15 minutes
```
Flink is now installed in `build-target`.
