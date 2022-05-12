<div>

JavaScript is disabled on your browser.

</div>

::: {role="banner"}
::: fixedNav
::: topNav
[]{#navbar.top}

::: skipNav
[Skip navigation links](#skip.navbar.top "Skip navigation links")
:::

[]{#navbar.top.firstrow}

-   [Overview](../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.parser.api {#package-com.facebook.buck.parser.api .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [FileManife                       | ::: block                         |
    | st](FileManifest.html "interface  | The                               |
    | in com.facebook.buck.parser.api") | [`FileManifes                     |
    |                                   | t`](FileManifest.html "interface  |
    |                                   | in com.facebook.buck.parser.api") |
    |                                   | output as a result of parsing a   |
    |                                   | file with a                       |
    |                                   | [`FilePars                        |
    |                                   | er`](FileParser.html "interface i |
    |                                   | n com.facebook.buck.parser.api"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileParse                        | ::: block                         |
    | r](FileParser.html "interface in  | Generic file parser, meant to be  |
    | com.facebook.buck.parser.api")\<T | extended for more specific        |
    | extends                           | parsers.                          |
    | [FileManifest                     | :::                               |
    | ](FileManifest.html "interface in |                                   |
    |  com.facebook.buck.parser.api")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [PackageFileParser](P             | ::: block                         |
    | ackageFileParser.html "interface  | Parses buck package files         |
    | in com.facebook.buck.parser.api") | (usually PACKAGE files) and       |
    |                                   | retrieve rule information from    |
    |                                   | them.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectBuildFileParser](Projec   | ::: block                         |
    | tBuildFileParser.html "interface  | Parses buck build files (usually  |
    | in com.facebook.buck.parser.api") | BUCK files) and retrieve rule     |
    |                                   | information from them.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UserDefinedRuleLoader](UserD     | ::: block                         |
    | efinedRuleLoader.html "interface  | Reads a manifest file, and        |
    | in com.facebook.buck.parser.api") | ensures that it has parsed the    |
    |                                   | files required to utilize all     |
    |                                   | user defined rules in that        |
    |                                   | manifest (based on buck.type)     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuildFileManifes                 | ::: block                         |
    | t](BuildFileManifest.html "class  | Describes the content of a build  |
    | in com.facebook.buck.parser.api") | file, which includes defined      |
    |                                   | targets and their metadata.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildFileManifestPojoizer](Build | ::: block                         |
    | FileManifestPojoizer.html "class  | Utility class to convert          |
    | in com.facebook.buck.parser.api") | parser-created objects to         |
    |                                   | equivalent POJO-typed objects     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildFileManifestPojoizer.PojoT  | ::: block                         |
    | ransformer](BuildFileManifestPojo | Container to hold transformation  |
    | izer.PojoTransformer.html "class  | function for classes assignable   |
    | in com.facebook.buck.parser.api") | to a provided class.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ForwardingProjectBuildFileParse  | ::: block                         |
    | rDecorator](ForwardingProjectBuil | A convenience decorator for       |
    | dFileParserDecorator.html "class  | [`ProjectBuildFileParser`](Projec |
    | in com.facebook.buck.parser.api") | tBuildFileParser.html "interface  |
    |                                   | in com.facebook.buck.parser.api") |
    |                                   | that forwards all method          |
    |                                   | invocation to the delegate.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PackageFileManifest]             | ::: block                         |
    | (PackageFileManifest.html "class  | Describes the content of a        |
    | in com.facebook.buck.parser.api") | package file, which includes a    |
    |                                   | package definition and their      |
    |                                   | metadata.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PackageMetad                     | ::: block                         |
    | ata](PackageMetadata.html "class  | Describes the attributes of a     |
    | in com.facebook.buck.parser.api") | package rule in a package file.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                           Description
      -------------------------------------------------------------- -------------
      [Syntax](Syntax.html "enum in com.facebook.buck.parser.api")    

      : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
