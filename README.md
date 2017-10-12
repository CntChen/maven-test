# maven-test
learning java.

## start
* follow document:
> https://spring.io/guides/gs/maven/

* update maven compile configulation
error when run `mvn compile`:
```
[ERROR] COMPILATION ERROR : 
[INFO] -------------------------------------------------------------
[ERROR] Source option 1.5 is no longer supported. Use 1.6 or later.
```

how to fix this:
> https://stackoverflow.com/questions/29258141/maven-compilation-error-use-source-7-or-higher-to-enable-diamond-operator

add the following code to `pom.xml` inside `project` property:
```
    <properties>
        <maven.compiler.source>1.7</maven.compiler.source>
        <maven.compiler.target>1.7</maven.compiler.target>
    </properties>
```

## run
* package
```
$ mvn package
```
and `target` folder is genarated.

* run
```
$ java -jar /target/maven-test-0.1.0.jar
Hello world!
```

## EOF