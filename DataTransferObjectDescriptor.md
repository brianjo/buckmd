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

## Class DataTransferObjectDescriptor\<T extends [DataTransferObject](../../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")\> {#class-datatransferobjectdescriptort-extends-datatransferobject .title title="Class DataTransferObjectDescriptor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.DataTransferObjectDescriptor\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class DataTransferObjectDescriptor<T extends DataTransferObject>
        extends Object

    ::: block
    Class that contains the values needed to build a DescriptionArg
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `DataTransferObj      | ::: block             |
        |                       | ectDescriptor.Builder | Checked exception     |
        |                       | BuildFailedException` | thrown by             |
        |                       |                       | [`DataTra             |
        |                       |                       | nsferObjectDescriptor |
        |                       |                       | .BuilderBuildFunction |
        |                       |                       | `](DataTransferObject |
        |                       |                       | Descriptor.BuilderBui |
        |                       |                       | ldFunction.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.rules.coercer") |
        |                       |                       | when a user error     |
        |                       |                       | (not internal error)  |
        |                       |                       | occurs.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `DataTransfe          | ::: block             |
        |                       | rObjectDescriptor.Bui | A function to build a |
        |                       | lderBuildFunction<T>` | builder returned by   |
        |                       |                       | [`g                   |
        |                       |                       | etBuilderFactory()`]( |
        |                       |                       | #getBuilderFactory()) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `DataTransferObjectDescriptor()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `T`                   | `b                    | ::: block             |
        |                       | uild​(Object builder,  | Builds the partially  |
        |                       |      Object context)` | constructed object    |
        |                       |                       | returned by           |
        |                       |                       | [`g                   |
        |                       |                       | etBuilderFactory()`]( |
        |                       |                       | #getBuilderFactory()) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getBuilderFactory()` | ::: block             |
        | tract java.util.funct |                       | Get the builder for a |
        | ion.Supplier<Object>` |                       | constructor arg.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getBuildFunction()`  | ::: block             |
        |  abstract DataTransfe |                       | A function that takes |
        | rObjectDescriptor.Bui |                       | the result of         |
        | lderBuildFunction<T>` |                       | [`get                 |
        |                       |                       | BuilderFactory()`](#g |
        |                       |                       | etBuilderFactory())}, |
        |                       |                       | and calls its         |
        |                       |                       | \'build\' function to |
        |                       |                       | return description    |
        |                       |                       | args of type `T`      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `getParamInfos()`     | ::: block             |
        | ct com.google.common. |                       | The param infos       |
        | collect.ImmutableMap< |                       | needed to populate    |
        | String,​ParamInfo<?>>` |                       | this object           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Class<T>`   | `objectClass()`       | ::: block             |
        |                       |                       | Reified `<T>`         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(Class<            |                       |
        |  <T extends DataTrans | T> objectClass,   jav |                       |
        | ferObject>DataTransfe | a.util.function.Suppl |                       |
        | rObjectDescriptor<T>` | ier<Object> builderFa |                       |
        |                       | ctory,   Map<String,​? |                       |
        |                       |  extends ParamInfo<?> |                       |
        |                       | > paramInfos,   DataT |                       |
        |                       | ransferObjectDescript |                       |
        |                       | or.BuilderBuildFuncti |                       |
        |                       | on<T> buildFunction)` |                       |
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

        -   #### DataTransferObjectDescriptor

                public DataTransferObjectDescriptor()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#objectClass()}

        -   #### objectClass

            ``` methodSignature
            public abstract Class<T> objectClass()
            ```

            ::: block
            Reified `<T>`
            :::

        []{#getBuilderFactory()}

        -   #### getBuilderFactory

            ``` methodSignature
            public abstract java.util.function.Supplier<Object> getBuilderFactory()
            ```

            ::: block
            Get the builder for a constructor arg.
            This is either the ImmutableValue.Builder class for `T`, or
            [`SkylarkDescriptionArg`](../../core/starlark/rule/SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule")
            :::

        []{#getParamInfos()}

        -   #### getParamInfos

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​ParamInfo<?>> getParamInfos()
            ```

            ::: block
            The param infos needed to populate this object
            :::

        []{#getBuildFunction()}

        -   #### getBuildFunction

            ``` methodSignature
            protected abstract DataTransferObjectDescriptor.BuilderBuildFunction<T> getBuildFunction()
            ```

            ::: block
            A function that takes the result of
            [`getBuilderFactory()`](#getBuilderFactory())}, and calls
            its \'build\' function to return description args of type
            `T`
            :::

        []{#build(java.lang.Object,java.lang.Object)}

        -   #### build

            ``` methodSignature
            public T build​(Object builder,
                           Object context)
            ```

            ::: block
            Builds the partially constructed object returned by
            [`getBuilderFactory()`](#getBuilderFactory())
            :::

            [Returns:]{.returnLabel}
            :   A fully constructed ConstructorArg of type `T` obtained
                by applying [`getBuildFunction()`](#getBuildFunction())
                to [`getBuilderFactory()`](#getBuilderFactory())

        []{#of(java.lang.Class,java.util.function.Supplier,java.util.Map,com.facebook.buck.rules.coercer.DataTransferObjectDescriptor.BuilderBuildFunction)}

        -   #### of

            ``` methodSignature
            public static <T extends DataTransferObject> DataTransferObjectDescriptor<T> of​(Class<T> objectClass,
                                                                                            java.util.function.Supplier<Object> builderFactory,
                                                                                            Map<String,​? extends ParamInfo<?>> paramInfos,
                                                                                            DataTransferObjectDescriptor.BuilderBuildFunction<T> buildFunction)
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
