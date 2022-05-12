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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.impl](package-summary.html)
:::

## Class MultiPlatformTargetConfigurationTransformer {#class-multiplatformtargetconfigurationtransformer .title title="Class MultiPlatformTargetConfigurationTransformer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.impl.MultiPlatformTargetConfigurationTransformer

::: description
-   

    All Implemented Interfaces:
    :   `TargetConfigurationTransformer`

    ------------------------------------------------------------------------

        public class MultiPlatformTargetConfigurationTransformer
        extends Object
        implements TargetConfigurationTransformer

    ::: block
    [`TargetConfigurationTransformer`](../TargetConfigurationTransformer.html "interface in com.facebook.buck.core.model")
    that transforms a single target configuration with a multiplatform
    as a target platform to multiple target configurations each
    containing platforms that are forming multiplatform.
    For example, a multiplatform \"A\" contains \"B\" as a base platform
    and \"X\", \"Y\", \"Z\" as nested platforms. In this case a target
    configuration with the \"A\" platform will be transformed to a set
    of platforms: \"A\", \"X\", \"Y\", \"Z\". Note that this
    transformation doesn\'t use \"B\" since the multiplatform uses its
    base platform to match constraints. Using the multiplatform instead
    of the base platform allows us to keep the rest of attributes (that
    don\'t use transformations) consistent with attributes that use
    transformations.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                    Description
          ---------------------------------------------------------------------------------------------- -------------
          `MultiPlatformTargetConfigurationTransformer​(TargetPlatformResolver targetPlatformResolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `needsTra             |                       |
        |                       | nsformation​(TargetCon |                       |
        |                       | figuration targetConf |                       |
        |                       | iguration,            |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `transform            | ::: block             |
        | ollect.ImmutableList< | ​(TargetConfiguration  | Transforms a single   |
        | TargetConfiguration>` | targetConfiguration,  | target configurations |
        |                       |          DependencySt | into multiple target  |
        |                       | ack dependencyStack)` | configurations.       |
        |                       |                       | :::                   |
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

        []{#<init>(com.facebook.buck.core.model.platform.TargetPlatformResolver)}

        -   #### MultiPlatformTargetConfigurationTransformer

                public MultiPlatformTargetConfigurationTransformer​(TargetPlatformResolver targetPlatformResolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#transform(com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### transform

            ``` methodSignature
            public com.google.common.collect.ImmutableList<TargetConfiguration> transform​(TargetConfiguration targetConfiguration,
                                                                                          DependencyStack dependencyStack)
            ```

            ::: block
            [Description copied from
            interface: `TargetConfigurationTransformer`]{.descfrmTypeLabel}
            :::

            ::: block
            Transforms a single target configurations into multiple
            target configurations.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `TargetConfigurationTransformer`

        []{#needsTransformation(com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### needsTransformation

            ``` methodSignature
            public boolean needsTransformation​(TargetConfiguration targetConfiguration,
                                               DependencyStack dependencyStack)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `needsTransformation` in
                interface `TargetConfigurationTransformer`

            [Returns:]{.returnLabel}
            :   `true` is the given target configuration can be
                transformed into other configurations.
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
