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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.impl](package-summary.html)
:::

## Class JsonTargetConfigurationSerializer {#class-jsontargetconfigurationserializer .title title="Class JsonTargetConfigurationSerializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.impl.JsonTargetConfigurationSerializer

::: description
-   

    All Implemented Interfaces:
    :   `TargetConfigurationSerializer`

    ------------------------------------------------------------------------

        public class JsonTargetConfigurationSerializer
        extends Object
        implements TargetConfigurationSerializer

    ::: block
    Serializer that uses JSON to represent
    [`TargetConfiguration`](../TargetConfiguration.html "class in com.facebook.buck.core.model")
    in a text form.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------- -------------
          `JsonTargetConfigurationSerializer​(java.util.function.Function<String,​UnconfiguredBuildTarget> buildTargetProvider)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `TargetConfiguration` | `deserial             | ::: block             |
        |                       | ize​(String rawValue)` | Creates               |
        |                       |                       | [`Target              |
        |                       |                       | Configuration`](../Ta |
        |                       |                       | rgetConfiguration.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | from the provided     |
        |                       |                       | text representation.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `serialize            | ::: block             |
        |                       | ​(TargetConfiguration  | Converts              |
        |                       | targetConfiguration)` | [`Target              |
        |                       |                       | Configuration`](../Ta |
        |                       |                       | rgetConfiguration.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | to string.            |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Function)}

        -   #### JsonTargetConfigurationSerializer

                public JsonTargetConfigurationSerializer​(java.util.function.Function<String,​UnconfiguredBuildTarget> buildTargetProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#serialize(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### serialize

            ``` methodSignature
            public String serialize​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `TargetConfigurationSerializer`]{.descfrmTypeLabel}
            :::

            ::: block
            Converts
            [`TargetConfiguration`](../TargetConfiguration.html "class in com.facebook.buck.core.model")
            to string.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in interface `TargetConfigurationSerializer`

        []{#deserialize(java.lang.String)}

        -   #### deserialize

            ``` methodSignature
            public TargetConfiguration deserialize​(String rawValue)
            ```

            ::: block
            [Description copied from
            interface: `TargetConfigurationSerializer`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates
            [`TargetConfiguration`](../TargetConfiguration.html "class in com.facebook.buck.core.model")
            from the provided text representation.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `deserialize` in
                interface `TargetConfigurationSerializer`
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
