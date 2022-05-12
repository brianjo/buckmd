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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser.buildtargetpattern](package-summary.html)
:::

## Class BuildTargetPattern {#class-buildtargetpattern .title title="Class BuildTargetPattern"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.parser.buildtargetpattern.BuildTargetPattern

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuildTargetPattern
        extends Object

    ::: block
    Parsed representation of build target pattern
    Refer to
    [`BuildTargetPatternParser`](BuildTargetPatternParser.html "class in com.facebook.buck.core.parser.buildtargetpattern")
    for acceptable pattern formats
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Bui                  | ::: block             |
        |                       | ldTargetPattern.Kind` | Type of a pattern     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `BuildTargetPattern()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             | ::: block             |
        |                       |                       | Validate that target  |
        |                       |                       | name is only present  |
        |                       |                       | when necessary        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getCe                | ::: block             |
        | act CellRelativePath` | llRelativeBasePath()` | Path to the package   |
        |                       |                       | folder that is a root |
        |                       |                       | for all build targets |
        |                       |                       | matched by a pattern  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Bui         | `getKind()`           | ::: block             |
        | ldTargetPattern.Kind` |                       | Type of the parsed    |
        |                       |                       | pattern               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getL                 | ::: block             |
        |                       | ocalNameAndFlavors()` | Target name in case   |
        |                       |                       | pattern is single     |
        |                       |                       | build target pattern; |
        |                       |                       | otherwise an empty    |
        |                       |                       | string                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRecursive()`       | ::: block             |
        |                       |                       | Whether this is a     |
        |                       |                       | \'//package/\...\'    |
        |                       |                       | pattern.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `of​(CellRelativePath  |                       |
        | c BuildTargetPattern` | cellRelativeBasePath, |                       |
        |                       |    BuildTargetPattern |                       |
        |                       | .Kind kind,   String  |                       |
        |                       | localNameAndFlavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildTargetPattern

                public BuildTargetPattern()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellRelativeBasePath()}

        -   #### getCellRelativeBasePath

            ``` methodSignature
            public abstract CellRelativePath getCellRelativeBasePath()
            ```

            ::: block
            Path to the package folder that is a root for all build
            targets matched by a pattern
            :::

        []{#getKind()}

        -   #### getKind

            ``` methodSignature
            public abstract BuildTargetPattern.Kind getKind()
            ```

            ::: block
            Type of the parsed pattern
            :::

        []{#getLocalNameAndFlavors()}

        -   #### getLocalNameAndFlavors

            ``` methodSignature
            public abstract String getLocalNameAndFlavors()
            ```

            ::: block
            Target name in case pattern is single build target pattern;
            otherwise an empty string
            :::

        []{#isRecursive()}

        -   #### isRecursive

            ``` methodSignature
            public boolean isRecursive()
            ```

            ::: block
            Whether this is a \'//package/\...\' pattern.
            :::

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

            ::: block
            Validate that target name is only present when necessary
            Should we move it to factory
            [`BuildTargetPatternParser`](BuildTargetPatternParser.html "class in com.facebook.buck.core.parser.buildtargetpattern")?
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#of(com.facebook.buck.core.model.CellRelativePath,com.facebook.buck.core.parser.buildtargetpattern.BuildTargetPattern.Kind,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static BuildTargetPattern of​(CellRelativePath cellRelativeBasePath,
                                                BuildTargetPattern.Kind kind,
                                                String localNameAndFlavors)
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
