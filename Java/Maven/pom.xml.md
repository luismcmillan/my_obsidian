


mvn archetype:generate -DgroupId=com.ibm.Reporting_app -DartifactId=Reporting_app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false


```
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"

xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">

	<modelVersion>4.0.0</modelVersion>
	<groupId>com.ibm.Reporting_app</groupId>
	<artifactId>Reporting_app</artifactId>
	<packaging>jar</packaging>
	<version>1.0-SNAPSHOT</version>
	<name>Reporting_app</name>
	<url>http://maven.apache.org</url>

	
	
	
	#NEED TO BE ADDED
	<dependencies>
		<dependency>
			<groupId>org.postgresql</groupId>
			<artifactId>postgresql</artifactId>
			<version>42.2.14</version>
		</dependency>
		
		<dependency>
			<groupId>org.json</groupId>
			<artifactId>json</artifactId>
			<version>20210307</version>
		</dependency>
	</dependencies>
	
	<build>
		<plugins>
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-jar-plugin</artifactId>
				<configuration>
					<archive>
					<manifest>
						<addClasspath>true</addClasspath>
						<mainClass>com.ibm.Reporting_app.App</mainClass>
					</manifest>
					</archive>
				</configuration>
			</plugin>
		</plugins>
	</build>
</project>
```



