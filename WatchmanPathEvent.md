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

## Class WatchmanPathEvent {#class-watchmanpathevent .title title="Class WatchmanPathEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.watchman.WatchmanPathEvent

::: description
-   

    All Implemented Interfaces:
    :   `WatchmanEvent`

    ------------------------------------------------------------------------

        public abstract class WatchmanPathEvent
        extends Object
        implements WatchmanEvent

    ::: block
    Buck sends this event for every file that was added, modified or
    deleted
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.io.watchman.WatchmanEvent}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.io.watchman.[WatchmanEvent](WatchmanEvent.html "interface in com.facebook.buck.io.watchman")

            `WatchmanEvent.Kind, WatchmanEvent.Type`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `WatchmanPathEvent()`    

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
        | `abstrac              | `getKind()`           | ::: block             |
        | t WatchmanEvent.Kind` |                       | The kind of event     |
        |                       |                       | that occurred.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract RelPath`    | `getPath()`           | ::: block             |
        |                       |                       | Relative path of the  |
        |                       |                       | actual file the event |
        |                       |                       | is about.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `o                    |                       |
        | ic WatchmanPathEvent` | f​(AbsPath cellPath,   |                       |
        |                       |  WatchmanEvent.Kind k |                       |
        |                       | ind,   RelPath path)` |                       |
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

        -   #### WatchmanPathEvent

                public WatchmanPathEvent()
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

        []{#getKind()}

        -   #### getKind

            ``` methodSignature
            public abstract WatchmanEvent.Kind getKind()
            ```

            ::: block
            The kind of event that occurred.
            :::

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public abstract RelPath getPath()
            ```

            ::: block
            Relative path of the actual file the event is about. The
            path is relative to the cell path returned by
            [`getCellPath()`](#getCellPath()).
            :::

        []{#of(com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.io.watchman.WatchmanEvent.Kind,com.facebook.buck.core.filesystems.RelPath)}

        -   #### of

            ``` methodSignature
            public static WatchmanPathEvent of​(AbsPath cellPath,
                                               WatchmanEvent.Kind kind,
                                               RelPath path)
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