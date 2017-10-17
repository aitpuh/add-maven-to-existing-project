1. Right-click project root > add framework support > Check Maven
2. Click enable auto-import on the lower right corner 
3. Edit pom.xml > add artifact id (org.sample.etc)  
4. Add the following to your pom.xml 

```xml
<properties>
		<java.version>1.8</java.version>
</properties>
<build>
    <resources>
        <resource>
            <directory>${project.basedir}/src/main/java</directory>
            <excludes>
                <exclude>**/*.java</exclude>
            </excludes>
        </resource>
        <resource>
            <directory>${project.basedir}/src/main/resources</directory>
            <includes>
                <include>*</include>
            </includes>
        </resource>
    </resources>
</build>
<dependencies>
</dependencies>
```


5. go to https://mvnrepository.com/ to search for dependencies to add to your pom.xml file! 
