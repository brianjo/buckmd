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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Class NativeLinkTargetMode {#class-nativelinktargetmode .title title="Class NativeLinkTargetMode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.nativelink.NativeLinkTargetMode

::: description
-   

    ------------------------------------------------------------------------

        public abstract class NativeLinkTargetMode
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `NativeLinkTargetMode()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type               Method                               Description
          ------------------------------- ------------------------------------ -------------
          `void`                          `check()`                             
          `static NativeLinkTargetMode`   `executable()`                        
          `abstract Optional<String>`     `getLibraryName()`                    
          `abstract Linker.LinkType`      `getType()`                           
          `static NativeLinkTargetMode`   `library()`                           
          `static NativeLinkTargetMode`   `library​(String soname)`              
          `static NativeLinkTargetMode`   `library​(Optional<String> soname)`    

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

        -   #### NativeLinkTargetMode

                public NativeLinkTargetMode()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract Linker.LinkType getType()
            ```

            [Returns:]{.returnLabel}
            :   the link type.

        []{#getLibraryName()}

        -   #### getLibraryName

            ``` methodSignature
            public abstract Optional<String> getLibraryName()
            ```

            [Returns:]{.returnLabel}
            :   the name of the library, if applicable.

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            public void check()
            ```

        []{#executable()}

        -   #### executable

            ``` methodSignature
            public static NativeLinkTargetMode executable()
            ```

        []{#library(java.util.Optional)}

        -   #### library

            ``` methodSignature
            public static NativeLinkTargetMode library​(Optional<String> soname)
            ```

        []{#library(java.lang.String)}

        -   #### library

            ``` methodSignature
            public static NativeLinkTargetMode library​(String soname)
            ```

        []{#library()}

        -   #### library

            ``` methodSignature
            public static NativeLinkTargetMode library()
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
