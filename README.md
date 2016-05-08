jetbrick-eclipse-formatter
=================================

jetbrick eclipse formatter configuration for `maven-java-formatter-plugin`

```xml
<plugin>
    <groupId>com.googlecode.maven-java-formatter-plugin</groupId>
    <artifactId>maven-java-formatter-plugin</artifactId>
    <version>0.4</version>
    <configuration>
        <configFile>jetbrick-eclipse-formatter.xml</configFile>
        <overrideConfigCompilerVersion>true</overrideConfigCompilerVersion>
        <lineEnding>LF</lineEnding>
    </configuration>
    <dependencies>
        <dependency>
            <groupId>com.github.subchen</groupId>
            <artifactId>jetbrick-eclipse-formatter</artifactId>
            <version>1.0</version>
         </dependency>
    </dependencies>
    <executions>
        <execution>
            <phase>process-sources</phase>
            <goals>
                <goal>format</goal>
            </goals>
        </execution>
    </executions>
</plugin>
```

Execute using maven

```bash
mvn process-sources
```