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
