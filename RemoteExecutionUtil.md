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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class RemoteExecutionUtil {#class-remoteexecutionutil .title title="Class RemoteExecutionUtil"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.RemoteExecutionUtil

::: description
-   

    ------------------------------------------------------------------------

        public class RemoteExecutionUtil
        extends Object

    ::: block
    Auxiliary utils to be used for starting/configuring/annotating etc.
    RE builds.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `prot                 | `doTargetsMatchProje  | ::: block             |
        | ected static boolean` | ctWhitelist​(com.googl | Checks whether the    |
        |                       | e.common.collect.Immu | given targets match   |
        |                       | tableSet<String> buil | the RE project        |
        |                       | dTargets,             | whitelist             |
        |                       |                    co | :::                   |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableSet<Strin |                       |
        |                       | g> projectWhitelist)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `doTargetsMatchPr     | ::: block             |
        |                       | ojectWhitelist​(List<S | Checks whether the    |
        |                       | tring> commandArgs,   | given target command  |
        |                       |                       | line arguments match  |
        |                       |         com.google.co | the RE project        |
        |                       | mmon.collect.Immutabl | whitelist             |
        |                       | eSet<String> projectW | :::                   |
        |                       | hitelist,             |                       |
        |                       |                    Bu |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `getCommonP           | ::: block             |
        | tic Optional<String>` | rojectPrefix​(List<Str | Given a list of       |
        |                       | ing> commandArgs,     | targets, determines   |
        |                       |                    Bu | if they all share a   |
        |                       | ckConfig buckConfig)` | common prefix, and if |
        |                       |                       | they do then returns  |
        |                       |                       | it.                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#doTargetsMatchProjectWhitelist(java.util.List,com.google.common.collect.ImmutableSet,com.facebook.buck.core.config.BuckConfig)}

        -   #### doTargetsMatchProjectWhitelist

            ``` methodSignature
            public static boolean doTargetsMatchProjectWhitelist​(List<String> commandArgs,
                                                                 com.google.common.collect.ImmutableSet<String> projectWhitelist,
                                                                 BuckConfig buckConfig)
            ```

            ::: block
            Checks whether the given target command line arguments match
            the RE project whitelist
            :::

        []{#getCommonProjectPrefix(java.util.List,com.facebook.buck.core.config.BuckConfig)}

        -   #### getCommonProjectPrefix

            ``` methodSignature
            public static Optional<String> getCommonProjectPrefix​(List<String> commandArgs,
                                                                  BuckConfig buckConfig)
            ```

            ::: block
            Given a list of targets, determines if they all share a
            common prefix, and if they do then returns it. E.g. for
            targets \'//project_one:a\', \'//project_one:b\', should
            return \'//project_one\'
            :::

        []{#doTargetsMatchProjectWhitelist(com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet)}

        -   #### doTargetsMatchProjectWhitelist

            ``` methodSignature
            protected static boolean doTargetsMatchProjectWhitelist​(com.google.common.collect.ImmutableSet<String> buildTargets,
                                                                    com.google.common.collect.ImmutableSet<String> projectWhitelist)
            ```

            ::: block
            Checks whether the given targets match the RE project
            whitelist
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
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
