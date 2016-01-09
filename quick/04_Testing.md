# Updates to Add Unit Testing

### Test Class

See **ApplicationTest.java**

### pom.xml

**General:**

Bump version to 1.3

**Dependencies:**

	<dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.12</version>
        <scope>test</scope>
    </dependency>

### Run

	mvn test
	# with rest of pipeline
	mvn package