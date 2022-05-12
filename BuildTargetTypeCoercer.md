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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class BuildTargetTypeCoercer {#class-buildtargettypecoercer .title title="Class BuildTargetTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.LeafTypeNewCoercer](LeafTypeNewCoercer.html "class in com.facebook.buck.rules.coercer")\<[UnconfiguredBuildTarget](../../core/model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model"),​[BuildTarget](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")\>

    -   -   com.facebook.buck.rules.coercer.BuildTargetTypeCoercer

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<BuildTarget>`,
        `TypeCoercer<UnconfiguredBuildTarget,​BuildTarget>`

    ------------------------------------------------------------------------

        public class BuildTargetTypeCoercer
        extends LeafTypeNewCoercer<UnconfiguredBuildTarget,​BuildTarget>

    ::: block
    Coerce to
    [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.coercer.TypeCoercer}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")

            `TypeCoercer.Traversal`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildTargetTypeCoercer​(TypeCoercer<UnconfiguredBuildTarget,​UnconfiguredBuildTarget> unconfiguredBuildTargetTypeCoercer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildTarget`         | `co                   |                       |
        |                       | erce​(CellNameResolver |                       |
        |                       |  cellRoots,       Pro |                       |
        |                       | jectFilesystem alsoUn |                       |
        |                       | used,       ForwardRe |                       |
        |                       | lativePath pathRelati |                       |
        |                       | veToProjectRoot,      |                       |
        |                       |   TargetConfiguration |                       |
        |                       |  targetConfiguration, |                       |
        |                       |        TargetConfigur |                       |
        |                       | ation hostConfigurati |                       |
        |                       | on,       Unconfigure |                       |
        |                       | dBuildTarget object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `coerceToUnco         | ::: block             |
        | onfiguredBuildTarget` | nfigured​(CellNameReso | Coerce to a value for |
        |                       | lver cellRoots,       | unconfigured graph.   |
        |                       |                Projec | :::                   |
        |                       | tFilesystem filesyste |                       |
        |                       | m,                    |                       |
        |                       |   ForwardRelativePath |                       |
        |                       |  pathRelativeToProjec |                       |
        |                       | tRoot,                |                       |
        |                       |       Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `getOutputType()`     |                       |
        | gle.common.reflect.Ty |                       |                       |
        | peToken<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.r  | `g                    |                       |
        | eflect.TypeToken<Unco | etUnconfiguredType()` |                       |
        | nfiguredBuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.LeafTypeNewCoercer}

            ### Methods inherited from class com.facebook.buck.rules.coercer.[LeafTypeNewCoercer](LeafTypeNewCoercer.html "class in com.facebook.buck.rules.coercer")

            `hasElementClass, traverse`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.TypeCoercer}

            ### Methods inherited from interface com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, concat, supportsConcatenation, unconfiguredToConfiguredCoercionIsIdentity`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercer)}

        -   #### BuildTargetTypeCoercer

                public BuildTargetTypeCoercer​(TypeCoercer<UnconfiguredBuildTarget,​UnconfiguredBuildTarget> unconfiguredBuildTargetTypeCoercer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<BuildTarget> getOutputType()
            ```

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<UnconfiguredBuildTarget> getUnconfiguredType()
            ```

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public UnconfiguredBuildTarget coerceToUnconfigured​(CellNameResolver cellRoots,
                                                                ProjectFilesystem filesystem,
                                                                ForwardRelativePath pathRelativeToProjectRoot,
                                                                Object object)
                                                         throws CoerceFailedException
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            Coerce to a value for unconfigured graph.
            :::

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### coerce

            ``` methodSignature
            public BuildTarget coerce​(CellNameResolver cellRoots,
                                      ProjectFilesystem alsoUnused,
                                      ForwardRelativePath pathRelativeToProjectRoot,
                                      TargetConfiguration targetConfiguration,
                                      TargetConfiguration hostConfiguration,
                                      UnconfiguredBuildTarget object)
                               throws CoerceFailedException
            ```

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - Input object cannot be coerced
                into the given type.
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