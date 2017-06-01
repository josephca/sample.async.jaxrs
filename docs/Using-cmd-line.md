## Building and running the sample using the command line

### Clone Git Repo
:pushpin: [Switch to Eclipse example](/docs/Using-WDT.md/#clone-git-repo)

```bash

$ git clone https://github.com/WASdev/sample.async.jaxrs.git

```

### Building the sample
:pushpin: [Switch to Eclipse example](/docs/Using-WDT.md/#building-the-sample-in-eclipse)

This sample can be built using [Maven](#apache-maven-commands).

###### [Apache Maven](http://maven.apache.org/) commands

```bash
$ mvn install
```

If you want to also run the functional tests then you need to [Download WAS Liberty](/docs/Downloading-WAS-Liberty.md) and pass in the location of your install as the system property libertyRoot:

```bash
$ mvn -DlibertyRoot=<LibertyInstallLocation> install
```

### Running the application locally
:pushpin: [Switch to Eclipse example](/docs/Using-WDT.md/#running-the-application-locally)

Pre-requisite: [Download WAS Liberty](/docs/Downloading-WAS-Liberty.md)

Use the following to start the server and run the application:

```bash
$ mvn liberty:run-server or,
$ mvn liberty:start-server
```

* `run-server` runs the server in the foreground.
* `start-server` runs the server in the background. 
