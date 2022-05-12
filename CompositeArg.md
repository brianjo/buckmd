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
[Package]{.packageLabelInType} [com.facebook.buck.rules.args](package-summary.html)
:::

## Class CompositeArg {#class-compositearg .title title="Class CompositeArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.args.CompositeArg

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Arg`

    ------------------------------------------------------------------------

        public abstract class CompositeArg
        extends Object
        implements Arg

    ::: block
    CompositeArg holds a list of args and appends them all to the
    command-line. It does not add any separator between the args, so if
    that\'s necessary it should be added via StringArgs in the list of
    Args.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `CompositeArg()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `appendToCommandLine​( | ::: block             |
        |                       | java.util.function.Co | Feed the contents of  |
        |                       | nsumer<String> consum | the Arg to the        |
        |                       | er,                   | supplied consumer.    |
        |                       |   SourcePathResolverA | :::                   |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ap                   |                       |
        |                       | pendToCommandLineRel​( |                       |
        |                       | java.util.function.Co |                       |
        |                       | nsumer<String> consum |                       |
        |                       | er,                   |                       |
        |                       |      CanonicalCellNam |                       |
        |                       | e cellName,           |                       |
        |                       |              SourcePa |                       |
        |                       | thResolverAdapter pat |                       |
        |                       | hResolver,            |                       |
        |                       |             boolean u |                       |
        |                       | seUnixPathSeparator)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CompositeArg` | `of​(com.googl         |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableList<Arg> args)` |                       |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.args.Arg}

            ### Methods inherited from interface com.facebook.buck.rules.args.[Arg](Arg.html "interface in com.facebook.buck.rules.args")

            `equals, hashCode, singleCommandLineArg, toString`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CompositeArg

                public CompositeArg()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#appendToCommandLine(java.util.function.Consumer,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### appendToCommandLine

            ``` methodSignature
            public void appendToCommandLine​(java.util.function.Consumer<String> consumer,
                                            SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            [Description copied from
            interface: `Arg`]{.descfrmTypeLabel}
            :::

            ::: block
            Feed the contents of the Arg to the supplied consumer. This
            call may feed any number of elements (including zero) into
            the consumer. This is only ever safe to call when the rule
            is running, as it may do things like resolving source paths.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `appendToCommandLine` in interface `Arg`

        []{#appendToCommandLineRel(java.util.function.Consumer,com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,boolean)}

        -   #### appendToCommandLineRel

            ``` methodSignature
            public void appendToCommandLineRel​(java.util.function.Consumer<String> consumer,
                                               CanonicalCellName cellName,
                                               SourcePathResolverAdapter pathResolver,
                                               boolean useUnixPathSeparator)
            ```

        []{#of(com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static CompositeArg of​(com.google.common.collect.ImmutableList<Arg> args)
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