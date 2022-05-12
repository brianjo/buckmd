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

-   [Overview](../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.jvm.java.abi.source {#package-com.facebook.buck.jvm.java.abi.source .title title="Package"}
:::

::: contentContainer
::: {.section role="region"}
[]{#package.description}

::: block
Enables generation of ABI jars using only the Java source code of a
single target, without requiring access to the source or ABI of
dependencies.

If the ABI of a dependency target is available, it will be used.
However, when one or more dependency ABIs are missing, certain language
constructs become ambiguous, and we have to make assumptions. Most of
those assumptions can be worked around with small changes to coding
style.

See `InterfaceValidator` for more information on the restrictions.
:::
:::

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [FileManagerSimulator](FileManag  | ::: block                         |
    | erSimulator.html "class in com.fa | Simulates the behavior of         |
    | cebook.buck.jvm.java.abi.source") | `javac`\'s file manager for       |
    |                                   | source-only ABI classpaths.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | FrontendOnlyJavacTask](FrontendOn | An implementation of `JavacTask`  |
    | lyJavacTask.html "class in com.fa | that implements only the frontend |
    | cebook.buck.jvm.java.abi.source") | portions of the task, using only  |
    |                                   | the parse phase of the underlying |
    |                                   | compiler and without requiring a  |
    |                                   | complete classpath.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FrontendOnlyJavacT               |                                   |
    | askProxyImpl](FrontendOnlyJavacTa |                                   |
    | skProxyImpl.html "class in com.fa |                                   |
    | cebook.buck.jvm.java.abi.source") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | StandalonePackageType](Standalone |                                   |
    | PackageType.html "class in com.fa |                                   |
    | cebook.buck.jvm.java.abi.source") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TreeBackedAnno                   | ::: block                         |
    | tatedConstruct](TreeBackedAnnotat | An implementation of              |
    | edConstruct.html "class in com.fa | [`AnnotatedCo                     |
    | cebook.buck.jvm.java.abi.source") | nstruct`](http://docs.oracle.com/ |
    |                                   | javase/7/docs/api/javax/lang/mode |
    |                                   | l/AnnotatedConstruct.html?is-exte |
    |                                   | rnal=true "class or interface in  |
    |                                   | javax.lang.model"){.externalLink} |
    |                                   | that uses only the information    |
    |                                   | available from a `Tree`.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TreeBackedAn                     | ::: block                         |
    | notationFactory](TreeBackedAnnota | Support for \@{link               |
    | tionFactory.html "class in com.fa | TreeBackedA                       |
    | cebook.buck.jvm.java.abi.source") | nnotatedConstruct#getAnnotation}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Va                               | ::: block                         |
    | lidatingTaskListener](ValidatingT | A `TaskListener` that is used     |
    | askListener.html "class in com.fa | during full compilation to        |
    | cebook.buck.jvm.java.abi.source") | validate the guesses made by      |
    |                                   | source-based ABI generation.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                          Description
      --------------------------------------------------------------------------------------------- -------------
      [CompletedTypeKind](CompletedTypeKind.html "enum in com.facebook.buck.jvm.java.abi.source")    

      : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
