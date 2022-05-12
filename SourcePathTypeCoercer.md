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

## Class SourcePathTypeCoercer {#class-sourcepathtypecoercer .title title="Class SourcePathTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.LeafTypeNewCoercer](LeafTypeNewCoercer.html "class in com.facebook.buck.rules.coercer")\<[UnconfiguredSourcePath](../../core/sourcepath/UnconfiguredSourcePath.html "class in com.facebook.buck.core.sourcepath"),​[SourcePath](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")\>

    -   -   com.facebook.buck.rules.coercer.SourcePathTypeCoercer

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<SourcePath>`,
        `TypeCoercer<UnconfiguredSourcePath,​SourcePath>`

    ------------------------------------------------------------------------

        public class SourcePathTypeCoercer
        extends LeafTypeNewCoercer<UnconfiguredSourcePath,​SourcePath>

    ::: block
    Coerce to
    [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath").
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

          Constructor                                                                                                                                                                                      Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `SourcePathTypeCoercer​(TypeCoercer<UnconfiguredBuildTargetWithOutputs,​BuildTargetWithOutputs> buildTargetWithOutputsTypeCoercer,                      TypeCoercer<Path,​Path> pathTypeCoercer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `SourcePath`          | `c                    |                       |
        |                       | oerce​(CellNameResolve |                       |
        |                       | r cellRoots,       Pr |                       |
        |                       | ojectFilesystem files |                       |
        |                       | ystem,       ForwardR |                       |
        |                       | elativePath pathRelat |                       |
        |                       | iveToProjectRoot,     |                       |
        |                       |    TargetConfiguratio |                       |
        |                       | n targetConfiguration |                       |
        |                       | ,       TargetConfigu |                       |
        |                       | ration hostConfigurat |                       |
        |                       | ion,       Unconfigur |                       |
        |                       | edSourcePath object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Un                   | `coerceToUnco         | ::: block             |
        | configuredSourcePath` | nfigured​(CellNameReso | Coerce to a value for |
        |                       | lver cellRoots,       | unconfigured graph.   |
        |                       |                Projec | :::                   |
        |                       | tFilesystem filesyste |                       |
        |                       | m,                    |                       |
        |                       |   ForwardRelativePath |                       |
        |                       |  pathRelativeToProjec |                       |
        |                       | tRoot,                |                       |
        |                       |       Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getOutputType()`     |                       |
        | ogle.common.reflect.T |                       |                       |
        | ypeToken<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `g                    |                       |
        | reflect.TypeToken<Unc | etUnconfiguredType()` |                       |
        | onfiguredSourcePath>` |                       |                       |
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

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercer,com.facebook.buck.rules.coercer.TypeCoercer)}

        -   #### SourcePathTypeCoercer

                public SourcePathTypeCoercer​(TypeCoercer<UnconfiguredBuildTargetWithOutputs,​BuildTargetWithOutputs> buildTargetWithOutputsTypeCoercer,
                                             TypeCoercer<Path,​Path> pathTypeCoercer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<SourcePath> getOutputType()
            ```

        []{#getUnconfiguredType()}

        -   #### getUnconfiguredType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<UnconfiguredSourcePath> getUnconfiguredType()
            ```

        []{#coerceToUnconfigured(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,java.lang.Object)}

        -   #### coerceToUnconfigured

            ``` methodSignature
            public UnconfiguredSourcePath coerceToUnconfigured​(CellNameResolver cellRoots,
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

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.sourcepath.UnconfiguredSourcePath)}

        -   #### coerce

            ``` methodSignature
            public SourcePath coerce​(CellNameResolver cellRoots,
                                     ProjectFilesystem filesystem,
                                     ForwardRelativePath pathRelativeToProjectRoot,
                                     TargetConfiguration targetConfiguration,
                                     TargetConfiguration hostConfiguration,
                                     UnconfiguredSourcePath object)
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
