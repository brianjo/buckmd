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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath](package-summary.html)
:::

## Class SourceWithFlags {#class-sourcewithflags .title title="Class SourceWithFlags"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.sourcepath.SourceWithFlags

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Comparable<SourceWithFlags>`

    ------------------------------------------------------------------------

        public abstract class SourceWithFlags
        extends Object
        implements Comparable<SourceWithFlags>, AddsToRuleKey

    ::: block
    Simple type representing a
    [`SourcePath`](SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    and a list of file-specific flags.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `SourceWithFlags()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                                                                 Description
          ------------------------------------------------------------ -------------------------------------------------------------------------------------- -------------
          `int`                                                        `compareTo​(SourceWithFlags that)`                                                       
          `abstract com.google.common.collect.ImmutableList<String>`   `getFlags()`                                                                            
          `abstract SourcePath`                                        `getSourcePath()`                                                                       
          `static SourceWithFlags`                                     `of​(SourcePath sourcePath)`                                                             
          `static SourceWithFlags`                                     `of​(SourcePath sourcePath,   com.google.common.collect.ImmutableList<String> flags)`    
          `SourceWithFlags`                                            `withSourcePath​(SourcePath sourcePath)`                                                 

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

        -   #### SourceWithFlags

                public SourceWithFlags()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourcePath()}

        -   #### getSourcePath

            ``` methodSignature
            public abstract SourcePath getSourcePath()
            ```

        []{#getFlags()}

        -   #### getFlags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getFlags()
            ```

        []{#compareTo(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(SourceWithFlags that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<SourceWithFlags>`

        []{#of(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### of

            ``` methodSignature
            public static SourceWithFlags of​(SourcePath sourcePath)
            ```

        []{#of(com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static SourceWithFlags of​(SourcePath sourcePath,
                                             com.google.common.collect.ImmutableList<String> flags)
            ```

        []{#withSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### withSourcePath

            ``` methodSignature
            public SourceWithFlags withSourcePath​(SourcePath sourcePath)
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
