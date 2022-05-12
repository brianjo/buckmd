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

## Class BuildConfigFields {#class-buildconfigfields .title title="Class BuildConfigFields"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.BuildConfigFields

::: description
-   

    All Implemented Interfaces:
    :   `Iterable<BuildConfigFields.Field>`

    ------------------------------------------------------------------------

        @Enclosing
        public abstract class BuildConfigFields
        extends Object
        implements Iterable<BuildConfigFields.Field>

    ::: block
    List of fields to add to a generated `BuildConfig.java` file. Each
    field knows its Java type, variable name, and value.
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
        |                       | ldConfigFields.Field` | An individual field   |
        |                       |                       | in a                  |
        |                       |                       | [`Bui                 |
        |                       |                       | ldConfigFields`](Buil |
        |                       |                       | dConfigFields.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.rules.coercer"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `BuildConfigFields()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stat                 | `fromFieldDe          |                       |
        | ic BuildConfigFields` | clarations​(Iterable<S |                       |
        |                       | tring> declarations)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `fromFields​(          |                       |
        | ic BuildConfigFields` | Iterable<BuildConfigF |                       |
        |                       | ields.Field> fields)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `generateBuildC       | ::: block             |
        |                       | onfigDotJava​(Unflavor | Creates the Java code |
        |                       | edBuildTarget source, | for a                 |
        |                       |                       | `BuildConfig.java`    |
        |                       |       String javaPack | file in the specified |
        |                       | age,                  | `javaPackage`.        |
        |                       |           boolean use | :::                   |
        |                       | ConstantExpressions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getNameToField()`    |                       |
        | tract Map<String,​Buil |                       |                       |
        | dConfigFields.Field>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterator<Buil        | `iterator()`          |                       |
        | dConfigFields.Field>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `of()`                |                       |
        | ic BuildConfigFields` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `of​(Map<String,​? exte |                       |
        | ic BuildConfigFields` | nds BuildConfigFields |                       |
        |                       | .Field> nameToField)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildConfigFields`   | `putAll​(Build         |                       |
        |                       | ConfigFields fields)` |                       |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Iterable}

            ### Methods inherited from interface java.lang.[Iterable](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `forEach, spliterator`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildConfigFields

                public BuildConfigFields()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNameToField()}

        -   #### getNameToField

            ``` methodSignature
            public abstract Map<String,​BuildConfigFields.Field> getNameToField()
            ```

        []{#of(java.util.Map)}

        -   #### of

            ``` methodSignature
            public static BuildConfigFields of​(Map<String,​? extends BuildConfigFields.Field> nameToField)
            ```

        []{#of()}

        -   #### of

            ``` methodSignature
            public static BuildConfigFields of()
            ```

        []{#fromFieldDeclarations(java.lang.Iterable)}

        -   #### fromFieldDeclarations

            ``` methodSignature
            public static BuildConfigFields fromFieldDeclarations​(Iterable<String> declarations)
            ```

        []{#fromFields(java.lang.Iterable)}

        -   #### fromFields

            ``` methodSignature
            public static BuildConfigFields fromFields​(Iterable<BuildConfigFields.Field> fields)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`BuildConfigFields`](BuildConfigFields.html "class in com.facebook.buck.rules.coercer")
                that contains the specified fields in iteration order.

        []{#putAll(com.facebook.buck.rules.coercer.BuildConfigFields)}

        -   #### putAll

            ``` methodSignature
            public BuildConfigFields putAll​(BuildConfigFields fields)
            ```

            [Returns:]{.returnLabel}
            :   A new
                [`BuildConfigFields`](BuildConfigFields.html "class in com.facebook.buck.rules.coercer")
                with all of the fields from this object, combined with
                all of the fields from the specified `fields`. If both
                objects have fields with the same name, the entry from
                the `fields` parameter wins.

        []{#generateBuildConfigDotJava(com.facebook.buck.core.model.UnflavoredBuildTarget,java.lang.String,boolean)}

        -   #### generateBuildConfigDotJava

            ``` methodSignature
            public String generateBuildConfigDotJava​(UnflavoredBuildTarget source,
                                                     String javaPackage,
                                                     boolean useConstantExpressions)
            ```

            ::: block
            Creates the Java code for a `BuildConfig.java` file in the
            specified `javaPackage`.
            :::

            [Parameters:]{.paramLabel}
            :   `source` - The build target of the rule that is
                responsible for generating this BuildConfig.java file.
            :   `javaPackage` - The Java package for the generated file.
            :   `useConstantExpressions` - Whether the value of each
                field in the generated Java code should be the literal
                value from the
                [`BuildConfigFields.Field`](BuildConfigFields.Field.html "class in com.facebook.buck.rules.coercer")
                (i.e., a constant expression) or a
                non-constant-expression that is guaranteed to evaluate
                to the literal value.

        []{#iterator()}

        -   #### iterator

            ``` methodSignature
            public Iterator<BuildConfigFields.Field> iterator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `iterator` in
                interface `Iterable<BuildConfigFields.Field>`

            [Returns:]{.returnLabel}
            :   iterator that enumerates the fields used to construct
                this
                [`BuildConfigFields`](BuildConfigFields.html "class in com.facebook.buck.rules.coercer").
                The
                [`Iterator.remove()`](http://docs.oracle.com/javase/7/docs/api/java/util/Iterator.html?is-external=true#remove() "class or interface in java.util"){.externalLink}
                method of the return value is not supported.

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   value that represents the data stored in this object
                such that it can be used to represent this object in a
                [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey").
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
