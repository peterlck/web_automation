This SeleniumAutomation project attempts to use the Maven project layout and configuration and enable it to support Eclipse IDE

Maven Directory Layout
SeleniumAutomation
   |-src
      |---main
         |-----java
	    |-------com
	       |---------plcapital
	          |-----------App.java
		     |---test
		        |-----java
			   |-------com
			      |---------plcapital
			         |-----------AppTest.java
				    |-pom.xml



IMPORTANT!!!!!
Since Indigo, the Maven Eclipse plugin formerly known as m2eclipse became part of Eclipse release (at least in the pure Java release). The name of the plugin also changed from m2eclipse to m2e.
If you have a Maven based Eclipse project that you generated using mvn eclipse:eclipse, youÎéÎ÷ll notice you wonÎéÎ÷t be able to use M2Eclipse (m2e) with it. If you look at the Eclipse .project file, youÎéÎ÷ll see this comment.
NO_M2ECLIPSE_SUPPORT: Project files created with the maven-eclipse-plugin are not supported in M2Eclipse.
- See more at: http://blog.teamextension.com/m2eclipse-m2e-support-for-maven-eclipse-plugin-projects-497


Git Repo
https://github.com/plcapital/web_automation

Install TestNG plugin for Eclipse
http://beust.com/eclipse

Install Maven plugin for Eclipse (m2ee)
http://download.eclipse.org/technology/m2e/releases

Create Maven project witht the following command
mvn archetype:generate -DgroupId=com.plcapital -DartifactId=SeleniumAutomation -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false



#Should not do following if you are using Eclipse after Indigo
Works with Eclipse IDE
mvn eclipse:eclipse
Add classpath variables to project classpath
Name: M2_REPO
Path: C:/Users/your_username/.m2/repository

