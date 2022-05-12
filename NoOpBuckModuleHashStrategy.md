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
[Package]{.packageLabelInType} [com.facebook.buck.core.module.impl](package-summary.html)
:::

## Class NoOpBuckModuleHashStrategy {#class-noopbuckmodulehashstrategy .title title="Class NoOpBuckModuleHashStrategy"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.module.impl.NoOpBuckModuleHashStrategy

::: description
-   

    All Implemented Interfaces:
    :   `BuckModuleHashStrategy`

    ------------------------------------------------------------------------

        public class NoOpBuckModuleHashStrategy
        extends Object
        implements BuckModuleHashStrategy
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `NoOpBuckModuleHashStrategy()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                         Description
          ------------------- ---------------------------------------------- -------------
          `String`            `getModuleHash​(Class<?> cls)`                   
          `boolean`           `needToAddModuleHashToRuleKey​(Class<?> cls)`    

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

        []{#<init>()}

        -   #### NoOpBuckModuleHashStrategy

                public NoOpBuckModuleHashStrategy()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#needToAddModuleHashToRuleKey(java.lang.Class)}

        -   #### needToAddModuleHashToRuleKey

            ``` methodSignature
            public boolean needToAddModuleHashToRuleKey​(Class<?> cls)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `needToAddModuleHashToRuleKey` in
                interface `BuckModuleHashStrategy`

            [Returns:]{.returnLabel}
            :   `true` if the hash of a module that contains `cls`
                should be added to a rule key.

        []{#getModuleHash(java.lang.Class)}

        -   #### getModuleHash

            ``` methodSignature
            public String getModuleHash​(Class<?> cls)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getModuleHash` in interface `BuckModuleHashStrategy`

            [Returns:]{.returnLabel}
            :   the hash of a module that contains `cls`
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
