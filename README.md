# Empty Maven skin

Empty Maven skin renders the Maven site pages without any additional skinning or decoration.
It only outputs the contents of each page.

## Usage

To use this Maven skin, include it in your `site.xml` file:

```xml
<project>
  ...
  <skin>
    <groupId>com.example</groupId>
    <artifactId>empty-maven-skin</artifactId>
    <version>0.1.0-SNAPSHOT</version>
  </skin>
  ...
</project>
```

The skin requires Velocity >= 1.7 when generating Maven site?
Add it as a dependency to `maven-site-plugin` in your POM file:

```xml
<build>
  <plugins>
    ...
    <plugin>
      <groupId>org.apache.maven.plugins</groupId>
      <artifactId>maven-site-plugin</artifactId>
      <version>3.2</version>
      <dependencies>
        ...
        <!-- Empty skin requires Velocity >= 1.7  -->
        <dependency>
          <groupId>org.apache.velocity</groupId>
          <artifactId>velocity</artifactId>
          <version>1.7</version>
        </dependency>
        ...
      </dependencies>
      ...
    </plugin>
    ...
  </plugins>
</build>
```


## Contributing

Fork the repository and submit pull requests.


## Author

The empty maven skin is based on the blank maven skin, by:

**Andrius Velykis**

+ http://andrius.velykis.lt
+ http://github.com/andriusvelykis

## Copyright and license

Copyright 2013 Andrius Velykis

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this work except in compliance with the License.
You may obtain a copy of the License in the LICENSE file, or at:

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
