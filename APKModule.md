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
[Package]{.packageLabelInType} [com.facebook.buck.android.apkmodule](package-summary.html)
:::

## Class APKModule {#class-apkmodule .title title="Class APKModule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.apkmodule.APKModule

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Comparable<APKModule>`

    ------------------------------------------------------------------------

        public abstract class APKModule
        extends Object
        implements Comparable<APKModule>, AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor     Description
          --------------- -------------
          `APKModule()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                                                             Description
          -------------------- ------------------------------------------------------------------ -------------
          `int`                `compareTo​(APKModule o)`                                            
          `String`             `getCanaryClassName()`                                              
          `abstract String`    `getName()`                                                         
          `abstract boolean`   `hasManifest()`                                                     
          `abstract boolean`   `hasResources()`                                                    
          `boolean`            `isRootModule()`                                                    
          `static APKModule`   `of​(String name,   boolean hasResources,   boolean hasManifest)`    

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

        -   #### APKModule

                public APKModule()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.lang.String,boolean,boolean)}

        -   #### of

            ``` methodSignature
            public static APKModule of​(String name,
                                       boolean hasResources,
                                       boolean hasManifest)
            ```

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public abstract String getName()
            ```

        []{#hasResources()}

        -   #### hasResources

            ``` methodSignature
            public abstract boolean hasResources()
            ```

        []{#hasManifest()}

        -   #### hasManifest

            ``` methodSignature
            public abstract boolean hasManifest()
            ```

        []{#isRootModule()}

        -   #### isRootModule

            ``` methodSignature
            @Derived
            public boolean isRootModule()
            ```

        []{#getCanaryClassName()}

        -   #### getCanaryClassName

            ``` methodSignature
            @Derived
            public String getCanaryClassName()
            ```

        []{#compareTo(com.facebook.buck.android.apkmodule.APKModule)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(APKModule o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<APKModule>`
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
