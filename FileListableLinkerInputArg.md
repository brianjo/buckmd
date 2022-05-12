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

## Class FileListableLinkerInputArg {#class-filelistablelinkerinputarg .title title="Class FileListableLinkerInputArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.args.FileListableLinkerInputArg

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Arg`, `HasSourcePath`

    ------------------------------------------------------------------------

        public class FileListableLinkerInputArg
        extends Object
        implements Arg, HasSourcePath

    ::: block
    Arg that represents object file that should be linked into resulting
    binary using normal mechanism, e.g. passed to the linker without any
    additional surrounding flags. Sometimes these arguments can be
    grouped into a single text file that linker can pick up. This is
    mostly to simplify and shorten command line that is used to invoke
    the linker. This arg represents such kind of object file in the list
    of args, so later we can easily create such file list for the
    linker.
    :::
:::

::: summary
-   ::: {.section role="region"}
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
        | `void`                | `appendToC            |                       |
        |                       | ommandLineRel​(java.ut |                       |
        |                       | il.function.Consumer< |                       |
        |                       | String> consumer,     |                       |
        |                       |                    Ca |                       |
        |                       | nonicalCellName curre |                       |
        |                       | ntCellName,           |                       |
        |                       |              SourcePa |                       |
        |                       | thResolverAdapter pat |                       |
        |                       | hResolver,            |                       |
        |                       |             boolean u |                       |
        |                       | seUnixPathSeparator)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | equals​(Object other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `from​(                |                       |
        | .google.common.collec | com.google.common.col |                       |
        | t.ImmutableList<Arg>` | lect.ImmutableList<So |                       |
        |                       | urcePathArg> values)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getPath()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Arg`          | `withSourcePathArg​(   |                       |
        |                       | SourcePathArg value)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.args.Arg}

            ### Methods inherited from interface com.facebook.buck.rules.args.[Arg](Arg.html "interface in com.facebook.buck.rules.args")

            `singleCommandLineArg`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#withSourcePathArg(com.facebook.buck.rules.args.SourcePathArg)}

        -   #### withSourcePathArg

            ``` methodSignature
            public static Arg withSourcePathArg​(SourcePathArg value)
            ```

        []{#from(com.google.common.collect.ImmutableList)}

        -   #### from

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Arg> from​(com.google.common.collect.ImmutableList<SourcePathArg> values)
            ```

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
                                               CanonicalCellName currentCellName,
                                               SourcePathResolverAdapter pathResolver,
                                               boolean useUnixPathSeparator)
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in interface `Arg`

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   a
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}
                representation suitable to use for debugging.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `equals` in interface `Arg`

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hashCode` in interface `Arg`

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public SourcePath getPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPath` in interface `HasSourcePath`
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
