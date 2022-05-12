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
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   Nested \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.io.watchman](package-summary.html)
:::

## Class Watchman {#class-watchman .title title="Class Watchman"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.watchman.Watchman

::: description
-   

    ------------------------------------------------------------------------

        public abstract class Watchman
        extends Object

    ::: block
    Contains the configuration for a Watchman client as well as the
    ability to create a client.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                              Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Watchman​(com.google.common.collect.ImmutableMap<AbsPath,​ProjectWatch> projectWatches,         com.google.common.collect.ImmutableSet<Capability> capabilities,         com.google.common.collect.ImmutableMap<String,​String> clockIds,         Optional<Path> transportPath,         String version)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `buildCloc            | ::: block             |
        | com.google.common.col | kWatchmanCursorMap()` | Build.                |
        | lect.ImmutableMap<Abs |                       | :::                   |
        | Path,​WatchmanCursor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `buildName            | ::: block             |
        | com.google.common.col | dWatchmanCursorMap()` | Build.                |
        | lect.ImmutableMap<Abs |                       | :::                   |
        | Path,​WatchmanCursor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `createClient()`      | ::: block             |
        | tract WatchmanClient` |                       | Note this method will |
        |                       |                       | throw an              |
        |                       |                       | [`IOException`](http  |
        |                       |                       | ://docs.oracle.com/ja |
        |                       |                       | vase/7/docs/api/java/ |
        |                       |                       | io/IOException.html?i |
        |                       |                       | s-external=true "clas |
        |                       |                       | s or interface in jav |
        |                       |                       | a.io"){.externalLink} |
        |                       |                       | if:                   |
        |                       |                       | [                     |
        |                       |                       | `getTransportPath()`] |
        |                       |                       | (#getTransportPath()) |
        |                       |                       | returns               |
        |                       |                       | [`Optional.em         |
        |                       |                       | pty()`](http://docs.o |
        |                       |                       | racle.com/javase/7/do |
        |                       |                       | cs/api/java/util/Opti |
        |                       |                       | onal.html?is-external |
        |                       |                       | =true#empty() "class  |
        |                       |                       | or interface in java. |
        |                       |                       | util"){.externalLink} |
        |                       |                       | It cannot establish a |
        |                       |                       | connection to         |
        |                       |                       | Watchman.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getCapabilities()`   |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<Capability>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getClockIds()`       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `getProjectWatches()` |                       |
        | ollect.ImmutableMap<A |                       |                       |
        | bsPath,​ProjectWatch>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getTransportPath()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getVersion()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasWildmatchGlob()`  |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableMap,java.util.Optional,java.lang.String)}

        -   #### Watchman

                public Watchman​(com.google.common.collect.ImmutableMap<AbsPath,​ProjectWatch> projectWatches,
                                com.google.common.collect.ImmutableSet<Capability> capabilities,
                                com.google.common.collect.ImmutableMap<String,​String> clockIds,
                                Optional<Path> transportPath,
                                String version)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#buildClockWatchmanCursorMap()}

        -   #### buildClockWatchmanCursorMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<AbsPath,​WatchmanCursor> buildClockWatchmanCursorMap()
            ```

            ::: block
            Build.
            :::

        []{#buildNamedWatchmanCursorMap()}

        -   #### buildNamedWatchmanCursorMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<AbsPath,​WatchmanCursor> buildNamedWatchmanCursorMap()
            ```

            ::: block
            Build.
            :::

        []{#getProjectWatches()}

        -   #### getProjectWatches

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<AbsPath,​ProjectWatch> getProjectWatches()
            ```

        []{#getCapabilities()}

        -   #### getCapabilities

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Capability> getCapabilities()
            ```

        []{#getClockIds()}

        -   #### getClockIds

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getClockIds()
            ```

        []{#hasWildmatchGlob()}

        -   #### hasWildmatchGlob

            ``` methodSignature
            public boolean hasWildmatchGlob()
            ```

        []{#getTransportPath()}

        -   #### getTransportPath

            ``` methodSignature
            public Optional<Path> getTransportPath()
            ```

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            public String getVersion()
            ```

        []{#createClient()}

        -   #### createClient

            ``` methodSignature
            public abstract WatchmanClient createClient()
                                                 throws IOException
            ```

            ::: block
            Note this method will throw an
            [`IOException`](http://docs.oracle.com/javase/7/docs/api/java/io/IOException.html?is-external=true "class or interface in java.io"){.externalLink}
            if:
            -   [`getTransportPath()`](#getTransportPath()) returns
                [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
            -   It cannot establish a connection to Watchman.
            :::

            [Returns:]{.returnLabel}
            :   a new client that the caller is responsible for closing.

            [Throws:]{.throwsLabel}
            :   `IOException`
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   Nested \| 
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
