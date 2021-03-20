# Maven:
  ======

Build tool

	Springboot Application	=> Java
	Spark 			=> Big Data
	Python 			=> Python
	npm			=> NodeJS


Lifecycle of Maven:
=============

	Clean
	Validate
	Compile
	Test
	Package
	Verify
	Install
	Deploy


Types of repository in Maven:
====================
	>> Local Repository			=> .m2 file, downloaded  all the dependancies from central /REmote repository 
	>> Central Repository			=> in real time, we cant download anything from this repository, retrieves only from remote repository (because of security reason)
	>> Remote Repository			
	
	Can create maven project in multiple ways,
	
		>> spring initializer(start.spring.io)
		>> ide tool(ecllipse,intelliJ)
		>> command line

For creating path:
============
	export PATH=$PATH:/opt/apache-maven-3.6.3/bin

	[root@ip-172-31-34-147 bin]# echo $PATH
	/usr/local/sbin:/sbin:/bin:/usr/sbin:/usr/bin:/root/bin:/opt/apache-maven-3.6.3/bin

for installing java,
===========
	yum install java-1.8.0-openjdk -y

 	export JAVA_HOME=$(dirname $(readlink -f $(which java))|sed 's^jre/bin^^')

For checking maven version after installation:
==============================

	[root@ip-172-31-34-147 bin]# mvn --version
	Apache Maven 3.0.5 (Red Hat 3.0.5-17)
	Maven home: /usr/share/maven
	Java version: 1.8.0_265, vendor: Oracle Corporation
	Java home: /usr/lib/jvm/java-1.8.0-openjdk-1.8.0.265.b01-1.amzn2.0.1.x86_64/jre
	Default locale: en_US, platform encoding: UTF-8
	OS name: "linux", version: "4.14.203-156.332.amzn2.x86_64", arch: "amd64", family: "unix"


Ennvironment variable setup :
===================
	syetem properties-> environmental variable-> System Variable - Select Path and include Maven bin location
	
	C:\Users\ganes\Master DEVOPS\apache-maven-3.6.3-bin\apache-maven-3.6.3\bin or
	
	Create new system variable 
	
	MAVEN_HOME	C:\Users\ganes\Master DEVOPS\apache-maven-3.6.3-bin\apache-maven-3.6.3

	And include this path
	%MAVEN_HOME%\bin

Open new CMD :
===========

C:\Users\ganes\Master DEVOPS\apache-maven-3.6.3-bin\apache-maven-3.6.3\bin


Creating Maven project in spring.io:
====================================

![image](https://user-images.githubusercontent.com/54719289/111886270-c795a300-89c4-11eb-8db0-77d06cf6be92.png)


![image](https://user-images.githubusercontent.com/54719289/111886125-d6c82100-89c3-11eb-8129-94048dc00f75.png)


# To build maven project:
========================

		mvn clean install or
		mvn clean package
Note : Build gets failed if pom.xml(Project Object Model) is not present so make sure before running mvn clean command.


![image](https://user-images.githubusercontent.com/54719289/111887394-be103900-89cc-11eb-931f-8d457c4d8859.png)
![image](https://user-images.githubusercontent.com/54719289/111887744-04ff2e00-89cf-11eb-9438-3cf0434c9cc1.png)



# To fix the fatal error of java version, change it into pom.xml

Fatal error compiling: invalid target release: 11

![image](https://user-images.githubusercontent.com/54719289/111887714-cec1ae80-89ce-11eb-8b05-41aa1339e7b8.png)









