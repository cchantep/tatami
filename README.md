# Tatami

Scala/Java artifact repository

## Maven 2/3

Following code can be merged into your `HOME/.m2/settings.xml` to be able to use this repository:

```xml
<settings>
  <profiles>
    <profile>
      <!-- ... -->
      <repositories>
        <repository>
          <id>tatami-releases</id>
          <name>Tatami Maven2 Repository (releases)</name>
          <url>https://raw.github.com/cchantep/tatami/master/releases</url>
          <releases>
            <enabled>true</enabled>
          </releases>
          <snapshots>
            <enabled>true</enabled>
          </snapshots>
        </repository>
      </repositories>
    </profile>
  </profiles>
</settings>
```

Url can be changed to https://raw.github.com/cchantep/tatami/snapshots to use snapshots artifacts.

## SBT

Add this repo to your SBT config:

```scala
resolvers ++= Seq(
  "Tatami Releases" at "https://raw.github.com/cchantep/tatami/master/releases",
  "Tatami Snapshots" at "https://raw.github.com/cchantep/tatami/master/snapshots")

```
