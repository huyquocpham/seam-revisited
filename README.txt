THIS IS NOW LEGACY PROTOTYPE OF SEAM 2.3 - CURRENT DEVELOPMENT IS IN OLD SVN JBOSS SEAM REPOSITORY
http://anonsvn.jboss.org/repos/seam/branches/community/Seam_2_3

****************************************************

JBoss Seam Framework - 2.3.x

This is a prototype of maven migration of http://anonsvn.jboss.org/repos/seam/branches/community/Seam_2_2

Project Directory Structure
-------------------

jboss-seam-parent - Parent module for declaring common parts for all/almost modules
 -	distribution - module for creating one distribution bundle - not working
 -	examples - migrated all examples to maven build style
 -	functional-tests - selenium automatic tests for existing examples
 -	jboss-embedded-bootstrap - configuration for jboss embedded runtime (mainly for integration tests)
 -	jboss-seam - core module of the Seam
 -	jboss-seam-debug - UI debug module
 -	jboss-seam-excel - excel integration module
 -	jboss-seam-flex - flex integration module
 -	jboss-seam-gen - Old Seam Gen tool
 -	jboss-seam-ioc - IOC integration module - inversion of control, integration with Spring, Guice
 -	jboss-seam-jul - JUL module - Java Util Logging abstraction
 -	jboss-seam-mail - Mail integration module
 -	jboss-seam-pdf - PDF integration module
 -	jboss-seam-remoting - Remoting module
 -	jboss-seam-resteasy - Resteasy integration module
 -	jboss-seam-rss - RSS integration module
 -	jboss-seam-ui - Seam UI module
 -	jboss-seam-wicket - Wicket integration module
 -	seam-integration-tests - Seam integration tests (jboss embedded as runtime)
 -	seam-reference-guide - Reference Guide sources

Dependencies
------------
The pom.xml in the jboss-seam-parent of the source checkout contains the Maven configuration which 
controls dependency versions. Individual dependencies used only in a module is used in an module pom file.

Building
-------------------
Run 
	mvn clean install

Required maven version is 3.0.0 and greater


