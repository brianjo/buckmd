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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class WatchmanFactory {#class-watchmanfactory .title title="Class WatchmanFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.watchman.WatchmanFactory

::: description
-   

    ------------------------------------------------------------------------

        public class WatchmanFactory
        extends Object

    ::: block
    Factory that is responsible for creating instances of
    [`Watchman`](Watchman.html "class in com.facebook.buck.io.watchman").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field             Description
          ------------------- ----------------- -------------
          `static String`     `NULL_CLOCK`       
          `static Watchman`   `NULL_WATCHMAN`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                             Description
          ------------------------------------------------------------------------------------------------------- -------------
          `WatchmanFactory()`                                                                                      
          `WatchmanFactory​(com.facebook.buck.io.watchman.WatchmanFactory.InitialWatchmanClientFactory factory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Watchman`            | `build​(co             |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableSet<AbsPa |                       |
        |                       | th> projectWatchList, |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableM |                       |
        |                       | ap<String,​String> env |                       |
        |                       | ,      Console consol |                       |
        |                       | e,      Clock clock,  |                       |
        |                       |      Optional<Long> c |                       |
        |                       | ommandTimeoutMillis)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `create               |                       |
        | tatic WatchmanClient` | WatchmanClient​(Path t |                       |
        |                       | ransportPath,         |                       |
        |                       |              Console  |                       |
        |                       | console,              |                       |
        |                       |         Clock clock)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Watchman`     | `getWatchman​(Wat      | ::: block             |
        |                       | chmanClient client,   | Query Watchman\'s     |
        |                       |           Path transp | capabilities and      |
        |                       | ortPath,            c | watch the given       |
        |                       | om.google.common.coll | directories.          |
        |                       | ect.ImmutableSet<AbsP | :::                   |
        |                       | ath> projectWatchList |                       |
        |                       | ,            Console  |                       |
        |                       | console,            C |                       |
        |                       | lock clock,           |                       |
        |                       |   long endTimeNanos)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#NULL_CLOCK}

        -   #### NULL_CLOCK

                public static final String NULL_CLOCK

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.watchman.WatchmanFactory.NULL_CLOCK)

        []{#NULL_WATCHMAN}

        -   #### NULL_WATCHMAN

                public static final Watchman NULL_WATCHMAN
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### WatchmanFactory

                public WatchmanFactory()

        []{#<init>(com.facebook.buck.io.watchman.WatchmanFactory.InitialWatchmanClientFactory)}

        -   #### WatchmanFactory

                public WatchmanFactory​(com.facebook.buck.io.watchman.WatchmanFactory.InitialWatchmanClientFactory factory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build(com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableMap,com.facebook.buck.util.Console,com.facebook.buck.util.timing.Clock,java.util.Optional)}

        -   #### build

            ``` methodSignature
            public Watchman build​(com.google.common.collect.ImmutableSet<AbsPath> projectWatchList,
                                  com.google.common.collect.ImmutableMap<String,​String> env,
                                  Console console,
                                  Clock clock,
                                  Optional<Long> commandTimeoutMillis)
                           throws InterruptedException
            ```

            [Returns:]{.returnLabel}
            :   new instance of
                [`Watchman`](Watchman.html "class in com.facebook.buck.io.watchman")
                using the specified params.

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#getWatchman(com.facebook.buck.io.watchman.WatchmanClient,java.nio.file.Path,com.google.common.collect.ImmutableSet,com.facebook.buck.util.Console,com.facebook.buck.util.timing.Clock,long)}

        -   #### getWatchman

            ``` methodSignature
            public static Watchman getWatchman​(WatchmanClient client,
                                               Path transportPath,
                                               com.google.common.collect.ImmutableSet<AbsPath> projectWatchList,
                                               Console console,
                                               Clock clock,
                                               long endTimeNanos)
                                        throws IOException,
                                               InterruptedException
            ```

            ::: block
            Query Watchman\'s capabilities and watch the given
            directories.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#createWatchmanClient(java.nio.file.Path,com.facebook.buck.util.Console,com.facebook.buck.util.timing.Clock)}

        -   #### createWatchmanClient

            ``` methodSignature
            public static WatchmanClient createWatchmanClient​(Path transportPath,
                                                              Console console,
                                                              Clock clock)
                                                       throws IOException
            ```

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
