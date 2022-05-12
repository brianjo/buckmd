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
[Package]{.packageLabelInType} [com.facebook.buck.io.watchman](package-summary.html)
:::

## Class WatchmanMultiplePathEvent {#class-watchmanmultiplepathevent .title title="Class WatchmanMultiplePathEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.watchman.WatchmanMultiplePathEvent

::: description
-   

    All Implemented Interfaces:
    :   `WatchmanEvent`

    ------------------------------------------------------------------------

        public abstract class WatchmanMultiplePathEvent
        extends Object
        implements WatchmanEvent

    ::: block
    Buck sends this event for all files, directories and symlinks that
    were changed since last invalidation
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `WatchmanMult         | ::: block             |
        |                       | iplePathEvent.Change` | Contains path and     |
        |                       |                       | type of file system   |
        |                       |                       | change                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.io.watchman.WatchmanEvent}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.io.watchman.[WatchmanEvent](WatchmanEvent.html "interface in com.facebook.buck.io.watchman")

            `WatchmanEvent.Kind, WatchmanEvent.Type`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `WatchmanMultiplePathEvent()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract AbsPath`    | `getCellPath()`       | ::: block             |
        |                       |                       | Absolute cell path    |
        |                       |                       | root being watched.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.google. | `getChanges()`        | ::: block             |
        | common.collect.Immuta |                       | All changes to        |
        | bleList<WatchmanMulti |                       | monitored file system |
        | plePathEvent.Change>` |                       | that occurred since   |
        |                       |                       | last invalidation     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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

        -   #### WatchmanMultiplePathEvent

                public WatchmanMultiplePathEvent()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellPath()}

        -   #### getCellPath

            ``` methodSignature
            public abstract AbsPath getCellPath()
            ```

            ::: block
            [Description copied from
            interface: `WatchmanEvent`]{.descfrmTypeLabel}
            :::

            ::: block
            Absolute cell path root being watched.
            :::

            [Specified by:]{.overrideSpecifyLabel}

            `getCellPath` in interface `WatchmanEvent`

            [Returns:]{.returnLabel}

        []{#getChanges()}

        -   #### getChanges

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<WatchmanMultiplePathEvent.Change> getChanges()
            ```

            ::: block
            All changes to monitored file system that occurred since
            last invalidation
            :::
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
