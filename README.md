# XWiki SAS Parent POM

Provide various parent pom.xml for XWiki SAS public extensions.

Extensions are automatically released on http://nexus.xwikisas.com if your user have the release right.

# Examples

For extensions having xwiki-platform dependencies:

```xml
  <parent>
    <groupId>com.xwiki.parent</groupId>
    <artifactId>xwikisas-parent-platform</artifactId>
    <version>16.10.9</version>
  </parent>
```

For custom XWiki distributions:

```xml
  <parent>
    <groupId>com.xwiki.parent</groupId>
    <artifactId>xwikisas-parent-platform-distribution</artifactId>
    <version>16.10.9</version>
  </parent>
```

# Versions

We follow the same versioning scheme as the [``xwiki-contrib/parent``](https://github.com/xwiki-contrib/parent?tab=readme-ov-file#versions) project.

# Release of a new parent pom

The Maven Release Plugin cannot be used for these pom.xml because one of the goal is to make sure release setup is a clean slate when you use them as parent.

* Check the [versioning scheme](#versions) above to make sure you chose the right version.
* Go to the right branch
* ./release.sh
