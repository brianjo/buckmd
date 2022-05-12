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
[Package]{.packageLabelInType} [com.facebook.buck.swift.toolchain](package-summary.html)
:::

## Class SwiftTargetTriple {#class-swifttargettriple .title title="Class SwiftTargetTriple"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.swift.toolchain.SwiftTargetTriple

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class SwiftTargetTriple
        extends Object
        implements AddsToRuleKey

    ::: block
    Expresses the target platform for Swift compilation. For more
    details, see the LLVM documentation:
    https://clang.llvm.org/docs/CrossCompilation.html#target-triple
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `SwiftTargetTriple()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                                                                                Description
          ---------------------------- --------------------------------------------------------------------------------------------------------------------- -------------
          `abstract String`            `getArchitecture()`                                                                                                    
          `abstract Boolean`           `getIsSimulator()`                                                                                                     
          `abstract String`            `getPlatformName()`                                                                                                    
          `abstract String`            `getTargetSdkVersion()`                                                                                                
          `String`                     `getTriple()`                                                                                                          
          `abstract String`            `getVendor()`                                                                                                          
          `static SwiftTargetTriple`   `of​(String architecture,   String vendor,   String platformName,   String targetSdkVersion,   Boolean isSimulator)`    
          `SwiftTargetTriple`          `withTargetSdkVersion​(String targetSdkVersion)`                                                                        

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

        -   #### SwiftTargetTriple

                public SwiftTargetTriple()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getArchitecture()}

        -   #### getArchitecture

            ``` methodSignature
            public abstract String getArchitecture()
            ```

        []{#getVendor()}

        -   #### getVendor

            ``` methodSignature
            public abstract String getVendor()
            ```

        []{#getPlatformName()}

        -   #### getPlatformName

            ``` methodSignature
            public abstract String getPlatformName()
            ```

        []{#getTargetSdkVersion()}

        -   #### getTargetSdkVersion

            ``` methodSignature
            public abstract String getTargetSdkVersion()
            ```

        []{#getIsSimulator()}

        -   #### getIsSimulator

            ``` methodSignature
            public abstract Boolean getIsSimulator()
            ```

        []{#getTriple()}

        -   #### getTriple

            ``` methodSignature
            public String getTriple()
            ```

        []{#of(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.Boolean)}

        -   #### of

            ``` methodSignature
            public static SwiftTargetTriple of​(String architecture,
                                               String vendor,
                                               String platformName,
                                               String targetSdkVersion,
                                               Boolean isSimulator)
            ```

        []{#withTargetSdkVersion(java.lang.String)}

        -   #### withTargetSdkVersion

            ``` methodSignature
            public SwiftTargetTriple withTargetSdkVersion​(String targetSdkVersion)
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
