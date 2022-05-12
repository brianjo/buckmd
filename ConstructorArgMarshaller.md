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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Interface ConstructorArgMarshaller {#interface-constructorargmarshaller .title title="Interface ConstructorArgMarshaller"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultConstructorArgMarshaller`

    ------------------------------------------------------------------------

        public interface ConstructorArgMarshaller

    ::: block
    Used to derive information from the constructor args returned by
    [`DescriptionWithTargetGraph`](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")
    instances. There are two major uses this information is put to:
    populating the DTO object from the deserialized JSON maps, which are
    outputted by the functions added to Buck\'s core build file parsing
    script. The second function of this class is to generate those
    functions.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T exte              | `popu                 | ::: block             |
        | nds ConstructorArg>T` | late​(CellNameResolver | Creates a constructor |
        |                       |  cellNameResolver,    | argument using raw    |
        |                       |       ProjectFilesyst | attributes that may   |
        |                       | em filesystem,        | contain configurable  |
        |                       |   SelectorListResolve | attributes.           |
        |                       | r selectorListResolve | :::                   |
        |                       | r,         TargetConf |                       |
        |                       | igurationTransformer  |                       |
        |                       | targetConfigurationTr |                       |
        |                       | ansformer,         Se |                       |
        |                       | lectableConfiguration |                       |
        |                       | Context configuration |                       |
        |                       | Context,         Buil |                       |
        |                       | dTarget buildTarget,  |                       |
        |                       |         TargetConfigu |                       |
        |                       | ration hostConfigurat |                       |
        |                       | ion,         Dependen |                       |
        |                       | cyStack dependencySta |                       |
        |                       | ck,         DataTrans |                       |
        |                       | ferObjectDescriptor<T |                       |
        |                       | > constructorArgDescr |                       |
        |                       | iptor,         com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSet.Builder<B |                       |
        |                       | uildTarget> declaredD |                       |
        |                       | eps,         com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSet.Builder<Bui |                       |
        |                       | ldTarget> configurati |                       |
        |                       | onDeps,         Map<S |                       |
        |                       | tring,​?> attributes)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#populate(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.select.SelectorListResolver,com.facebook.buck.core.model.TargetConfigurationTransformer,com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.rules.coercer.DataTransferObjectDescriptor,com.google.common.collect.ImmutableSet.Builder,com.google.common.collect.ImmutableSet.Builder,java.util.Map)}

        -   #### populate

            ``` methodSignature
            <T extends ConstructorArg> T populate​(CellNameResolver cellNameResolver,
                                                  ProjectFilesystem filesystem,
                                                  SelectorListResolver selectorListResolver,
                                                  TargetConfigurationTransformer targetConfigurationTransformer,
                                                  SelectableConfigurationContext configurationContext,
                                                  BuildTarget buildTarget,
                                                  TargetConfiguration hostConfiguration,
                                                  DependencyStack dependencyStack,
                                                  DataTransferObjectDescriptor<T> constructorArgDescriptor,
                                                  com.google.common.collect.ImmutableSet.Builder<BuildTarget> declaredDeps,
                                                  com.google.common.collect.ImmutableSet.Builder<BuildTarget> configurationDeps,
                                                  Map<String,​?> attributes)
                                           throws CoerceFailedException
            ```

            ::: block
            Creates a constructor argument using raw attributes that may
            contain configurable attributes.
            Use the information contained in the `params` to fill in the
            public fields and settable properties of `dto`. The
            following rules are used:

            -   Boolean values are set to true or false.
            -   [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
                are resolved and will be fully qualified.
            -   Numeric values are handled as if being cast from Long.
            -   [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                instances will be set to the appropriate implementation.
            -   [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                declarations will be set to be relative to the project
                root.
            -   Strings will be set \"as is\".
            -   [`List`](http://docs.oracle.com/javase/7/docs/api/java/util/List.html?is-external=true "class or interface in java.util"){.externalLink}s
                and
                [`Set`](http://docs.oracle.com/javase/7/docs/api/java/util/Set.html?is-external=true "class or interface in java.util"){.externalLink}s
                will be populated with the expected generic type,
                provided the wildcarding allows an upperbound to be
                determined to be one of the above.

            Any property that is marked as being an
            [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
            field will be set to a default value if none is set. This is
            typically
            [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink},
            but in the case of collections is an empty collection.
            :::

            [Parameters:]{.paramLabel}
            :   `cellNameResolver` -
            :   `hostConfiguration` -
            :   `declaredDeps` - A builder to be populated with the
                declared dependencies.
            :   `attributes` - configured attributes that cannot contain
                selectable values (instances of
                [`SelectorList`](../../core/select/SelectorList.html "class in com.facebook.buck.core.select"))

            [Returns:]{.returnLabel}
            :   The fully populated DTO.

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::