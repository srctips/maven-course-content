# Updates to Set Source/Target Version

### Application.java

**Imports:**

	import java.util.ArrayList;
	import java.util.List;

**Code:**

	List<String> greetings = new ArrayList<>();
    greetings.add("Hello");

### pom.xml

**Build:**

	<build>
		<plugins>
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-compiler-plugin</artifactId>
				<version>3.2</version>
				<configuration>
					<source>1.8</source>
					<target>1.8</target>
				</configuration>
			</plugin>
		</plugins>
	</build>

### Run

	mvn package
	java -cp target/simple-example.jar training.maven.quick.Application