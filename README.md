<h1 align="center"><img src="https://jmeter.apache.org/images/logo.svg" alt="Apache JMeter logo" /></h1>

Performance and load testing using Apache Jmeter.
## About Apache Jmeter
Apache JMeter can measure performance and load test static and dynamic web applications.

It can be used to simulate a heavy load on a server, group of servers,
network or object to test its strength or to analyze overall performance under different load types.

![image](https://github.com/user-attachments/assets/112632d8-4d18-40d6-baf6-001782b06921)

## Features
Complete portability and 100% Java.
Multi-threading allows concurrent sampling by many threads and
simultaneous sampling of different functions by separate thread groups.

### IDE

Fully featured Test IDE that allows fast Test Plan **recording**
 (from Browsers or native applications), **building** and **debugging**.

 ### Create Jtl file Command Line
 ```console
 jmeter -n -t b30_demo.jmx -l report\b30_demo.jtl
```
### Create Html file Command Line
```console
 jmeter -g report\b30_demo.jtl -o report\b30_demo.html
```
### Report
![image](https://github.com/user-attachments/assets/091bda18-e53a-4229-8f2c-d052b0bbe898)
![image](https://github.com/user-attachments/assets/86cb731e-a686-49dd-b7c3-695dbd33be76)

### Highly Extensible Core

- Pluggable Samplers allow unlimited testing capabilities.
- **Scriptable Samplers** (JSR223-compatible languages like Groovy).
- Several load statistics can be chosen with **pluggable tiers**.
- Data analysis and **visualization plugins** allow great extensibility and personalization.
- Functions can be used to provide dynamic input to a test or provide data manipulation.
- Easy Continuous Integration via 3rd party Open Source libraries for Maven, Gradle and Jenkins.

## Requirements

The following requirements exist for running Apache JMeter:

- Java Interpreter:

  A fully compliant Java 17 Runtime Environment is required
  for Apache JMeter to execute. A JDK with `keytool` utility is better suited
  for Recording HTTPS websites.

- Optional jars:

  Some jars are not included with JMeter.
  If required, these should be downloaded and placed in the lib directory
  - JDBC - available from the database supplier
  - JMS - available from the JMS provider
  - [Bouncy Castle](https://www.bouncycastle.org/) -
  only needed for SMIME Assertion

- Java Compiler (*OPTIONAL*):

  A Java compiler is not needed since the distribution includes a
  precompiled Java binary archive.
  > **Note** that a compiler is required to build plugins for Apache JMeter.

## Installation Instructions

> **Note** that spaces in directory names can cause problems.

- Release builds

  Unpack the binary archive into a suitable directory structure.

## Running JMeter

1. Change to the `bin` directory
2. Run the `jmeter` (Un\*x) or `jmeter.bat` (Windows) file.

### Windows

For Windows, there are also some other scripts which you can drag-and-drop
a JMX file onto:

- `jmeter-n.cmd` - runs the file as a non-GUI test
- `jmeter-n-r.cmd` - runs the file as a non-GUI remote (client-server) test
- `jmeter-t.cmd` - loads the file ready to run it as a GUI test

![image](https://github.com/user-attachments/assets/9cb16d10-9a56-4fc0-b20e-4de563bca090)
![image](https://github.com/user-attachments/assets/8b508595-4515-4ff8-b2e6-b45fb99ded03)



