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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Class Serializer {#class-serializer .title title="Class Serializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.Serializer

::: description
-   

    ------------------------------------------------------------------------

        public class Serializer
        extends Object

    ::: block
    Implementation of Serialization of Buildables.
    This works by walking all referenced values with a ValueVisitor.

    Referenced \"dynamic\" objects (i.e. implementations of
    AddsToRuleKey) are serialized as simply a hash of their serialized
    representation. The serialization of a complex object is then
    effectively a merkle tree. This allows us to share the serialized
    representation of shared objects (for c++ particularly, there are
    many shared references to the PreprocessorDelegate and other such
    fields).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Serializer.Delegate` | ::: block             |
        |                       |                       | The first time a      |
        |                       |                       | \"dynamic\" object is |
        |                       |                       | encountered           |
        |                       |                       | (including Buildables |
        |                       |                       | themselves),          |
        |                       |                       | registerNewValue will |
        |                       |                       | be called.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                       Description
          ------------------- ------------------------------------------- -------------
          `static int`        `TARGET_CONFIGURATION_TYPE_CONFIGURATION`    
          `static int`        `TARGET_CONFIGURATION_TYPE_DEFAULT`          
          `static int`        `TARGET_CONFIGURATION_TYPE_EMPTY`            

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------- -------------
          `Serializer​(SourcePathRuleFinder ruleFinder,           CellPathResolver cellResolver,           Serializer.Delegate delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T extends           | `res                  | ::: block             |
        | AddsToRuleKey>byte[]` | erialize​(T instance)` | Returns the           |
        |                       |                       | serialized bytes of   |
        |                       |                       | the instance.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends Adds      | `s                    | ::: block             |
        | ToRuleKey>com.google. | erialize​(T instance)` | Serializes an object. |
        | common.hash.HashCode` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T extend            | `serialize​(T i        | ::: block             |
        | s AddsToRuleKey>Eithe | nstance,          Cla | See Serialize(T       |
        | r<com.google.common.h | ssInfo<T> classInfo)` | instance) above.      |
        | ash.HashCode,​byte[]>` |                       | :::                   |
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
    -   []{#field.detail}

        ### Field Detail

        []{#TARGET_CONFIGURATION_TYPE_EMPTY}

        -   #### TARGET_CONFIGURATION_TYPE_EMPTY

                public static final int TARGET_CONFIGURATION_TYPE_EMPTY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.rules.modern.Serializer.TARGET_CONFIGURATION_TYPE_EMPTY)

        []{#TARGET_CONFIGURATION_TYPE_DEFAULT}

        -   #### TARGET_CONFIGURATION_TYPE_DEFAULT

                public static final int TARGET_CONFIGURATION_TYPE_DEFAULT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.rules.modern.Serializer.TARGET_CONFIGURATION_TYPE_DEFAULT)

        []{#TARGET_CONFIGURATION_TYPE_CONFIGURATION}

        -   #### TARGET_CONFIGURATION_TYPE_CONFIGURATION

                public static final int TARGET_CONFIGURATION_TYPE_CONFIGURATION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.rules.modern.Serializer.TARGET_CONFIGURATION_TYPE_CONFIGURATION)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.rules.modern.Serializer.Delegate)}

        -   #### Serializer

                public Serializer​(SourcePathRuleFinder ruleFinder,
                                  CellPathResolver cellResolver,
                                  Serializer.Delegate delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#serialize(com.facebook.buck.core.rulekey.AddsToRuleKey)}
        []{#serialize(T)}

        -   #### serialize

            ``` methodSignature
            public <T extends AddsToRuleKey> com.google.common.hash.HashCode serialize​(T instance)
                                                                                throws IOException
            ```

            ::: block
            Serializes an object. For small objects, the full serialized
            format will be returned as a byte\[\]. For larger objects,
            the representation will be recorded with the delegate and
            the hash will be returned.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#serialize(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.modern.ClassInfo)}
        []{#serialize(T,com.facebook.buck.rules.modern.ClassInfo)}

        -   #### serialize

            ``` methodSignature
            public <T extends AddsToRuleKey> Either<com.google.common.hash.HashCode,​byte[]> serialize​(T instance,
                                                                                                            ClassInfo<T> classInfo)
                                                                                                     throws IOException
            ```

            ::: block
            See Serialize(T instance) above.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#reserialize(com.facebook.buck.core.rulekey.AddsToRuleKey)}
        []{#reserialize(T)}

        -   #### reserialize

            ``` methodSignature
            public <T extends AddsToRuleKey> byte[] reserialize​(T instance)
                                                         throws IOException
            ```

            ::: block
            Returns the serialized bytes of the instance. This is useful
            if the caller has lost the value recorded in a previous
            serialize call.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
