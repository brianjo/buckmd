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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class ExternalJavacProvider {#class-externaljavacprovider .title title="Class ExternalJavacProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.ExternalJavacProvider

::: description
-   

    All Implemented Interfaces:
    :   `JavacProvider`

    ------------------------------------------------------------------------

        public class ExternalJavacProvider
        extends Object
        implements JavacProvider

    ::: block
    Provides utilities for creating/providing javac instances.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                  Description
          ------------------- -------------------------------------- -------------
          `static String`     `COM_SUN_TOOLS_JAVAC_API_JAVAC_TOOL`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                     Description
          ----------------------------------------------- -------------
          `ExternalJavacProvider​(SourcePath javacPath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addParseTimeDe       |                       |
        |                       | ps​(com.google.common. |                       |
        |                       | collect.ImmutableColl |                       |
        |                       | ection.Builder<BuildT |                       |
        |                       | arget> depsConsumer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getB                 |                       |
        | le.common.collect.Imm | uildDeps​(SourcePathRu |                       |
        | utableSet<BuildRule>` | leFinder ruleFinder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getProviderFor       | ::: block             |
        | static JavacProvider` | Spec​(JavacSpec spec)` | Creates a             |
        |                       |                       | JavacProvider based   |
        |                       |                       | on a spec.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Javac`               | `resolve​(SourcePathRu | ::: block             |
        |                       | leFinder ruleFinder)` | Creates an            |
        |                       |                       | ExternalJavac.        |
        |                       |                       | :::                   |
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

        []{#COM_SUN_TOOLS_JAVAC_API_JAVAC_TOOL}

        -   #### COM_SUN_TOOLS_JAVAC_API_JAVAC_TOOL

                public static final String COM_SUN_TOOLS_JAVAC_API_JAVAC_TOOL

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.jvm.java.ExternalJavacProvider.COM_SUN_TOOLS_JAVAC_API_JAVAC_TOOL)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### ExternalJavacProvider

                public ExternalJavacProvider​(SourcePath javacPath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProviderForSpec(com.facebook.buck.jvm.java.JavacSpec)}

        -   #### getProviderForSpec

            ``` methodSignature
            public static JavacProvider getProviderForSpec​(JavacSpec spec)
            ```

            ::: block
            Creates a JavacProvider based on a spec.
            :::

        []{#resolve(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### resolve

            ``` methodSignature
            public Javac resolve​(SourcePathRuleFinder ruleFinder)
            ```

            ::: block
            Creates an ExternalJavac.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `JavacProvider`

        []{#addParseTimeDeps(com.google.common.collect.ImmutableCollection.Builder)}

        -   #### addParseTimeDeps

            ``` methodSignature
            public void addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> depsConsumer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addParseTimeDeps` in interface `JavacProvider`

        []{#getBuildDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getBuildDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> getBuildDeps​(SourcePathRuleFinder ruleFinder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildDeps` in interface `JavacProvider`
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
