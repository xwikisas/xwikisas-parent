Provide various parent pom.xml for XWiki SAS public extensions.

Extensions are automatically released on http://nexus.xwikisas.com if your user have the release right.

# Example

For extensions having xwiki-platform dependencies:

```xml
  <parent>
    <groupId>com.xwiki.parent</groupId>
    <artifactId>xwikisas-parent-platform</artifactId>
    <version>6.4</version>
  </parent>
```

# Release of a new parent pom

The Maven Release Plugin cannot be used for these pom.xml because one of the goal is to make sure release setup is a clean slate when you use them as parent.

* Go to the right branch
* ./release.sh
