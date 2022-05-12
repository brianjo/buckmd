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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class BuildTarget {#class-buildtarget .title title="Class BuildTarget"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.BuildTarget

::: description
-   

    All Implemented Interfaces:
    :   `DependencyStack.Element`, `DependencyStack.ProvidesElement`,
        `Comparable<BuildTarget>`

    ------------------------------------------------------------------------

        @ThreadSafe
        public class BuildTarget
        extends Object
        implements Comparable<BuildTarget>, DependencyStack.Element
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildTarget`         | `assertUnflavored()`  | ::: block             |
        |                       |                       | Verifies that this    |
        |                       |                       | build target has no   |
        |                       |                       | flavors.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `compare              |                       |
        |                       | To​(BuildTarget that)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BaseName`            | `getBaseName()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CanonicalCellName`   | `getCell()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CellRelativePath`    | `getCe                |                       |
        |                       | llRelativeBasePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    | ::: block             |
        |                       | etCellRelativeName()` | If this build target  |
        |                       |                       | is                    |
        |                       |                       | cell//third_party/jav |
        |                       |                       | a/guava:guava-latest, |
        |                       |                       | then this would       |
        |                       |                       | return                |
        |                       |                       | \"//third_party/java/ |
        |                       |                       | guava:guava-latest\". |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getFlavorPostfix()`  | ::: block             |
        |                       |                       | An empty string when  |
        |                       |                       | there are no flavors, |
        |                       |                       | or hash followed by   |
        |                       |                       | comma-separated       |
        |                       |                       | flavors.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `FlavorSet`           | `getFlavors()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `                     |                       |
        |                       | getFlavorsAsString()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `get                  | ::: block             |
        |                       | FullyQualifiedName()` | If this build target  |
        |                       |                       | is                    |
        |                       |                       | cell//third_party/jav |
        |                       |                       | a/guava:guava-latest, |
        |                       |                       | then this would       |
        |                       |                       | return                |
        |                       |                       | \"ce                  |
        |                       |                       | ll//third_party/java/ |
        |                       |                       | guava:guava-latest\". |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortNa           | ::: block             |
        |                       | meAndFlavorPostfix()` | If this build target  |
        |                       |                       | were                  |
        |                       |                       | cell//third_party/jav |
        |                       |                       | a/guava:guava-latest, |
        |                       |                       | then this would       |
        |                       |                       | return                |
        |                       |                       | \"guava-latest\".     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `TargetConfiguration` | `getT                 |                       |
        |                       | argetConfiguration()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `getUncon             |                       |
        | onfiguredBuildTarget` | figuredBuildTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `U                    | `getUnf               |                       |
        | nflavoredBuildTarget` | lavoredBuildTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isFlavored()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toStrin              | ::: block             |
        |                       | gWithConfiguration()` | Target name and       |
        |                       |                       | configuration.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withAppendedFlavor   |                       |
        |                       | s​(Flavor... flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withAppendedFlavors​( |                       |
        |                       | Set<Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withFlavor           |                       |
        |                       | s​(Flavor... flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withFl               |                       |
        |                       | avors​(Iterable<? exte |                       |
        |                       | nds Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withoutFlavors()`    | ::: block             |
        |                       |                       | A copy of this build  |
        |                       |                       | target but without    |
        |                       |                       | any flavors.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withoutFlavor        |                       |
        |                       | s​(Flavor... flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withoutFlavors​(      |                       |
        |                       | Set<Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withShortNa          |                       |
        |                       | me​(String shortName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `withUnflavored       | ::: block             |
        |                       | BuildTarget​(Unflavore | Keep flavors and      |
        |                       | dBuildTarget target)` | configuration,        |
        |                       |                       | replace everything    |
        |                       |                       | else.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.exceptions.DependencyStack.Element}

            ### Methods inherited from interface com.facebook.buck.core.exceptions.[DependencyStack.Element](../exceptions/DependencyStack.Element.html "interface in com.facebook.buck.core.exceptions")

            `getElement`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnconfiguredBuildTarget()}

        -   #### getUnconfiguredBuildTarget

            ``` methodSignature
            public UnconfiguredBuildTarget getUnconfiguredBuildTarget()
            ```

        []{#getUnflavoredBuildTarget()}

        -   #### getUnflavoredBuildTarget

            ``` methodSignature
            public UnflavoredBuildTarget getUnflavoredBuildTarget()
            ```

        []{#getFlavors()}

        -   #### getFlavors

            ``` methodSignature
            public FlavorSet getFlavors()
            ```

        []{#getTargetConfiguration()}

        -   #### getTargetConfiguration

            ``` methodSignature
            public TargetConfiguration getTargetConfiguration()
            ```

        []{#getCell()}

        -   #### getCell

            ``` methodSignature
            public CanonicalCellName getCell()
            ```

        []{#getBaseName()}

        -   #### getBaseName

            ``` methodSignature
            public BaseName getBaseName()
            ```

        []{#getCellRelativeBasePath()}

        -   #### getCellRelativeBasePath

            ``` methodSignature
            public CellRelativePath getCellRelativeBasePath()
            ```

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

        []{#getShortNameAndFlavorPostfix()}

        -   #### getShortNameAndFlavorPostfix

            ``` methodSignature
            public String getShortNameAndFlavorPostfix()
            ```

            ::: block
            If this build target were
            cell//third_party/java/guava:guava-latest, then this would
            return \"guava-latest\". Note that the flavor of the target
            is included here.
            :::

        []{#getFlavorPostfix()}

        -   #### getFlavorPostfix

            ``` methodSignature
            public String getFlavorPostfix()
            ```

            ::: block
            An empty string when there are no flavors, or hash followed
            by comma-separated flavors.
            :::

        []{#getFlavorsAsString()}

        -   #### getFlavorsAsString

            ``` methodSignature
            protected String getFlavorsAsString()
            ```

        []{#getFullyQualifiedName()}

        -   #### getFullyQualifiedName

            ``` methodSignature
            public String getFullyQualifiedName()
            ```

            ::: block
            If this build target is
            cell//third_party/java/guava:guava-latest, then this would
            return \"cell//third_party/java/guava:guava-latest\".
            :::

        []{#getCellRelativeName()}

        -   #### getCellRelativeName

            ``` methodSignature
            public String getCellRelativeName()
            ```

            ::: block
            If this build target is
            cell//third_party/java/guava:guava-latest, then this would
            return \"//third_party/java/guava:guava-latest\".
            :::

        []{#isFlavored()}

        -   #### isFlavored

            ``` methodSignature
            public boolean isFlavored()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   [`getFullyQualifiedName()`](#getFullyQualifiedName())

        []{#toStringWithConfiguration()}

        -   #### toStringWithConfiguration

            ``` methodSignature
            public String toStringWithConfiguration()
            ```

            ::: block
            Target name and configuration.
            :::

        []{#withShortName(java.lang.String)}

        -   #### withShortName

            ``` methodSignature
            public BuildTarget withShortName​(String shortName)
            ```

        []{#assertUnflavored()}

        -   #### assertUnflavored

            ``` methodSignature
            public BuildTarget assertUnflavored()
            ```

            ::: block
            Verifies that this build target has no flavors.
            :::

            [Returns:]{.returnLabel}
            :   this build target

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if a build target has flavors

        []{#withoutFlavors(java.util.Set)}

        -   #### withoutFlavors

            ``` methodSignature
            public BuildTarget withoutFlavors​(Set<Flavor> flavors)
            ```

        []{#withoutFlavors(com.facebook.buck.core.model.Flavor...)}

        -   #### withoutFlavors

            ``` methodSignature
            public BuildTarget withoutFlavors​(Flavor... flavors)
            ```

        []{#withoutFlavors()}

        -   #### withoutFlavors

            ``` methodSignature
            public BuildTarget withoutFlavors()
            ```

            ::: block
            A copy of this build target but without any flavors.
            :::

        []{#withFlavors(com.facebook.buck.core.model.Flavor...)}

        -   #### withFlavors

            ``` methodSignature
            public BuildTarget withFlavors​(Flavor... flavors)
            ```

        []{#withFlavors(java.lang.Iterable)}

        -   #### withFlavors

            ``` methodSignature
            public BuildTarget withFlavors​(Iterable<? extends Flavor> flavors)
            ```

        []{#withAppendedFlavors(java.util.Set)}

        -   #### withAppendedFlavors

            ``` methodSignature
            public BuildTarget withAppendedFlavors​(Set<Flavor> flavors)
            ```

        []{#withAppendedFlavors(com.facebook.buck.core.model.Flavor...)}

        -   #### withAppendedFlavors

            ``` methodSignature
            public BuildTarget withAppendedFlavors​(Flavor... flavors)
            ```

        []{#withUnflavoredBuildTarget(com.facebook.buck.core.model.UnflavoredBuildTarget)}

        -   #### withUnflavoredBuildTarget

            ``` methodSignature
            public BuildTarget withUnflavoredBuildTarget​(UnflavoredBuildTarget target)
            ```

            ::: block
            Keep flavors and configuration, replace everything else.
            :::

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#compareTo(com.facebook.buck.core.model.BuildTarget)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(BuildTarget that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<BuildTarget>`
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
