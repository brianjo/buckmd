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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser](package-summary.html)
:::

## Class BuildTargetPatternToBuildPackagePathKey {#class-buildtargetpatterntobuildpackagepathkey .title title="Class BuildTargetPatternToBuildPackagePathKey"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.parser.BuildTargetPatternToBuildPackagePathKey

::: description
-   

    All Implemented Interfaces:
    :   `ComputeKey<BuildPackagePaths>`

    ------------------------------------------------------------------------

        public abstract class BuildTargetPatternToBuildPackagePathKey
        extends Object
        implements ComputeKey<BuildPackagePaths>

    ::: block
    Transformation key containing build target pattern for which to
    discover package paths
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                   Field          Description
          --------------------------------------------------- -------------- -------------
          `static ComputationIdentifier<BuildPackagePaths>`   `IDENTIFIER`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                   Description
          --------------------------------------------- -------------
          `BuildTargetPatternToBuildPackagePathKey()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ComputationIdentifie | `getIdentifier()`     |                       |
        | r<BuildPackagePaths>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `getPattern()`        | ::: block             |
        | t BuildTargetPattern` |                       | Pattern for which to  |
        |                       |                       | discover paths to     |
        |                       |                       | appropriate packages. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `of​(BuildTa           |                       |
        | c BuildTargetPatternT | rgetPattern pattern)` |                       |
        | oBuildPackagePathKey` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#field.detail}

        ### Field Detail

        []{#IDENTIFIER}

        -   #### IDENTIFIER

                public static final ComputationIdentifier<BuildPackagePaths> IDENTIFIER
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildTargetPatternToBuildPackagePathKey

                public BuildTargetPatternToBuildPackagePathKey()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPattern()}

        -   #### getPattern

            ``` methodSignature
            public abstract BuildTargetPattern getPattern()
            ```

            ::: block
            Pattern for which to discover paths to appropriate packages.
            Pattern can specify single target like //package:target or
            multiple targets like //package: or //package/\...
            :::

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<BuildPackagePaths> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `ComputeKey<BuildPackagePaths>`

            [Returns:]{.returnLabel}
            :   the identifier of this key. This identifier is used to
                map all keys of the same
                [`ComputationIdentifier`](../graph/transformation/model/ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                to the same
                [`GraphComputation`](../graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").

        []{#of(com.facebook.buck.core.parser.buildtargetpattern.BuildTargetPattern)}

        -   #### of

            ``` methodSignature
            public static BuildTargetPatternToBuildPackagePathKey of​(BuildTargetPattern pattern)
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
