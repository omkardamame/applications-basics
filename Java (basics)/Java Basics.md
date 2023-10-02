## Java Version

```bash
java -version
```


## Set path for Java

```bash
export PATH=$PATH:/opt/jdk-20/bin
```

## Java Virtual Machine (JVM)

Java runs its class file in a virtual machine. The class file is in intermediary byte code. This JVM is destroyed after successful execution of the code.

![[java_jvm.png]]


## Packaging in Java: 

Sometimes, we need to run multiple class files and they might be dependent on each other and on dependencies. In this case a Java Archive (JAR) file is created. A Web Archive (WAR) file is created when it consist of images and other files.

This command is run when jar file is needed,

```bash
jar cf MyApp.jar test1.class test2.class ...
```

When this file is created, it generates a manifest file within the package at path at `META-INF/MANIFEST.MF`. This files consist of information of files present in jar file and any other metadata regarding the application. There is a main class file which needs to run before all the class files which is specified in `Main-Class` field in the manifest file.

To run the jar file you should use following command format,

```bash
java -jar MyApp.jar
```

![[java_package.png]]

## Document

Documentation should be created so that other devs can easily browser and through and read.

You can use javadoc utility by running the Java doc command and specifying the source code as input.

```bash
javadoc -d doc MyClass.java
```

```bash
cd /opt/app/; javadoc -d doc MyClass.java
```

![[java_doc.png]]

## Build Process

This is the basic build process of building a java file. This can be much more complex depending upon application and project. This is just a simplified version.

![[java_build_process.png]]

This process can be done with ease using build tools such as,

1. Maven
2. Gradle
3. ANT

These tools use configuration files where you can specify the steps that you want to automate such as the steps in your build process and these tools can automatically execute that steps in that particular order that you have defined.

This is a simple example for ANT tool's build file which uses XML.

![[java_ant.png]]

To install Apache ANT tool, use following command (CentOS/ RHEL),

```bash
sudo yum install -y ant
```

To install MAVEN tool, use following command (CentOS/ RHEL),

```bash
sudo yum install -y maven
```

curl -sL https://rpm.nodesource.com/setup_14.x | sudo bash -;sudo yum install -y nodejs