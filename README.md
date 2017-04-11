# Acorn Conveyer

## Overview
Acorn Conveyer is a distributed computing system agent. It is installed in each calculating purposed servers/PCs and acts as an orchestrater among the system resources.

* Operating System Support
  * Microsoft Windows 7/Server 2003 or above with JDK 1.8 supports
  * Redhat/CentOS/Ubuntu Linux with JDK 1.8 supports  
  * MacOS with JDK 1.8 supports

## How to compile
Acorn Conveyer is able to compile on following environments:

* [JDK 1.8 or above](http://java.oracle.com)
* [Apache Maven](http://http://maven.apache.org)

If those applications are installed, run this command:

```bash
mvn package
```

Packaged JAR file is located in **target** folder with the name of **conveyer-[version].jar**.

## Overall Folder Structure

* conveyer-[version].jar
* application.properties

**To run:**
```bash
java -jar conveyer-[version].jar
```

## Application Settings

**application.properties** file is aim to config specific settings. Details are below:

* server.port=30000
  > Administration console port (Default: 30000)
* conveyer.address=localhost
  > Acorn Warehouse Server Address (Default: localhost)
* conveyer.port=9001  
  > Acorn Warehouse Server Port (Default: 9001)
* message.log.useLogstash=false
  > (Default: false)
* conveyer.inflow-cpu-limit=80.0
  > CPU limit to receive jobs from the central message queue. It presents as percent. (Default: 80.0)
* conveyer.inflow-memery-min=1000
  > Minimum required memory size to receive jobs from the central message queue. It presents as mega bytes. (Default: 1000)

## Job Flow Diagram
![Flow](https://cloud.githubusercontent.com/assets/26543063/24454726/b0b95c90-14d8-11e7-9cde-865375ffe429.png)


## Commercial Support
This solution is open-source based project. Therefore, it can be supported by communities through GitHub's issue tracker.
We also have consulting and commercial support services. If you want to discuss more, please contact at contact@acornworks.net.





  
