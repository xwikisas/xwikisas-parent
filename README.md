Provide various parent pom.xml for XWikiSAS extensions.

Extensions are automatically release on http://nexus.xwikisas.com if your user have the release right.

# Example

For extensions having xwiki-platform dependencies:

```xml
  <parent>
    <groupId>com.xwiki.parent</groupId>
    <artifactId>xwikisas-parent-platform</artifactId>
    <version>7.4.4</version>
  </parent>
```

For extensions having xwiki-rendering and xwiki-commons dependencies:

```xml
  <parent>
    <groupId>com.xwiki.parent</groupId>
    <artifactId>xwikisas-parent-rendering</artifactId>
    <version>7.4.4</version>
  </parent>
```

For extensions having xwiki-commons dependencies only:

```xml
  <parent>
    <groupId>com.xwiki.parent</groupId>
    <artifactId>xwikisas-parent-commons</artifactId>
    <version>7.4.4</version>
  </parent>
```

# Release of a new parent pom

The Maven Release Plugin cannot be used for these pom.xml because one of the goal is to make sure release setup is a clean slate when you use them as parent.

* Go to the right branch
* ./release.sh
