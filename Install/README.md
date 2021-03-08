# **1. Overview**

Simply put, Maven is a command-line tool for building Java applications.

The Maven project provides a simple ZIP file containing a precompiled version of Maven for your convenience. There is no installer. It's up to you to set up your prerequisites and environment to run Maven.

The installation of Apache Maven is a simple process of extracting the archive and adding the bin folder with the *mvn* command [to the PATH](https://www.baeldung.com/linux/path-variable).



### **1.1. Prerequisites**

Maven is written in Java (and primarily used for building JVM programs). Thus, the major prerequisite is the Java JDK. You need to install the Java JDK (e.g. from [Oracle's download site](http://www.oracle.com/technetwork/java/javase/downloads/index.html)), and you should install it to a pathname without spaces.

Once Java is installed, you must ensure that the commands from the Java JDK are in your PATH environment variable. Running, for example:

```
java -version
```



# **2. Installing Maven on Windows**

To install Maven on windows, head over to [Apache Maven site](https://maven.apache.org/) to download the latest version, select the Maven zip file, for example apache-maven-3.3.9-bin.zip.

Unzip it to the folder you want Maven to live.



### **2.1. Adding Maven to the Environment Path**

Add both *M2_HOME* and *MAVEN_HOME* variables to the Windows environment using system properties, and point it to your Maven folder.

Update the PATH variable by appending the Maven bin folder – *%M2_HOME%\bin*, so that you can run the Maven’s command everywhere.

To verify it run:

```
mvn -version
```

in the command prompt. It should display the Maven version, the java version, and the operating system information. That's it, you have set up Maven on your Windows system.



# **3. Installing Maven on Linux**

To install Maven on the Linux operating system, download the latest version from the [Apache Maven site](https://maven.apache.org/), select the Maven binary tar.gz file, for example: apache-maven-3.3.9-bin.tar.gz.

Extract the archive to your desired location.



### **3.1. Adding Maven to the Environment Path**

Open the command terminal and run the following commands to set the environment variables:

```
$ export M2_HOME=/usr/local/apache-maven/apache-maven-3.3.9

$ export M2=$M2_HOME/bin

$ export MAVEN_OPTS=-Xms256m -Xmx512m
```

with *M2_Home* path corresponding with the location of your extracted Maven files.

Now append the *M2* variable to the system path:

```
$ export PATH=$M2:$PATH 
```

Finally, verify if Maven has been added by running:

```
$ mvn -version
```

The output should be as follows:

```
Apache Maven 3.3.3 (7994120775791599e205a5524ec3e0dfe41d4a06; 2016-12-03T17:27:37+05:30)
Maven home: /usr/local/apache-maven/apache-maven-3.3.9

Java version: 1.8.0_75, vendor: Oracle Corporation

Java home: /usr/local/java-current/jdk1.8.0_75/jre
```

You have successfully installed Maven on your Linux system.



# **4. Conclusion**

This quick guide illustrated how to install Maven on the major operating systems for development.

To learn how to get started with Spring with Maven – check out the tutorial [here](https://www.baeldung.com/spring-with-maven).
