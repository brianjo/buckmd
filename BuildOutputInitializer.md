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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.attr](package-summary.html)
:::

## Class BuildOutputInitializer\<T\> {#class-buildoutputinitializert .title title="Class BuildOutputInitializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.attr.BuildOutputInitializer\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public final class BuildOutputInitializer<T>
        extends Object

    ::: block
    Delegates the actual reading of disk-cached data to the
    [`InitializableFromDisk`](InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")
    and is responsible for safely storing and retrieving the in-memory
    data structures.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                               Description
          ------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildOutputInitializer​(BuildTarget buildTarget,                       InitializableFromDisk<T> initializableFromDisk)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `T`                   | `getBuildOutput()`    | ::: block             |
        |                       |                       | The initialized       |
        |                       |                       | buildOutput.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `initializeFromDis    | ::: block             |
        |                       | k​(SourcePathResolverA | Initializes the build |
        |                       | dapter pathResolver)` | output from the on    |
        |                       |                       | disk state.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidate()`        | ::: block             |
        |                       |                       | Invalidates the       |
        |                       |                       | cached build output.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setBuildOutputFor    | ::: block             |
        |                       | Tests​(T buildOutput)` | This should be        |
        |                       |                       | invoked only by the   |
        |                       |                       | build engine          |
        |                       |                       | (currently,           |
        |                       |                       | [`CachingBuildEngin   |
        |                       |                       | e`](../../build/engin |
        |                       |                       | e/impl/CachingBuildEn |
        |                       |                       | gine.html "class in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .build.engine.impl")) |
        |                       |                       | that invoked          |
        |                       |                       | [`initializeFro       |
        |                       |                       | mDisk(SourcePathResol |
        |                       |                       | verAdapter)`](#initia |
        |                       |                       | lizeFromDisk(com.face |
        |                       |                       | book.buck.core.source |
        |                       |                       | path.resolver.SourceP |
        |                       |                       | athResolverAdapter)). |
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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.attr.InitializableFromDisk)}

        -   #### BuildOutputInitializer

                public BuildOutputInitializer​(BuildTarget buildTarget,
                                              InitializableFromDisk<T> initializableFromDisk)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#invalidate()}

        -   #### invalidate

            ``` methodSignature
            public void invalidate()
            ```

            ::: block
            Invalidates the cached build output. This should be called
            whenever the on disk state is about to change.
            :::

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public void initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                                    throws IOException
            ```

            ::: block
            Initializes the build output from the on disk state.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setBuildOutputForTests(java.lang.Object)}
        []{#setBuildOutputForTests(T)}

        -   #### setBuildOutputForTests

            ``` methodSignature
            public void setBuildOutputForTests​(T buildOutput)
                                        throws IllegalStateException
            ```

            ::: block
            This should be invoked only by the build engine (currently,
            [`CachingBuildEngine`](../../build/engine/impl/CachingBuildEngine.html "class in com.facebook.buck.core.build.engine.impl"))
            that invoked
            [`initializeFromDisk(SourcePathResolverAdapter)`](#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)).
            :::

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if this method has already
                been invoked.

        []{#getBuildOutput()}

        -   #### getBuildOutput

            ``` methodSignature
            public T getBuildOutput()
                             throws IllegalStateException
            ```

            ::: block
            The initialized buildOutput.
            :::

            [Throws:]{.throwsLabel}
            :   `IllegalStateException`
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
