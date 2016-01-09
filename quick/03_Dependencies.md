# Updates to Add Dependency

### Application.java

**Imports:**

	import org.apache.commons.lang3.StringUtils;

**New Method:**

	public int countWords(String words) {
        String[] separateWords = StringUtils.split(words, ' ');
        return (separateWords == null) ? 0 : separateWords.length;
    }

**Add to Main:**

	int count = app.countWords("I have four words");
    System.out.println ("Word Count: " + count);

### pom.xml

**General:**

Bump version to 1.2

**Dependencies:**

	<dependencies>
		<dependency>
			<groupId>org.apache.commons</groupId>
			<artifactId>commons-lang3</artifactId>
			<version>3.3.2</version>
		</dependency>
	</dependencies>

### Run

	mvn package
	cd target
	java -cp simple-example-1.2.jar training.maven.quick.Application

### Dependecy Tree

	mvn dependency:tree