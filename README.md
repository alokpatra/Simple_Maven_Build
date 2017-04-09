# Simple_Maven_Build
Building Java Projects with Maven

Implementation of the following link
https://spring.io/guides/gs/maven/

The only modification when running via command line is you have to add the following dependecy to configure the maven compiler plugin to use a source higher than 1.3

You need to configure the maven-compiler-plugin:

<project>
  ...
  <build>
    <plugins>
      <plugin>
        <groupId>org.apache.maven.plugins</groupId>
        <artifactId>maven-compiler-plugin</artifactId>
        <version>2.3.2</version>
        <configuration>
          <source>1.5</source>
          <target>1.5</target>
        </configuration>
      </plugin>
      ...
    </plugins>
    ...
  </build>
</project>

Commands to be used post creating the Maven Project Structure as shown in the link

  mvn clean compile
  mvn package
  java -cp target/gs-maven-0.1.0.jar
  java -cp target/gs-maven-0.1.0.jar hello.HelloWorld
  git init
  git add .
  git commit -m "First Maven Build"
  git add remote origin https://github.com/alokpatra/Simple_Maven_Build.git
  git remote add origin https://github.com/alokpatra/Simple_Maven_Build.git
  git push -u origin master
  
  Project was also run sucessfully using Eclipse
  *Dependency changes doent have to be made while running with Eclipse
  
