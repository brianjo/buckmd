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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class XcodeScriptDescriptionArg.Builder {#class-xcodescriptdescriptionarg.builder .title title="Class XcodeScriptDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.XcodeScriptDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [XcodeScriptDescriptionArg](XcodeScriptDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class XcodeScriptDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`XcodeScriptDescriptionArg`](XcodeScriptDescriptionArg.html "class in com.facebook.buck.apple").
    Initialize attributes and then invoke the [`build()`](#build())
    method to create an immutable instance.
    *`Builder` is not thread-safe and generally should not be stored in
    a field or collection, but instead used immediately to create
    instances.*
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `XcodeScriptDe        | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compa               |
        |                       | ildTarget> elements)` | tibleWith`](XcodeScri |
        |                       |                       | ptDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addAll               | ::: block             |
        | scriptionArg.Builder` | InputFileLists​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`input               |
        |                       |                       | FileLists`](XcodeScri |
        |                       |                       | ptDescriptionArg.html |
        |                       |                       | #getInputFileLists()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addAllInputs​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`inputs`](X          |
        |                       |                       | codeScriptDescription |
        |                       |                       | Arg.html#getInputs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](X          |
        |                       |                       | codeScriptDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Xco      |
        |                       |                       | deScriptDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addAllO              | ::: block             |
        | scriptionArg.Builder` | utputFileLists​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`outputF             |
        |                       |                       | ileLists`](XcodeScrip |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getOutputFileLists()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addAllOutputs​(Iterab | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`outputs`](Xc        |
        |                       |                       | odeScriptDescriptionA |
        |                       |                       | rg.html#getOutputs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`srcs`]              |
        |                       |                       | (XcodeScriptDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compa               |
        |                       |                       | tibleWith`](XcodeScri |
        |                       |                       | ptDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compa               |
        |                       |                       | tibleWith`](XcodeScri |
        |                       |                       | ptDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addInputFileL        | ::: block             |
        | scriptionArg.Builder` | ists​(String element)` | Adds one element to   |
        |                       |                       | [`input               |
        |                       |                       | FileLists`](XcodeScri |
        |                       |                       | ptDescriptionArg.html |
        |                       |                       | #getInputFileLists()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addInputFileLists    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`input               |
        |                       |                       | FileLists`](XcodeScri |
        |                       |                       | ptDescriptionArg.html |
        |                       |                       | #getInputFileLists()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addIn                | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [`inputs`](X          |
        |                       |                       | codeScriptDescription |
        |                       |                       | Arg.html#getInputs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addInputs            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`inputs`](X          |
        |                       |                       | codeScriptDescription |
        |                       |                       | Arg.html#getInputs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](X          |
        |                       |                       | codeScriptDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](X          |
        |                       |                       | codeScriptDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Xco      |
        |                       |                       | deScriptDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Xco      |
        |                       |                       | deScriptDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addOutputFileL       | ::: block             |
        | scriptionArg.Builder` | ists​(String element)` | Adds one element to   |
        |                       |                       | [`outputF             |
        |                       |                       | ileLists`](XcodeScrip |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getOutputFileLists()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addOutputFileLists   | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`outputF             |
        |                       |                       | ileLists`](XcodeScrip |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getOutputFileLists()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addOut               | ::: block             |
        | scriptionArg.Builder` | puts​(String element)` | Adds one element to   |
        |                       |                       | [`outputs`](Xc        |
        |                       |                       | odeScriptDescriptionA |
        |                       |                       | rg.html#getOutputs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addOutputs           | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`outputs`](Xc        |
        |                       |                       | odeScriptDescriptionA |
        |                       |                       | rg.html#getOutputs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`srcs`]              |
        |                       |                       | (XcodeScriptDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`srcs`]              |
        |                       |                       | (XcodeScriptDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Xcode                | `build()`             | ::: block             |
        | ScriptDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`XcodeScript         |
        |                       |                       | DescriptionArg`](Xcod |
        |                       |                       | eScriptDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `from​(com.f           | ::: block             |
        | scriptionArg.Builder` | acebook.buck.apple.Ab | Copy abstract value   |
        |                       | stractXcodeScriptDesc | type                  |
        |                       | riptionArg instance)` | `AbstractXcode        |
        |                       |                       | ScriptDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `from​(XcodeScriptDesc | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Xcode                |
        |                       |                       | ScriptDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HasSrcs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.core.des |
        |                       |                       | cription.arg.HasSrcs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setCmd​(String cmd)`  | ::: block             |
        | scriptionArg.Builder` |                       | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`cmd`                |
        |                       |                       | ](XcodeScriptDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compa               |
        |                       |                       | tibleWith`](XcodeScri |
        |                       |                       | ptDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatfo |
        |                       |                       | rm`](XcodeScriptDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatfo |
        |                       | faultTargetPlatform)` | rm`](XcodeScriptDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | InputFileLists​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`input               |
        |                       |                       | FileLists`](XcodeScri |
        |                       |                       | ptDescriptionArg.html |
        |                       |                       | #getInputFileLists()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setInputs​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`inputs`](X          |
        |                       |                       | codeScriptDescription |
        |                       |                       | Arg.html#getInputs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](X          |
        |                       |                       | codeScriptDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Xco      |
        |                       |                       | deScriptDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`]              |
        |                       |                       | (XcodeScriptDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setO                 | ::: block             |
        | scriptionArg.Builder` | utputFileLists​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`outputF             |
        |                       |                       | ileLists`](XcodeScrip |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getOutputFileLists()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setOutputs​(Iterab    | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`outputs`](Xc        |
        |                       |                       | odeScriptDescriptionA |
        |                       |                       | rg.html#getOutputs()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeScriptDe        | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`srcs`]              |
        |                       |                       | (XcodeScriptDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | sortedSet.            |
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
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.apple.XcodeScriptDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder from​(XcodeScriptDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `XcodeScriptDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AbstractXcodeScriptDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder from​(com.facebook.buck.apple.AbstractXcodeScriptDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractXcodeScriptDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder from​(BuildRuleArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.BuildRuleArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasSrcs)}

        -   #### from

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder from​(HasSrcs instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasSrcs` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder from​(ConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.ConstructorArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addInputs(java.lang.String)}

        -   #### addInputs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addInputs​(String element)
            ```

            ::: block
            Adds one element to
            [`inputs`](XcodeScriptDescriptionArg.html#getInputs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A inputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addInputs(java.lang.String...)}

        -   #### addInputs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addInputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`inputs`](XcodeScriptDescriptionArg.html#getInputs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of inputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInputs(java.lang.Iterable)}

        -   #### setInputs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setInputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`inputs`](XcodeScriptDescriptionArg.html#getInputs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of inputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllInputs(java.lang.Iterable)}

        -   #### addAllInputs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addAllInputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`inputs`](XcodeScriptDescriptionArg.html#getInputs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of inputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addInputFileLists(java.lang.String)}

        -   #### addInputFileLists

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addInputFileLists​(String element)
            ```

            ::: block
            Adds one element to
            [`inputFileLists`](XcodeScriptDescriptionArg.html#getInputFileLists())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A inputFileLists element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addInputFileLists(java.lang.String...)}

        -   #### addInputFileLists

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addInputFileLists​(String... elements)
            ```

            ::: block
            Adds elements to
            [`inputFileLists`](XcodeScriptDescriptionArg.html#getInputFileLists())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of inputFileLists elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInputFileLists(java.lang.Iterable)}

        -   #### setInputFileLists

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setInputFileLists​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`inputFileLists`](XcodeScriptDescriptionArg.html#getInputFileLists())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of inputFileLists elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllInputFileLists(java.lang.Iterable)}

        -   #### addAllInputFileLists

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addAllInputFileLists​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`inputFileLists`](XcodeScriptDescriptionArg.html#getInputFileLists())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of inputFileLists elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addOutputs(java.lang.String)}

        -   #### addOutputs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addOutputs​(String element)
            ```

            ::: block
            Adds one element to
            [`outputs`](XcodeScriptDescriptionArg.html#getOutputs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A outputs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addOutputs(java.lang.String...)}

        -   #### addOutputs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addOutputs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`outputs`](XcodeScriptDescriptionArg.html#getOutputs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of outputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOutputs(java.lang.Iterable)}

        -   #### setOutputs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setOutputs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`outputs`](XcodeScriptDescriptionArg.html#getOutputs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of outputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllOutputs(java.lang.Iterable)}

        -   #### addAllOutputs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addAllOutputs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`outputs`](XcodeScriptDescriptionArg.html#getOutputs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of outputs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addOutputFileLists(java.lang.String)}

        -   #### addOutputFileLists

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addOutputFileLists​(String element)
            ```

            ::: block
            Adds one element to
            [`outputFileLists`](XcodeScriptDescriptionArg.html#getOutputFileLists())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A outputFileLists element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addOutputFileLists(java.lang.String...)}

        -   #### addOutputFileLists

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addOutputFileLists​(String... elements)
            ```

            ::: block
            Adds elements to
            [`outputFileLists`](XcodeScriptDescriptionArg.html#getOutputFileLists())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of outputFileLists elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOutputFileLists(java.lang.Iterable)}

        -   #### setOutputFileLists

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setOutputFileLists​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`outputFileLists`](XcodeScriptDescriptionArg.html#getOutputFileLists())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of outputFileLists elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllOutputFileLists(java.lang.Iterable)}

        -   #### addAllOutputFileLists

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addAllOutputFileLists​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`outputFileLists`](XcodeScriptDescriptionArg.html#getOutputFileLists())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of outputFileLists elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmd(java.lang.String)}

        -   #### setCmd

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setCmd​(String cmd)
            ```

            ::: block
            Initializes the value for the
            [`cmd`](XcodeScriptDescriptionArg.html#getCmd()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](XcodeScriptDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](XcodeScriptDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](XcodeScriptDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](XcodeScriptDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](XcodeScriptDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](XcodeScriptDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](XcodeScriptDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](XcodeScriptDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](XcodeScriptDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultTargetPlatform(java.util.Optional)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](XcodeScriptDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](XcodeScriptDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](XcodeScriptDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](XcodeScriptDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](XcodeScriptDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](XcodeScriptDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addSrcs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](XcodeScriptDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](XcodeScriptDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](XcodeScriptDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final XcodeScriptDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](XcodeScriptDescriptionArg.html#getSrcs())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public XcodeScriptDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`XcodeScriptDescriptionArg`](XcodeScriptDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of XcodeScriptDescriptionArg

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if any required attributes are
                missing
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
