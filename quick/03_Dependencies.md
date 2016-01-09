# Updates to Add Dependency

### Application.java

**Imports:**

	import org.apache.commons.lang3.StringUtils;

**New Method:**

	public int countWords(String words) {
        String[] separateWords = StringUtils.split(words, ' ');
        return (separateWords == null) ? 0 : separateWords.length;
    }

### pom.xml

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
	java -cp target/simple-example.jar training.maven.quick.Application

### Dependecy Tree

	mvn dependency:tree