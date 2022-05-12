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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.attr](package-summary.html)
:::

## Interface InitializableFromDisk\<T\> {#interface-initializablefromdiskt .title title="Interface InitializableFromDisk"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AndroidLibrary`, `AndroidPrebuiltAar`, `AndroidResource`,
        `CalculateClassAbi`, `CalculateSourceAbi`,
        `CalculateSourceAbiFromLibraryTarget`, `CompareAbis`,
        `DefaultJavaLibrary`, `DefaultWorkerToolRule`,
        `DexProducedFromJavaLibrary`, `DummyRDotJava`, `PrebuiltJar`,
        `PreDexSplitDexGroup`, `ResourcesFilter`, `UnzipAar`

    ------------------------------------------------------------------------

        public interface InitializableFromDisk<T>

    ::: block
    Object that has in-memory data structures that need to be populated
    as a result of executing its steps. An object that implements this
    interface will *always* have its internal data structures
    initialized through this interface, regardless of whether it was
    built locally or read from cache. This ensures that a rule is always
    in the same state once `isRuleBuilt()` returns `true`.
    Objects that implement this interface should create getter methods
    that delegate to
    [`BuildOutputInitializer.getBuildOutput()`](BuildOutputInitializer.html#getBuildOutput())
    to access the in-memory data structures rather than have clients
    invoke
    [`BuildOutputInitializer.getBuildOutput()`](BuildOutputInitializer.html#getBuildOutput())
    directly. This ensures that all getters go through any protections
    provided by
    [`BuildOutputInitializer.getBuildOutput()`](BuildOutputInitializer.html#getBuildOutput()).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                         Description
          ----------------------------- -------------------------------------------------------------- -------------
          `BuildOutputInitializer<T>`   `getBuildOutputInitializer()`                                   
          `T`                           `initializeFromDisk​(SourcePathResolverAdapter pathResolver)`    
          `default void`                `invalidateInitializeFromDiskState()`                           

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            T initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                          throws IOException
            ```

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            BuildOutputInitializer<T> getBuildOutputInitializer()
            ```

        []{#invalidateInitializeFromDiskState()}

        -   #### invalidateInitializeFromDiskState

            ``` methodSignature
            default void invalidateInitializeFromDiskState()
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
