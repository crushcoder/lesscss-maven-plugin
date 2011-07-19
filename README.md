#LessCSS Maven Plugin

This plugin compiles [LessCSS](http://lesscss.org/) to CSS at build time. By default it searches for Less files under ```/src/main/less```, but this is customizable. It is configured as follows:

    <build>
    ...
      <plugins>
        <plugin>
          <artifactId>lesscss-maven-plugin</artifactId>
          <groupId>eu.numberfour.maven.plugins</groupId>
          <executions>
            <execution>
              <goals>
                <goal>compile</goal>
              </goals>
              <phase>compile</phase>
            </execution>
          </executions>
          <configuration>
            <outputDir>${basedir}/target/classes</outputDir>
          </configuration>    
      </plugin>
    ...
    </build>
