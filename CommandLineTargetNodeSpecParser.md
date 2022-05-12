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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class CommandLineTargetNodeSpecParser {#class-commandlinetargetnodespecparser .title title="Class CommandLineTargetNodeSpecParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.CommandLineTargetNodeSpecParser

::: description
-   

    ------------------------------------------------------------------------

        public class CommandLineTargetNodeSpecParser
        extends Object

    ::: block
    A helper wrapper over
    [`BuildTargetMatcherTargetNodeParser`](../parser/spec/BuildTargetMatcherTargetNodeParser.html "class in com.facebook.buck.parser.spec")
    to normalize user input before parsing, resolve aliases and validate
    that base path exists
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CommandLineTargetNodeSpecParser​(Cell rootCell,                                Path absoluteClientWorkingDirectory,                                BuckConfig config,                                BuildTargetMatcherTargetNodeParser parser)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected String`    | `                     |                       |
        |                       | normalizeBuildTargetS |                       |
        |                       | tring​(String target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `parse​(Cell owningCe  | ::: block             |
        | mmon.collect.Immutabl | ll,      String arg)` | Parse command line    |
        | eSet<TargetNodeSpec>` |                       | argument provided by  |
        |                       |                       | user into a set of    |
        |                       |                       | [`TargetNodeSpec      |
        |                       |                       | `](../parser/spec/Tar |
        |                       |                       | getNodeSpec.html "int |
        |                       |                       | erface in com.faceboo |
        |                       |                       | k.buck.parser.spec")s |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.cell.Cell,java.nio.file.Path,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.parser.spec.BuildTargetMatcherTargetNodeParser)}

        -   #### CommandLineTargetNodeSpecParser

                public CommandLineTargetNodeSpecParser​(Cell rootCell,
                                                       Path absoluteClientWorkingDirectory,
                                                       BuckConfig config,
                                                       BuildTargetMatcherTargetNodeParser parser)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#normalizeBuildTargetString(java.lang.String)}

        -   #### normalizeBuildTargetString

            ``` methodSignature
            protected String normalizeBuildTargetString​(String target)
            ```

        []{#parse(com.facebook.buck.core.cell.Cell,java.lang.String)}

        -   #### parse

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<TargetNodeSpec> parse​(Cell owningCell,
                                                                                String arg)
            ```

            ::: block
            Parse command line argument provided by user into a set of
            [`TargetNodeSpec`](../parser/spec/TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")s
            :::

            [Parameters:]{.paramLabel}
            :   `owningCell` - Cell that owns the resolution of a spec
            :   `arg` - Unresolved command line argument, can be alias
                or target name or recursive spec
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
