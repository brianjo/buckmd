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

## Class CxxLinkGroupMappingTargetTraversalCoercer {#class-cxxlinkgroupmappingtargettraversalcoercer .title title="Class CxxLinkGroupMappingTargetTraversalCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.coercer.LeafTypeCoercer](LeafTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<[CxxLinkGroupMappingTarget.Traversal](../../core/linkgroup/CxxLinkGroupMappingTarget.Traversal.html "enum in com.facebook.buck.core.linkgroup")\>

    -   -   com.facebook.buck.rules.coercer.CxxLinkGroupMappingTargetTraversalCoercer

::: description
-   

    All Implemented Interfaces:
    :   `Concatable<CxxLinkGroupMappingTarget.Traversal>`,
        `TypeCoercer<Object,​CxxLinkGroupMappingTarget.Traversal>`

    ------------------------------------------------------------------------

        public class CxxLinkGroupMappingTargetTraversalCoercer
        extends LeafTypeCoercer<CxxLinkGroupMappingTarget.Traversal>

    ::: block
    [`TypeCoercer`](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")
    for
    [`CxxLinkGroupMappingTarget.Traversal`](../../core/linkgroup/CxxLinkGroupMappingTarget.Traversal.html "enum in com.facebook.buck.core.linkgroup").
    This
    [`TypeCoercer`](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")
    is used to convert the traversal of a link group mapping (e.g.,
    `(..., "tree")`) to a
    [`CxxLinkGroupMappingTarget.Traversal`](../../core/linkgroup/CxxLinkGroupMappingTarget.Traversal.html "enum in com.facebook.buck.core.linkgroup").
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

          Constructor                                     Description
          ----------------------------------------------- -------------
          `CxxLinkGroupMappingTargetTraversalCoercer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                            Method                                                                                                                                                                                                                                           Description
          ---------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CxxLinkGroupMappingTarget.Traversal`                                        `coerce​(CellNameResolver cellRoots,       ProjectFilesystem alsoUnused,       ForwardRelativePath pathRelativeToProjectRoot,       TargetConfiguration targetConfiguration,       TargetConfiguration hostConfiguration,       Object object)`    
          `com.google.common.reflect.TypeToken<CxxLinkGroupMappingTarget.Traversal>`   `getOutputType()`                                                                                                                                                                                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.coercer.LeafTypeCoercer}

            ### Methods inherited from class com.facebook.buck.rules.coercer.[LeafTypeCoercer](LeafTypeCoercer.html "class in com.facebook.buck.rules.coercer")

            `coerceToUnconfigured, getUnconfiguredType, hasElementClass, traverse`

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

        []{#<init>()}

        -   #### CxxLinkGroupMappingTargetTraversalCoercer

                public CxxLinkGroupMappingTargetTraversalCoercer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputType()}

        -   #### getOutputType

            ``` methodSignature
            public com.google.common.reflect.TypeToken<CxxLinkGroupMappingTarget.Traversal> getOutputType()
            ```

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object)}

        -   #### coerce

            ``` methodSignature
            public CxxLinkGroupMappingTarget.Traversal coerce​(CellNameResolver cellRoots,
                                                              ProjectFilesystem alsoUnused,
                                                              ForwardRelativePath pathRelativeToProjectRoot,
                                                              TargetConfiguration targetConfiguration,
                                                              TargetConfiguration hostConfiguration,
                                                              Object object)
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
