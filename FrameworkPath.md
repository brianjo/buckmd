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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class FrameworkPath {#class-frameworkpath .title title="Class FrameworkPath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.FrameworkPath

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Comparable<FrameworkPath>`

    ------------------------------------------------------------------------

        public abstract class FrameworkPath
        extends Object
        implements Comparable<FrameworkPath>, AddsToRuleKey

    ::: block
    Frameworks can be specified as either a path to a file, or a path
    prefixed by a build setting.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `pro                  | `FrameworkPath.Type`  | ::: block             |
        | tected static class ` |                       | The type of framework |
        |                       |                       | entry this object     |
        |                       |                       | represents.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `FrameworkPath()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                                                                                                                                                                            Description
          ------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected void`                      `check()`                                                                                                                                                                                                          
          `int`                                 `compareTo​(FrameworkPath o)`                                                                                                                                                                                       
          `Iterator<BuildRule>`                 `getDeps​(SourcePathRuleFinder ruleFinder)`                                                                                                                                                                         
          `Path`                                `getFileName​(java.util.function.Function<SourcePath,​Path> resolver)`                                                                                                                                               
          `String`                              `getName​(java.util.function.Function<SourcePath,​Path> resolver)`                                                                                                                                                   
          `abstract Optional<SourcePath>`       `getSourcePath()`                                                                                                                                                                                                  
          `abstract Optional<SourceTreePath>`   `getSourceTreePath()`                                                                                                                                                                                              
          `abstract FrameworkPath.Type`         `getType()`                                                                                                                                                                                                        
          `static Path`                         `getUnexpandedSearchPath​(java.util.function.Function<SourcePath,​Path> resolver,                        java.util.function.Function<? super Path,​Path> relativizer,                        FrameworkPath input)`    
          `boolean`                             `isSDKROOTFrameworkPath()`                                                                                                                                                                                         
          `static FrameworkPath`                `of​(FrameworkPath.Type type,   Optional<? extends SourceTreePath> sourceTreePath,   Optional<? extends SourcePath> sourcePath)`                                                                                    
          `static FrameworkPath`                `ofSourcePath​(SourcePath sourcePath)`                                                                                                                                                                              
          `static FrameworkPath`                `ofSourceTreePath​(SourceTreePath sourceTreePath)`                                                                                                                                                                  

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

        -   #### FrameworkPath

                public FrameworkPath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract FrameworkPath.Type getType()
            ```

        []{#getSourceTreePath()}

        -   #### getSourceTreePath

            ``` methodSignature
            public abstract Optional<SourceTreePath> getSourceTreePath()
            ```

        []{#getSourcePath()}

        -   #### getSourcePath

            ``` methodSignature
            public abstract Optional<SourcePath> getSourcePath()
            ```

        []{#getDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getDeps

            ``` methodSignature
            public Iterator<BuildRule> getDeps​(SourcePathRuleFinder ruleFinder)
            ```

        []{#getFileName(java.util.function.Function)}

        -   #### getFileName

            ``` methodSignature
            public Path getFileName​(java.util.function.Function<SourcePath,​Path> resolver)
            ```

        []{#getName(java.util.function.Function)}

        -   #### getName

            ``` methodSignature
            public String getName​(java.util.function.Function<SourcePath,​Path> resolver)
            ```

        []{#isSDKROOTFrameworkPath()}

        -   #### isSDKROOTFrameworkPath

            ``` methodSignature
            public boolean isSDKROOTFrameworkPath()
            ```

        []{#getUnexpandedSearchPath(java.util.function.Function,java.util.function.Function,com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### getUnexpandedSearchPath

            ``` methodSignature
            public static Path getUnexpandedSearchPath​(java.util.function.Function<SourcePath,​Path> resolver,
                                                       java.util.function.Function<? super Path,​Path> relativizer,
                                                       FrameworkPath input)
            ```

        []{#of(com.facebook.buck.rules.coercer.FrameworkPath.Type,java.util.Optional,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static FrameworkPath of​(FrameworkPath.Type type,
                                           Optional<? extends SourceTreePath> sourceTreePath,
                                           Optional<? extends SourcePath> sourcePath)
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#compareTo(com.facebook.buck.rules.coercer.FrameworkPath)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(FrameworkPath o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<FrameworkPath>`

        []{#ofSourceTreePath(com.facebook.buck.apple.xcode.xcodeproj.SourceTreePath)}

        -   #### ofSourceTreePath

            ``` methodSignature
            public static FrameworkPath ofSourceTreePath​(SourceTreePath sourceTreePath)
            ```

        []{#ofSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### ofSourcePath

            ``` methodSignature
            public static FrameworkPath ofSourcePath​(SourcePath sourcePath)
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
