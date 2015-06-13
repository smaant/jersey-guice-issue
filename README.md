This is a very simple app (based on one of the Jersey examples), which reproduces the issue
with jersey2-guice and Jersey >= 2.16 packed into the uber-jar (https://github.com/Squarespace/jersey2-guice/issues/30).

To run:
```bash
$ mvn clean package
$ java -jar target/jersey-guice-issue-1.0-SNAPSHOT.jar
```

To solve the issue, uncomment string in `pom.xml` in `maven-shade-plugin` configuration.
