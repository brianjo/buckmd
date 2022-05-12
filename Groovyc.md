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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.groovy](package-summary.html)
:::

## Class Groovyc {#class-groovyc .title title="Class Groovyc"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.groovy.Groovyc

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`

    ------------------------------------------------------------------------

        public class Groovyc
        extends Object
        implements Tool
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field           Description
          ------------------- --------------- -------------
          `static String`     `BIN_GROOVYC`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                  Description
          -------------------------------------------------------------------------------------------- -------------
          `Groovyc​(SourcePath path,        boolean external)`                                           
          `Groovyc​(java.util.function.Supplier<? extends SourcePath> path,        boolean external)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                   Description
          --------------------------------------------------------- -------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<String>`         `getCommandPrefix​(SourcePathResolverAdapter resolver)`    
          `com.google.common.collect.ImmutableMap<String,​String>`   `getEnvironment​(SourcePathResolverAdapter resolver)`      

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
    -   []{#field.detail}

        ### Field Detail

        []{#BIN_GROOVYC}

        -   #### BIN_GROOVYC

                public static String BIN_GROOVYC
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Supplier,boolean)}

        -   #### Groovyc

                public Groovyc​(java.util.function.Supplier<? extends SourcePath> path,
                               boolean external)

        []{#<init>(com.facebook.buck.core.sourcepath.SourcePath,boolean)}

        -   #### Groovyc

                public Groovyc​(SourcePath path,
                               boolean external)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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
