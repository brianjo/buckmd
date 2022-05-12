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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class GroupedSource {#class-groupedsource .title title="Class GroupedSource"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.GroupedSource

::: description
-   

    ------------------------------------------------------------------------

        public abstract class GroupedSource
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `GroupedSource.Type`  | ::: block             |
        |                       |                       | The type of grouped   |
        |                       |                       | source entry this     |
        |                       |                       | object represents.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `G                    |                       |
        |                       | roupedSource.Visitor` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `GroupedSource()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getN                 |                       |
        |                       | ame​(java.util.functio |                       |
        |                       | n.Function<SourcePath |                       |
        |                       | ,​Path> pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protect              | `getSourceGroup()`    |                       |
        | ed abstract Optional< |                       |                       |
        | List<GroupedSource>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstr      | `                     |                       |
        | act Optional<String>` | getSourceGroupName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abs        | `getSourceGroupPa     |                       |
        | tract Optional<Path>` | thRelativeToTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstract   | `getSourcePath()`     |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `                     |                       |
        | tected abstract Optio | getSourceWithFlags()` |                       |
        | nal<SourceWithFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstrac    | `getType()`           |                       |
        | t GroupedSource.Type` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ofIgnoredSource​(So   | ::: block             |
        | static GroupedSource` | urcePath sourcePath)` | Creates a             |
        |                       |                       | [`Grouped             |
        |                       |                       | Source`](GroupedSourc |
        |                       |                       | e.html "class in com. |
        |                       |                       | facebook.buck.apple") |
        |                       |                       | given a               |
        |                       |                       | [`SourcePath`](       |
        |                       |                       | ../core/sourcepath/So |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | representing a file   |
        |                       |                       | that should not be    |
        |                       |                       | included in sources.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ofPrivateHeader​(So   | ::: block             |
        | static GroupedSource` | urcePath headerPath)` | Creates a             |
        |                       |                       | [`Grouped             |
        |                       |                       | Source`](GroupedSourc |
        |                       |                       | e.html "class in com. |
        |                       |                       | facebook.buck.apple") |
        |                       |                       | given a               |
        |                       |                       | [`SourcePath`](       |
        |                       |                       | ../core/sourcepath/So |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | representing a        |
        |                       |                       | private header file.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ofPublicHeader​(So    | ::: block             |
        | static GroupedSource` | urcePath headerPath)` | Creates a             |
        |                       |                       | [`Grouped             |
        |                       |                       | Source`](GroupedSourc |
        |                       |                       | e.html "class in com. |
        |                       |                       | facebook.buck.apple") |
        |                       |                       | given a               |
        |                       |                       | [`SourcePath`](       |
        |                       |                       | ../core/sourcepath/So |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | representing a public |
        |                       |                       | header file.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ofSourceGroup​(S      | ::: block             |
        | static GroupedSource` | tring sourceGroupName | Creates a             |
        |                       | ,              Path s | [`Grouped             |
        |                       | ourceGroupPathRelativ | Source`](GroupedSourc |
        |                       | eToTarget,            | e.html "class in com. |
        |                       |    Collection<Grouped | facebook.buck.apple") |
        |                       | Source> sourceGroup)` | given a source group  |
        |                       |                       | name and a list of    |
        |                       |                       | GroupedSources.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ofSourceW            | ::: block             |
        | static GroupedSource` | ithFlags​(SourceWithFl | Creates a             |
        |                       | ags sourceWithFlags)` | [`Grouped             |
        |                       |                       | Source`](GroupedSourc |
        |                       |                       | e.html "class in com. |
        |                       |                       | facebook.buck.apple") |
        |                       |                       | given a               |
        |                       |                       | [                     |
        |                       |                       | `SourceWithFlags`](.. |
        |                       |                       | /core/sourcepath/Sour |
        |                       |                       | ceWithFlags.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.core.sourcepath"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `visit​(GroupedSou     |                       |
        |                       | rce.Visitor visitor)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### GroupedSource

                public GroupedSource()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            protected abstract GroupedSource.Type getType()
            ```

        []{#getSourceWithFlags()}

        -   #### getSourceWithFlags

            ``` methodSignature
            protected abstract Optional<SourceWithFlags> getSourceWithFlags()
            ```

        []{#getSourcePath()}

        -   #### getSourcePath

            ``` methodSignature
            protected abstract Optional<SourcePath> getSourcePath()
            ```

        []{#getSourceGroupName()}

        -   #### getSourceGroupName

            ``` methodSignature
            protected abstract Optional<String> getSourceGroupName()
            ```

        []{#getSourceGroupPathRelativeToTarget()}

        -   #### getSourceGroupPathRelativeToTarget

            ``` methodSignature
            protected abstract Optional<Path> getSourceGroupPathRelativeToTarget()
            ```

        []{#getSourceGroup()}

        -   #### getSourceGroup

            ``` methodSignature
            protected abstract Optional<List<GroupedSource>> getSourceGroup()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#getName(java.util.function.Function)}

        -   #### getName

            ``` methodSignature
            public String getName​(java.util.function.Function<SourcePath,​Path> pathResolver)
            ```

        []{#ofSourceWithFlags(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### ofSourceWithFlags

            ``` methodSignature
            public static GroupedSource ofSourceWithFlags​(SourceWithFlags sourceWithFlags)
            ```

            ::: block
            Creates a
            [`GroupedSource`](GroupedSource.html "class in com.facebook.buck.apple")
            given a
            [`SourceWithFlags`](../core/sourcepath/SourceWithFlags.html "class in com.facebook.buck.core.sourcepath").
            :::

        []{#ofIgnoredSource(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### ofIgnoredSource

            ``` methodSignature
            public static GroupedSource ofIgnoredSource​(SourcePath sourcePath)
            ```

            ::: block
            Creates a
            [`GroupedSource`](GroupedSource.html "class in com.facebook.buck.apple")
            given a
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            representing a file that should not be included in sources.
            :::

        []{#ofPublicHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### ofPublicHeader

            ``` methodSignature
            public static GroupedSource ofPublicHeader​(SourcePath headerPath)
            ```

            ::: block
            Creates a
            [`GroupedSource`](GroupedSource.html "class in com.facebook.buck.apple")
            given a
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            representing a public header file.
            :::

        []{#ofPrivateHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### ofPrivateHeader

            ``` methodSignature
            public static GroupedSource ofPrivateHeader​(SourcePath headerPath)
            ```

            ::: block
            Creates a
            [`GroupedSource`](GroupedSource.html "class in com.facebook.buck.apple")
            given a
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            representing a private header file.
            :::

        []{#ofSourceGroup(java.lang.String,java.nio.file.Path,java.util.Collection)}

        -   #### ofSourceGroup

            ``` methodSignature
            public static GroupedSource ofSourceGroup​(String sourceGroupName,
                                                      Path sourceGroupPathRelativeToTarget,
                                                      Collection<GroupedSource> sourceGroup)
            ```

            ::: block
            Creates a
            [`GroupedSource`](GroupedSource.html "class in com.facebook.buck.apple")
            given a source group name and a list of GroupedSources.
            :::

        []{#visit(com.facebook.buck.apple.GroupedSource.Visitor)}

        -   #### visit

            ``` methodSignature
            public void visit​(GroupedSource.Visitor visitor)
            ```
    :::
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
