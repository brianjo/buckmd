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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.tool.impl](package-summary.html)
:::

## Class VersionedTool {#class-versionedtool .title title="Class VersionedTool"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.toolchain.tool.impl.VersionedTool

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `HasCustomInputsLogic`, `Tool`

    ------------------------------------------------------------------------

        public abstract class VersionedTool
        extends Object
        implements Tool, HasCustomInputsLogic

    ::: block
    A
    [`Tool`](../Tool.html "interface in com.facebook.buck.core.toolchain.tool")
    which only contributes a fixed name and version when appended to a
    rule key. This class also holds a
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
    reference to the tool and additional flags used when invoking the
    tool, which do \*not\* themselves contribute to the rule key. This
    is useful in situations such as supporting cross-compilation, in
    which case the different tools themselves might not be bit-by-bit
    identical (and, similarly, they might need to invoked with slightly
    different flags) but we know that they produce identical output, in
    which case they should also generate identical rule keys.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `VersionedTool()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<E ex                | `computeInputs        |                       |
        | tends Exception>void` | ​(ThrowingConsumer<Sou |                       |
        |                       | rcePath,​E> consumer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getCommandP          |                       |
        | ogle.common.collect.I | refix​(SourcePathResol |                       |
        | mmutableList<String>` | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getEnviro            |                       |
        | ommon.collect.Immutab | nment​(SourcePathResol |                       |
        | leMap<String,​String>` | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getExtraArgs()`      | ::: block             |
        | ogle.common.collect.I |                       | Additional flags that |
        | mmutableList<String>` |                       | we pass to the tool,  |
        |                       |                       | but which do \*not\*  |
        |                       |                       | contribute to the     |
        |                       |                       | rule key.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getPath()`           | ::: block             |
        | tract PathSourcePath` |                       | The path to the tool. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getVersion()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(String name,      |                       |
        | static VersionedTool` |    PathSourcePath pat |                       |
        |                       | h,   String version)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(String nam        |                       |
        | static VersionedTool` | e,   PathSourcePath p |                       |
        |                       | ath,   String version |                       |
        |                       | ,   com.google.common |                       |
        |                       | .collect.ImmutableLis |                       |
        |                       | t<String> extraArgs)` |                       |
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

        -   #### VersionedTool

                public VersionedTool()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public abstract String getName()
            ```

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public abstract PathSourcePath getPath()
            ```

            ::: block
            The path to the tool. The contents or path to the tool do
            not contribute to the rule key.
            :::

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            public abstract String getVersion()
            ```

        []{#getExtraArgs()}

        -   #### getExtraArgs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getExtraArgs()
            ```

            ::: block
            Additional flags that we pass to the tool, but which do
            \*not\* contribute to the rule key.
            :::

        []{#getCommandPrefix(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getCommandPrefix

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCommandPrefix​(SourcePathResolverAdapter resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCommandPrefix` in interface `Tool`

            [Returns:]{.returnLabel}
            :   the prefix command use to run this tool.

        []{#getEnvironment(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getEnvironment

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironment​(SourcePathResolverAdapter resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnvironment` in interface `Tool`

            [Returns:]{.returnLabel}
            :   the list of environment variables to set when running
                the command.

        []{#computeInputs(com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### computeInputs

            ``` methodSignature
            public <E extends Exception> void computeInputs​(ThrowingConsumer<SourcePath,​E> consumer)
                                                     throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeInputs` in interface `HasCustomInputsLogic`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#of(java.lang.String,com.facebook.buck.core.sourcepath.PathSourcePath,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static VersionedTool of​(String name,
                                           PathSourcePath path,
                                           String version)
            ```

        []{#of(java.lang.String,com.facebook.buck.core.sourcepath.PathSourcePath,java.lang.String,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static VersionedTool of​(String name,
                                           PathSourcePath path,
                                           String version,
                                           com.google.common.collect.ImmutableList<String> extraArgs)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
