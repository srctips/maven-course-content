# Updates to Set Source/Target Version

### Application.java

**Imports:**

	import java.util.ArrayList;
	import java.util.List;

**New Method:**

	public void greet() {
        List<String> greetings = new ArrayList<>();
        greetings.add("Hello");

        for (String greeting : greetings) {
            System.out.println ("Greeting: " + greeting);
        }
    }

**Add to Main:**

	app.greet();
	
### pom.xml

**General:**

Bump version to 1.1

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
	java -cp target/simple-example-1.1.jar training.maven.quick.Application