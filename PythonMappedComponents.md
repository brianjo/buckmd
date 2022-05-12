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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonMappedComponents {#class-pythonmappedcomponents .title title="Class PythonMappedComponents"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonMappedComponents

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `PythonComponents`

    ------------------------------------------------------------------------

        public abstract class PythonMappedComponents
        extends Object
        implements PythonComponents

    ::: block
    An implementation of
    [`PythonComponents`](PythonComponents.html "interface in com.facebook.buck.features.python")
    wrapping a fixed map of sources, where the keys determine where in
    the Python package the sources get added.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `PythonMappe          | ::: block             |
        |                       | dComponents.Resolved` | An implementation of  |
        |                       |                       | [`Pyt                 |
        |                       |                       | honComponents.Resolve |
        |                       |                       | d`](PythonComponents. |
        |                       |                       | Resolved.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.features.python") |
        |                       |                       | for                   |
        |                       |                       | [`PythonMappedCo      |
        |                       |                       | mponents`](PythonMapp |
        |                       |                       | edComponents.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.features.python") |
        |                       |                       | with                  |
        |                       |                       | [`SourcePath`](../.   |
        |                       |                       | ./core/sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath")s |
        |                       |                       | resolved to           |
        |                       |                       | [`Path`](http://doc   |
        |                       |                       | s.oracle.com/javase/7 |
        |                       |                       | /docs/api/java/nio/fi |
        |                       |                       | le/Path.html?is-exter |
        |                       |                       | nal=true "class or in |
        |                       |                       | terface in java.nio.f |
        |                       |                       | ile"){.externalLink}s |
        |                       |                       | for use with          |
        |                       |                       | [`Step                |
        |                       |                       | `](../../step/Step.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.step"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `PythonMappedComponents()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Symlinks`            | `asSymlinks()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | forEachInput​(java.uti | Run `consumer` on all |
        |                       | l.function.Consumer<S | [`SourcePath`](../.   |
        |                       | ourcePath> consumer)` | ./core/sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath")s |
        |                       |                       | contained in this     |
        |                       |                       | object.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getComponents()`     |                       |
        |  com.google.common.co |                       |                       |
        | llect.ImmutableSorted |                       |                       |
        | Map<Path,​SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util            | `ge                   |                       |
        | .function.Supplier<co | tComponentsRuleKey()` |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableSortedMap |                       |                       |
        | <String,​SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Py            | `of​(com.google.       |                       |
        | thonMappedComponents` | common.collect.Immuta |                       |
        |                       | bleSortedMap<Path,​Sou |                       |
        |                       | rcePath> components)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PythonMappe          | `resolvePythonCompo   | ::: block             |
        | dComponents.Resolved` | nents​(SourcePathResol | Convert this          |
        |                       | verAdapter resolver)` | [`Python              |
        |                       |                       | Components`](PythonCo |
        |                       |                       | mponents.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.features.python") |
        |                       |                       | to a                  |
        |                       |                       | [`Pyth                |
        |                       |                       | onComponents.Resolved |
        |                       |                       | `](PythonComponents.R |
        |                       |                       | esolved.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.features.python"), |
        |                       |                       | where all             |
        |                       |                       | [`SourcePath`](../.   |
        |                       |                       | ./core/sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath")s |
        |                       |                       | have been resolved to |
        |                       |                       | [`Path`](http://doc   |
        |                       |                       | s.oracle.com/javase/7 |
        |                       |                       | /docs/api/java/nio/fi |
        |                       |                       | le/Path.html?is-exter |
        |                       |                       | nal=true "class or in |
        |                       |                       | terface in java.nio.f |
        |                       |                       | ile"){.externalLink}s |
        |                       |                       | for use with          |
        |                       |                       | [`Step`               |
        |                       |                       | ](../../step/Step.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.step")s. |
        |                       |                       | :::                   |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PythonMappedComponents

                public PythonMappedComponents()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.google.common.collect.ImmutableSortedMap)}

        -   #### of

            ``` methodSignature
            public static PythonMappedComponents of​(com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> components)
            ```

        []{#getComponents()}

        -   #### getComponents

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> getComponents()
            ```

        []{#getComponentsRuleKey()}

        -   #### getComponentsRuleKey

            ``` methodSignature
            @Derived
            @Auxiliary
            public java.util.function.Supplier<com.google.common.collect.ImmutableSortedMap<String,​SourcePath>> getComponentsRuleKey()
            ```

        []{#forEachInput(java.util.function.Consumer)}

        -   #### forEachInput

            ``` methodSignature
            public void forEachInput​(java.util.function.Consumer<SourcePath> consumer)
            ```

            ::: block
            [Description copied from
            interface: `PythonComponents`]{.descfrmTypeLabel}
            :::

            ::: block
            Run `consumer` on all
            [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
            contained in this object.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `forEachInput` in interface `PythonComponents`

        []{#resolvePythonComponents(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### resolvePythonComponents

            ``` methodSignature
            public PythonMappedComponents.Resolved resolvePythonComponents​(SourcePathResolverAdapter resolver)
            ```

            ::: block
            [Description copied from
            interface: `PythonComponents`]{.descfrmTypeLabel}
            :::

            ::: block
            Convert this
            [`PythonComponents`](PythonComponents.html "interface in com.facebook.buck.features.python")
            to a
            [`PythonComponents.Resolved`](PythonComponents.Resolved.html "interface in com.facebook.buck.features.python"),
            where all
            [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
            have been resolved to
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s
            for use with
            [`Step`](../../step/Step.html "interface in com.facebook.buck.step")s.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolvePythonComponents` in
                interface `PythonComponents`

        []{#asSymlinks()}

        -   #### asSymlinks

            ``` methodSignature
            @Lazy
            public Symlinks asSymlinks()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asSymlinks` in interface `PythonComponents`

            [Returns:]{.returnLabel}
            :   a
                [`Symlinks`](../../core/rules/impl/Symlinks.html "interface in com.facebook.buck.core.rules.impl")
                used to symlink the components contained in this object
                via a
                [`SymlinkTree`](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")
                rule.
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
