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
[Package]{.packageLabelInType} [com.facebook.buck.core.artifact](package-summary.html)
:::

## Class SourceArtifactImpl {#class-sourceartifactimpl .title title="Class SourceArtifactImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.artifact.SourceArtifactImpl

::: description
-   

    All Implemented Interfaces:
    :   `Artifact`, `BoundArtifact`, `SourceArtifact`, `AddsToRuleKey`,
        `SkylarkArtifactApi`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `Comparable<Artifact>`

    ------------------------------------------------------------------------

        public abstract class SourceArtifactImpl
        extends Object
        implements SourceArtifact, BoundArtifact

    ::: block
    An artifact representing a source file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `SourceArtifactImpl()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                              Description
          --------------------------------------------------------- ----------------------------------------------------------------------------------- -------------
          `BoundArtifact`                                           `asBound()`                                                                          
          `BuildArtifact`                                           `asBuildArtifact()`                                                                  
          `com.facebook.buck.core.artifact.DeclaredArtifact`        `asDeclared()`                                                                       
          `OutputArtifact`                                          `asOutputArtifact()`                                                                 
          `SkylarkOutputArtifactApi`                                `asSkylarkOutputArtifact​(com.google.devtools.build.lib.events.Location location)`    
          `SourceArtifact`                                          `asSource()`                                                                         
          `int`                                                     `compareTo​(Artifact artifact)`                                                       
          `String`                                                  `getBasename()`                                                                      
          `String`                                                  `getExtension()`                                                                     
          `Object`                                                  `getOwner()`                                                                         
          `Optional<com.google.devtools.build.lib.cmdline.Label>`   `getOwnerTyped()`                                                                    
          `String`                                                  `getShortPath()`                                                                     
          `abstract PathSourcePath`                                 `getSourcePath()`                                                                    
          `boolean`                                                 `isBound()`                                                                          
          `boolean`                                                 `isSource()`                                                                         
          `static SourceArtifactImpl`                               `of​(PathSourcePath sourcePath)`                                                      
          `void`                                                    `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`        
          `protected void`                                          `requireBound()`                                                                     
          `protected void`                                          `requireDeclared()`                                                                  

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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.artifact.Artifact}

            ### Methods inherited from interface com.facebook.buck.core.artifact.[Artifact](Artifact.html "interface in com.facebook.buck.core.artifact")

            `asBound, asDeclared`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Comparable}

            ### Methods inherited from interface java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `compareTo`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.starlark.rule.artifact.SkylarkArtifactApi}

            ### Methods inherited from interface com.facebook.buck.core.starlark.rule.artifact.[SkylarkArtifactApi](../starlark/rule/artifact/SkylarkArtifactApi.html "interface in com.facebook.buck.core.starlark.rule.artifact")

            `getOwner, isImmutable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### SourceArtifactImpl

                public SourceArtifactImpl()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isBound()}

        -   #### isBound

            ``` methodSignature
            public final boolean isBound()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isBound` in interface `Artifact`

            [Returns:]{.returnLabel}
            :   whether the artifact is bound, as described above

        []{#getSourcePath()}

        -   #### getSourcePath

            ``` methodSignature
            public abstract PathSourcePath getSourcePath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePath` in interface `BoundArtifact`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePath` in interface `SourceArtifact`

            [Returns:]{.returnLabel}
            :   the path to the source file

        []{#asSource()}

        -   #### asSource

            ``` methodSignature
            @Nullable
            public SourceArtifact asSource()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asSource` in interface `BoundArtifact`

            [Returns:]{.returnLabel}
            :   this artifact as a
                [`SourceArtifact`](SourceArtifact.html "interface in com.facebook.buck.core.artifact"),
                null if this is not a
                [`SourceArtifact`](SourceArtifact.html "interface in com.facebook.buck.core.artifact")

        []{#asBuildArtifact()}

        -   #### asBuildArtifact

            ``` methodSignature
            @Nullable
            public BuildArtifact asBuildArtifact()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asBuildArtifact` in interface `BoundArtifact`

            [Returns:]{.returnLabel}
            :   this artifact as a
                [`BuildArtifact`](BuildArtifact.html "interface in com.facebook.buck.core.artifact"),
                null if this is not a
                [`BuildArtifact`](BuildArtifact.html "interface in com.facebook.buck.core.artifact")

        []{#getBasename()}

        -   #### getBasename

            ``` methodSignature
            @Lazy
            public String getBasename()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBasename` in interface `SkylarkArtifactApi`

        []{#getExtension()}

        -   #### getExtension

            ``` methodSignature
            @Lazy
            public String getExtension()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtension` in interface `SkylarkArtifactApi`

        []{#getOwnerTyped()}

        -   #### getOwnerTyped

            ``` methodSignature
            @Lazy
            public Optional<com.google.devtools.build.lib.cmdline.Label> getOwnerTyped()
            ```

            [Returns:]{.returnLabel}
            :   The Label of the rule that created this artifact, or
                [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
                if not applicable. This is converted to a Skylark
                appropriate type by
                [`SkylarkArtifactApi.getOwner()`](../starlark/rule/artifact/SkylarkArtifactApi.html#getOwner())

        []{#isSource()}

        -   #### isSource

            ``` methodSignature
            @Lazy
            public boolean isSource()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSource` in interface `SkylarkArtifactApi`

        []{#getShortPath()}

        -   #### getShortPath

            ``` methodSignature
            @Lazy
            public String getShortPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortPath` in interface `SkylarkArtifactApi`

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`

        []{#asSkylarkOutputArtifact(com.google.devtools.build.lib.events.Location)}

        -   #### asSkylarkOutputArtifact

            ``` methodSignature
            public SkylarkOutputArtifactApi asSkylarkOutputArtifact​(com.google.devtools.build.lib.events.Location location)
                                                             throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asSkylarkOutputArtifact` in
                interface `SkylarkArtifactApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#asOutputArtifact()}

        -   #### asOutputArtifact

            ``` methodSignature
            public OutputArtifact asOutputArtifact()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asOutputArtifact` in interface `Artifact`

            [Returns:]{.returnLabel}
            :   get this artifact as an
                [`OutputArtifact`](OutputArtifact.html "class in com.facebook.buck.core.artifact").
                Throws if cannot be converted

        []{#of(com.facebook.buck.core.sourcepath.PathSourcePath)}

        -   #### of

            ``` methodSignature
            public static SourceArtifactImpl of​(PathSourcePath sourcePath)
            ```

        []{#asBound()}

        -   #### asBound

            ``` methodSignature
            public final BoundArtifact asBound()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asBound` in interface `Artifact`

            [Returns:]{.returnLabel}
            :   a view of this artifact as a
                [`BoundArtifact`](BoundArtifact.html "interface in com.facebook.buck.core.artifact")

        []{#asDeclared()}

        -   #### asDeclared

            ``` methodSignature
            public final com.facebook.buck.core.artifact.DeclaredArtifact asDeclared()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asDeclared` in interface `Artifact`

            [Returns:]{.returnLabel}
            :   a view of this artifact as a `DeclaredArtifact`

        []{#requireBound()}

        -   #### requireBound

            ``` methodSignature
            protected void requireBound()
            ```

        []{#requireDeclared()}

        -   #### requireDeclared

            ``` methodSignature
            protected void requireDeclared()
            ```

        []{#getOwner()}

        -   #### getOwner

            ``` methodSignature
            public final Object getOwner()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOwner` in interface `SkylarkArtifactApi`

        []{#compareTo(com.facebook.buck.core.artifact.Artifact)}

        -   #### compareTo

            ``` methodSignature
            public final int compareTo​(Artifact artifact)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<Artifact>`
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
