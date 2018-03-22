mvn --version
  - reports Maven version
  - reports JAVA HOME
  - reports Maven Home

src/main/java folder - holds all application source code
src/test/java folder - holds all test cases (JUnits)

During compile phase, maven-compiler-plugin compile goal will compile all Java sources kept under src/main/java

During testCompile phase, maven-compiler-plugin testCompile goal will compile all JUnits kept under src/test/java 

During test phase, maven-surefire-plugin test goal will execute all Unit test cases

To compile the project
mvn compile

To delete target folder with all binaries
mvn clean

To perform rebuild
mvn clean compile

To perform test
mvn clean test 

To list maven life cycle phases
mvn help:describe -Dcmd=compile 

To list plugin goals
mvn help:describe -Dcmd=plugin=org.apache.maven.plugins:maven-compiler-plugin:3.7.0

To list plugin goals with parameter details
mvn help:describe -Dcmd=plugin=org.apache.maven.plugins:maven-compiler-plugin:3.7.0 -Ddetail

To generate effective pom
mvn help:effective-pom

To generate effective settings
mvn help:effective-settings



