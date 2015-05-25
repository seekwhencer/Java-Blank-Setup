#Build:
Call in folder with pom file to..

* build: **mvn package** 
* to clean: **mvn clean**
* first clean then build: **mvn clean package**

See target folder for built files.

[Introduction maven lifecycle](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html)

So "package" will implicitly call: validate, compile, test, package.

#Maven folder structure

    Java-Blank-Setup
    |- src
    	|- main // all code
    		|- java
    		|- resources
    	|- test // all test code
    	    |- java
    		|- resources
    |- target //contains compiled stuff " mvn clean" deletes this
    |- pom.xml //maven project file


#Eclipse:

File->Import...->Maven/Existing Maven projects, chose **folder** with pom. The workspace folder could/should be a different folder:


    stuff  
    |--workspace  
    |--Java-Blank-Setup  
        | --pom  
	    | ...  
