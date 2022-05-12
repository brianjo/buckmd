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

## Class LeafUnconfiguredOnlyCoercer\<T\> {#class-leafunconfiguredonlycoercert .title title="Class LeafUnconfiguredOnlyCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.LeafTypeNewCoercer](LeafTypeNewCoercer.html "class in com.facebook.buck.rules.coercer")\<T,​T\>

    -   -   com.facebook.buck.rules.coercer.LeafUnconfiguredOnlyCoercer\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<T>`, `TypeCoercer<T,​T>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ConstraintTypeCoercer`, `EnumTypeCoercer`, `FlavorTypeCoercer`,
        `IdentityTypeCoercer`, `LogLevelTypeCoercer`,
        `NumberTypeCoercer`, `PathTypeCoercer`, `PatternTypeCoercer`,
        `UnconfiguredBuildTargetTypeCoercer`,
        `UnconfiguredBuildTargetWithOutputsTypeCoercer`

    ------------------------------------------------------------------------

        public abstract class LeafUnconfiguredOnlyCoercer<T>
        extends LeafTypeNewCoercer<T,​T>

    ::: block
    Second phase coercion is identity.
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

          Constructor                       Description
          --------------------------------- -------------
          `LeafUnconfiguredOnlyCoercer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `T`                   | `c                    |                       |
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
        |                       | ion,       T object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getOutputType()`     |                       |
        | reflect.TypeToken<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `unc                  | ::: block             |
        |                       | onfiguredToConfigured | [`TypeCoercer.        |
        |                       | CoercionIsIdentity()` | coerce(CellNameResolv |
        |                       |                       | er, ProjectFilesystem |
        |                       |                       | , ForwardRelativePath |
        |                       |                       | , TargetConfiguration |
        |                       |                       | ,  TargetConfiguratio |
        |                       |                       | n, Object)`](TypeCoer |
        |                       |                       | cer.html#coerce(com.f |
        |                       |                       | acebook.buck.core.cel |
        |                       |                       | l.nameresolver.CellNa |
        |                       |                       | meResolver,com.facebo |
        |                       |                       | ok.buck.io.filesystem |
        |                       |                       | .ProjectFilesystem,co |
        |                       |                       | m.facebook.buck.core. |
        |                       |                       | path.ForwardRelativeP |
        |                       |                       | ath,com.facebook.buck |
        |                       |                       | .core.model.TargetCon |
        |                       |                       | figuration,com.facebo |
        |                       |                       | ok.buck.core.model.Ta |
        |                       |                       | rgetConfiguration,U)) |
        |                       |                       | must be no-op when    |
        |                       |                       | this returns `true`.  |
        |                       |                       | :::                   |
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

            `checkOutputAssignableTo, checkUnconfiguredAssignableTo, coerceBoth, coerceToUnconfigured, concat, getUnconfiguredType, supportsConcatenation`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LeafUnconfiguredOnlyCoercer

                public LeafUnconfiguredOnlyCoercer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#unconfiguredToConfiguredCoercionIsIdentity()}

        -   #### unconfiguredToConfiguredCoercionIsIdentity

            ``` methodSignature
            public final boolean unconfiguredToConfiguredCoercionIsIdentity()
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercer`]{.descfrmTypeLabel}
            :::

            ::: block
            [`TypeCoercer.coerce(CellNameResolver, ProjectFilesystem, ForwardRelativePath, TargetConfiguration,  TargetConfiguration, Object)`](TypeCoercer.html#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,U))
            must be no-op when this returns `true`.
            :::

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public final com.google.common.reflect.TypeToken<T> getOutputType()
            ```

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object)}
        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,T)}

        -   #### coerce

            ``` methodSignature
            public final T coerce​(CellNameResolver cellRoots,
                                  ProjectFilesystem filesystem,
                                  ForwardRelativePath pathRelativeToProjectRoot,
                                  TargetConfiguration targetConfiguration,
                                  TargetConfiguration hostConfiguration,
                                  T object)
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
