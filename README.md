# karaf-assembly-test
Test Karaf Assembly Plugin

Note: ipojo features file don't have "features" classifier, so you need to handle this manually ...

Download this file:
https://repo1.maven.org/maven2/org/apache/felix/org.apache.felix.ipojo.features/1.12.1/org.apache.felix.ipojo.features-1.12.1.xml

And copy it here:
<YOUR_LOCAL_MAVEN_REPO>/org/apache/felix/org.apache.felix.ipojo/1.12.1/org.apache.felix.ipojo-1.12.1-features.xml

So this pom.xml dependency is valid:

        <dependency>
            <groupId>org.apache.felix</groupId>
            <artifactId>org.apache.felix.ipojo</artifactId>
            <version>${version.ipojo}</version>
            <classifier>features</classifier>
            <type>xml</type>
        </dependency>

