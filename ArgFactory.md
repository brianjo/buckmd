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
[Package]{.packageLabelInType} [com.facebook.buck.rules.args](package-summary.html)
:::

## Class ArgFactory {#class-argfactory .title title="Class ArgFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.args.ArgFactory

::: description
-   

    ------------------------------------------------------------------------

        public class ArgFactory
        extends Object

    ::: block
    Simple factory class to convert objects from
    [`CommandLineArgs`](../../core/rules/actions/lib/args/CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
    to [`Arg`](Arg.html "interface in com.facebook.buck.rules.args")
    objects
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Arg`          | `from​(Object object)` | ::: block             |
        |                       |                       | Convert a command     |
        |                       |                       | line argument to an   |
        |                       |                       | [`Arg`](Arg.html "i   |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.rules.args") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Arg`          | `fro                  |                       |
        |                       | m​(Object object,      |                       |
        |                       | String formatString)` |                       |
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

        []{#from(java.lang.Object,java.lang.String)}

        -   #### from

            ``` methodSignature
            public static Arg from​(Object object,
                                   String formatString)
            ```

        []{#from(java.lang.Object)}

        -   #### from

            ``` methodSignature
            public static Arg from​(Object object)
            ```

            ::: block
            Convert a command line argument to an
            [`Arg`](Arg.html "interface in com.facebook.buck.rules.args")
            :::

            [Parameters:]{.paramLabel}
            :   `object` - the object
                ([`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink},
                [`Artifact`](../../core/artifact/Artifact.html "interface in com.facebook.buck.core.artifact"),
                etc) to convert to an
                [`Arg`](Arg.html "interface in com.facebook.buck.rules.args")

            [Returns:]{.returnLabel}
            :   the arg

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if `object` is not able to
                be converted, or the provided object was an unbound
                [`Artifact`](../../core/artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
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
