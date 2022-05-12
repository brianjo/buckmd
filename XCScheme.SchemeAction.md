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
[Package]{.packageLabelInType} [com.facebook.buck.apple.xcode](package-summary.html)
:::

## Class XCScheme.SchemeAction {#class-xcscheme.schemeaction .title title="Class XCScheme.SchemeAction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.xcode.XCScheme.SchemeAction

::: description
-   

    Direct Known Subclasses:
    :   `XCScheme.AnalyzeAction`, `XCScheme.ArchiveAction`,
        `XCScheme.BuildAction`, `XCScheme.LaunchAction`,
        `XCScheme.ProfileAction`, `XCScheme.TestAction`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [XCScheme](XCScheme.html "class in com.facebook.buck.apple.xcode")

    ------------------------------------------------------------------------

        public abstract static class XCScheme.SchemeAction
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `SchemeAction​(Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> preActions,             Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> postActions)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                   Method               Description
          ----------------------------------------------------------------------------------- -------------------- -------------
          `Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>>`   `getPostActions()`    
          `Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>>`   `getPreActions()`     

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

        []{#<init>(java.util.Optional,java.util.Optional)}

        -   #### SchemeAction

                public SchemeAction​(Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> preActions,
                                    Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> postActions)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPreActions()}

        -   #### getPreActions

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> getPreActions()
            ```

        []{#getPostActions()}

        -   #### getPostActions

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> getPostActions()
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
