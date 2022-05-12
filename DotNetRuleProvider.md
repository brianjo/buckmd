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
[Package]{.packageLabelInType} [com.facebook.buck.features.dotnet](package-summary.html)
:::

## Class DotNetRuleProvider {#class-dotnetruleprovider .title title="Class DotNetRuleProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.dotnet.DotNetRuleProvider

::: description
-   

    All Implemented Interfaces:
    :   `BuiltInProviderProvider`, `DescriptionProvider`,
        `org.pf4j.ExtensionPoint`

    ------------------------------------------------------------------------

        @Extension
        public class DotNetRuleProvider
        extends Object
        implements DescriptionProvider, BuiltInProviderProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `DotNetRuleProvider()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Collection           | `g                    | ::: block             |
        | <BuiltInProvider<?>>` | etBuiltInProviders()` | Providers to expose   |
        |                       |                       | to users              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Collec               | `getDescrip           |                       |
        | tion<Description<?>>` | tions​(DescriptionCrea |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### DotNetRuleProvider

                public DotNetRuleProvider()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDescriptions(com.facebook.buck.core.description.DescriptionCreationContext)}

        -   #### getDescriptions

            ``` methodSignature
            public Collection<Description<?>> getDescriptions​(DescriptionCreationContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescriptions` in interface `DescriptionProvider`

        []{#getBuiltInProviders()}

        -   #### getBuiltInProviders

            ``` methodSignature
            public Collection<BuiltInProvider<?>> getBuiltInProviders()
            ```

            ::: block
            [Description copied from
            interface: `BuiltInProviderProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Providers to expose to users
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuiltInProviders` in
                interface `BuiltInProviderProvider`
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
