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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class NoopRuleKeyScopedHasher {#class-nooprulekeyscopedhasher .title title="Class NoopRuleKeyScopedHasher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.NoopRuleKeyScopedHasher

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyScopedHasher`

    ------------------------------------------------------------------------

        public class NoopRuleKeyScopedHasher
        extends Object
        implements RuleKeyScopedHasher

    ::: block
    Does nothing.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.keys.RuleKeyScopedHasher}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.keys.[RuleKeyScopedHasher](RuleKeyScopedHasher.html "interface in com.facebook.buck.rules.keys")

            `RuleKeyScopedHasher.ContainerScope`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                  Field        Description
          ---------------------------------- ------------ -------------
          `static NoopRuleKeyScopedHasher`   `INSTANCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                Description
          -------------------------------------- ----------------------------------------------------- -------------
          `RuleKeyScopedHasher.ContainerScope`   `containerScope​(RuleKeyHasher.Container container)`    
          `Scope`                                `keyScope​(String key)`                                 
          `Scope`                                `pathKeyScope​(Path key)`                               
          `Scope`                                `wrapperScope​(RuleKeyHasher.Wrapper wrapper)`          

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

        []{#INSTANCE}

        -   #### INSTANCE

                public static final NoopRuleKeyScopedHasher INSTANCE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#keyScope(java.lang.String)}

        -   #### keyScope

            ``` methodSignature
            public Scope keyScope​(String key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `keyScope` in interface `RuleKeyScopedHasher`

        []{#pathKeyScope(java.nio.file.Path)}

        -   #### pathKeyScope

            ``` methodSignature
            public Scope pathKeyScope​(Path key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `pathKeyScope` in interface `RuleKeyScopedHasher`

        []{#wrapperScope(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### wrapperScope

            ``` methodSignature
            public Scope wrapperScope​(RuleKeyHasher.Wrapper wrapper)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `wrapperScope` in interface `RuleKeyScopedHasher`

        []{#containerScope(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container)}

        -   #### containerScope

            ``` methodSignature
            public RuleKeyScopedHasher.ContainerScope containerScope​(RuleKeyHasher.Container container)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `containerScope` in interface `RuleKeyScopedHasher`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
