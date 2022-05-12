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

## Class UnconfiguredBuildTarget {#class-unconfiguredbuildtarget .title title="Class UnconfiguredBuildTarget"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.UnconfiguredBuildTarget

::: description
-   

    All Implemented Interfaces:
    :   `DependencyStack.Element`, `DependencyStack.ProvidesElement`,
        `QueryTarget`, `Comparable<UnconfiguredBuildTarget>`

    ------------------------------------------------------------------------

        public class UnconfiguredBuildTarget
        extends Object
        implements Comparable<UnconfiguredBuildTarget>, QueryTarget, DependencyStack.Element

    ::: block
    Data object that holds properties to uniquely identify a build
    target with flavors
    In other words, this represents a parsed representation of a build
    target with flavors but without configuration.

    For example, a fully qualified target name like
    \`cell//path/to:target#flavor1,flavor2\` parses \`cell\` as a cell
    name, \`//path/to\` as a base name that corresponds to the real path
    to the build file that contains a target, \`target\` is a target
    name found in that build file and \`flavor1\` and \'flavor2\' as
    flavors as applied to this build target.

    Flavors are a legacy way to configure a build target so it can
    mutate its behavior based on user-provided input or client settings,
    like target or running platforms. Flavors should not be used
    anymore, instead you want to use a
    [`BuildTarget`](BuildTarget.html "class in com.facebook.buck.core.model")
    along with passed
    [`TargetConfiguration`](TargetConfiguration.html "class in com.facebook.buck.core.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Unc                  | `assertUnflavored()`  | ::: block             |
        | onfiguredBuildTarget` |                       | Verifies that this    |
        |                       |                       | build target has no   |
        |                       |                       | flavors.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `compareTo​(Unconfigu  |                       |
        |                       | redBuildTarget that)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `configure            |                       |
        |                       | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BaseName`            | `getBaseName()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CanonicalCellName`   | `getCell()`           | ::: block             |
        |                       |                       | Name of the cell that |
        |                       |                       | current build target  |
        |                       |                       | belongs to            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CellRelativePath`    | `getCe                | ::: block             |
        |                       | llRelativeBasePath()` | Typed version of      |
        |                       |                       | [`getBaseName         |
        |                       |                       | ()`](#getBaseName()). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    |                       |
        |                       | etCellRelativeName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Dep                  | `getElement()`        |                       |
        | endencyStack.Element` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `FlavorSet`           | `getFlavors()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getFlavorSet()`      | ::: block             |
        | common.collect.Immuta |                       | Set of flavors used   |
        | bleSortedSet<Flavor>` |                       | with that build       |
        |                       |                       | target.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `get                  | ::: block             |
        |                       | FullyQualifiedName()` | Fully qualified name  |
        |                       |                       | of unconfigured build |
        |                       |                       | target, for example   |
        |                       |                       | cell//some/target     |
        |                       |                       | :name#flavor1,flavor2 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Name of the build     |
        |                       |                       | target, i.e.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortNa           |                       |
        |                       | meAndFlavorPostfix()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `U                    | `getUnf               |                       |
        | nflavoredBuildTarget` | lavoredBuildTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isFlavored()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Unc           | `                     | ::: block             |
        | onfiguredBuildTarget` | of​(CanonicalCellName  | A constructor         |
        |                       | cell,   BaseName base | :::                   |
        |                       | Name,   String name,  |                       |
        |                       |   FlavorSet flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Unc           | `                     | ::: block             |
        | onfiguredBuildTarget` | of​(BaseName baseName, | Helper for creating a |
        |                       |    String shortName)` | build target in the   |
        |                       |                       | root cell with no     |
        |                       |                       | flavors.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Unc           | `of​(Unf               | ::: block             |
        | onfiguredBuildTarget` | lavoredBuildTarget un | A constructor         |
        |                       | flavoredBuildTarget,  | :::                   |
        |                       |   FlavorSet flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `withFlavor           | ::: block             |
        | onfiguredBuildTarget` | s​(Flavor... flavors)` | Creates a new build   |
        |                       |                       | target by copying all |
        |                       |                       | of the information    |
        |                       |                       | from this build       |
        |                       |                       | target and using the  |
        |                       |                       | provided flavors as   |
        |                       |                       | flavors in the new    |
        |                       |                       | build target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `withFl               | ::: block             |
        | onfiguredBuildTarget` | avors​(Iterable<? exte | Creates a new build   |
        |                       | nds Flavor> flavors)` | target by copying all |
        |                       |                       | of the information    |
        |                       |                       | from this build       |
        |                       |                       | target and using the  |
        |                       |                       | provided flavors as   |
        |                       |                       | flavors in the new    |
        |                       |                       | build target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `withLocalNa          |                       |
        | onfiguredBuildTarget` | me​(String localName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `withoutFlavors()`    |                       |
        | onfiguredBuildTarget` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `withShortNa          | ::: block             |
        | onfiguredBuildTarget` | me​(String shortName)` | Creates a new build   |
        |                       |                       | target by copying all |
        |                       |                       | of the information    |
        |                       |                       | from this build       |
        |                       |                       | target and replacing  |
        |                       |                       | the short name with   |
        |                       |                       | the given name.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `withUnflavored       |                       |
        | onfiguredBuildTarget` | BuildTarget​(Unflavore |                       |
        |                       | dBuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnflavoredBuildTarget()}

        -   #### getUnflavoredBuildTarget

            ``` methodSignature
            public UnflavoredBuildTarget getUnflavoredBuildTarget()
            ```

        []{#getCell()}

        -   #### getCell

            ``` methodSignature
            public CanonicalCellName getCell()
            ```

            ::: block
            Name of the cell that current build target belongs to
            :::

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

            ::: block
            Typed version of [`getBaseName()`](#getBaseName()).
            :::

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Name of the build target, i.e. part of fully qualified name
            after the colon If this build target were
            cell_name//third_party/java/guava:guava-latest, then this
            would return \"guava-latest\"
            :::

        []{#getFlavorSet()}

        -   #### getFlavorSet

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Flavor> getFlavorSet()
            ```

            ::: block
            Set of flavors used with that build target.
            :::

        []{#getFlavors()}

        -   #### getFlavors

            ``` methodSignature
            public FlavorSet getFlavors()
            ```

        []{#getFullyQualifiedName()}

        -   #### getFullyQualifiedName

            ``` methodSignature
            public String getFullyQualifiedName()
            ```

            ::: block
            Fully qualified name of unconfigured build target, for
            example cell//some/target:name#flavor1,flavor2
            :::

        []{#getShortNameAndFlavorPostfix()}

        -   #### getShortNameAndFlavorPostfix

            ``` methodSignature
            public String getShortNameAndFlavorPostfix()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#compareTo(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(UnconfiguredBuildTarget that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<UnconfiguredBuildTarget>`

        []{#getCellRelativeName()}

        -   #### getCellRelativeName

            ``` methodSignature
            public String getCellRelativeName()
            ```

        []{#getElement()}

        -   #### getElement

            ``` methodSignature
            public DependencyStack.Element getElement()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getElement` in interface `DependencyStack.Element`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getElement` in
                interface `DependencyStack.ProvidesElement`

        []{#of(com.facebook.buck.core.model.UnflavoredBuildTarget,com.facebook.buck.core.model.FlavorSet)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredBuildTarget of​(UnflavoredBuildTarget unflavoredBuildTarget,
                                                     FlavorSet flavors)
            ```

            ::: block
            A constructor
            :::

        []{#of(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.model.BaseName,java.lang.String,com.facebook.buck.core.model.FlavorSet)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredBuildTarget of​(CanonicalCellName cell,
                                                     BaseName baseName,
                                                     String name,
                                                     FlavorSet flavors)
            ```

            ::: block
            A constructor
            :::

        []{#of(com.facebook.buck.core.model.BaseName,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredBuildTarget of​(BaseName baseName,
                                                     String shortName)
            ```

            ::: block
            Helper for creating a build target in the root cell with no
            flavors.
            :::

        []{#withoutFlavors()}

        -   #### withoutFlavors

            ``` methodSignature
            public UnconfiguredBuildTarget withoutFlavors()
            ```

        []{#withLocalName(java.lang.String)}

        -   #### withLocalName

            ``` methodSignature
            public UnconfiguredBuildTarget withLocalName​(String localName)
            ```

        []{#configure(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### configure

            ``` methodSignature
            public BuildTarget configure​(TargetConfiguration targetConfiguration)
            ```

        []{#isFlavored()}

        -   #### isFlavored

            ``` methodSignature
            public boolean isFlavored()
            ```

        []{#withFlavors(java.lang.Iterable)}

        -   #### withFlavors

            ``` methodSignature
            public UnconfiguredBuildTarget withFlavors​(Iterable<? extends Flavor> flavors)
            ```

            ::: block
            Creates a new build target by copying all of the information
            from this build target and using the provided flavors as
            flavors in the new build target.
            :::

            [Parameters:]{.paramLabel}
            :   `flavors` - flavors to use when creating a new build
                target

        []{#withFlavors(com.facebook.buck.core.model.Flavor...)}

        -   #### withFlavors

            ``` methodSignature
            public UnconfiguredBuildTarget withFlavors​(Flavor... flavors)
            ```

            ::: block
            Creates a new build target by copying all of the information
            from this build target and using the provided flavors as
            flavors in the new build target.
            :::

            [Parameters:]{.paramLabel}
            :   `flavors` - flavors to use when creating a new build
                target

        []{#withShortName(java.lang.String)}

        -   #### withShortName

            ``` methodSignature
            public UnconfiguredBuildTarget withShortName​(String shortName)
            ```

            ::: block
            Creates a new build target by copying all of the information
            from this build target and replacing the short name with the
            given name.
            :::

            [Parameters:]{.paramLabel}
            :   `shortName` - short name of the new build target

        []{#withUnflavoredBuildTarget(com.facebook.buck.core.model.UnflavoredBuildTarget)}

        -   #### withUnflavoredBuildTarget

            ``` methodSignature
            public UnconfiguredBuildTarget withUnflavoredBuildTarget​(UnflavoredBuildTarget target)
            ```

        []{#assertUnflavored()}

        -   #### assertUnflavored

            ``` methodSignature
            public UnconfiguredBuildTarget assertUnflavored()
            ```

            ::: block
            Verifies that this build target has no flavors.
            :::

            [Returns:]{.returnLabel}
            :   this build target

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if a build target has flavors
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
