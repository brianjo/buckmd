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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.common](package-summary.html)
:::

## Class CopyInXcode {#class-copyinxcode .title title="Class CopyInXcode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.common.CopyInXcode

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CopyInXcode
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                           Description
          ------------------- ------------------------------- -------------
          `static class `     `CopyInXcode.DestinationBase`    
          `static class `     `CopyInXcode.SourceType`         

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `CopyInXcode()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                        Method                                                                                                                              Description
          ---------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract CopyInXcode.DestinationBase`   `getDestinationBase()`                                                                                                               
          `abstract Path`                          `getDestinationPath()`                                                                                                               
          `abstract Path`                          `getSourcePath()`                                                                                                                    
          `abstract CopyInXcode.SourceType`        `getSourceType()`                                                                                                                    
          `static CopyInXcode`                     `of​(CopyInXcode.SourceType sourceType,   Path sourcePath,   CopyInXcode.DestinationBase destinationBase,   Path destinationPath)`    

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

        -   #### CopyInXcode

                public CopyInXcode()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.features.apple.common.CopyInXcode.SourceType,java.nio.file.Path,com.facebook.buck.features.apple.common.CopyInXcode.DestinationBase,java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static CopyInXcode of​(CopyInXcode.SourceType sourceType,
                                         Path sourcePath,
                                         CopyInXcode.DestinationBase destinationBase,
                                         Path destinationPath)
            ```

        []{#getSourceType()}

        -   #### getSourceType

            ``` methodSignature
            public abstract CopyInXcode.SourceType getSourceType()
            ```

        []{#getSourcePath()}

        -   #### getSourcePath

            ``` methodSignature
            public abstract Path getSourcePath()
            ```

        []{#getDestinationBase()}

        -   #### getDestinationBase

            ``` methodSignature
            public abstract CopyInXcode.DestinationBase getDestinationBase()
            ```

        []{#getDestinationPath()}

        -   #### getDestinationPath

            ``` methodSignature
            public abstract Path getDestinationPath()
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
