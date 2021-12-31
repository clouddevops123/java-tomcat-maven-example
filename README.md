# java-tomcat-maven-example
Prerequisites:

Edit tomcat-users.xml in tomcat ::

	<role rolename="tomcat"/>
	<role rolename="admin-script"/>
	<role rolename="manager-script"/>
	<role rolename="manager-gui"/>
	<role rolename="manager-jmx"/>
	<role rolename="manager-status"/>
	<role rolename="manager"/>
	<role rolename="admin"/>
	<user password="password" roles="tomcat" username="admin"/>
	<user password="password" roles="manager-gui" username="admin"/>
	<user password="password" roles="admin,admin-script,manager-gui,manager-script,manager-jmx,manager-status" username="admin"/>
	
	::

---------------------------------

'Automation:'
Deploying Project War files to Tomcat using Maven

mvn install tomcat7:deploy

--------------------------------

"Automation:"
Deploying Project snapshots to nexus using Maven

mvn clean deploy
