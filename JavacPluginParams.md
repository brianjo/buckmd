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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavacPluginParams {#class-javacpluginparams .title title="Class JavacPluginParams"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavacPluginParams

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class JavacPluginParams
        extends Object
        implements AddsToRuleKey

    ::: block
    Information for javac plugins (includes annotation processors).
    Javac Plugins involves a set of plugin properties, their
    classpath(s), and a few other command-line options for javac. We
    want to be able to specify all this various information in a BUCK
    configuration file and use it when we generate the javac command.
    This facilitates threading the information through buck in a more
    descriptive package rather than passing all the components
    separately.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Javac                | ::: block             |
        |                       | PluginParams.Builder` | A customized Builder  |
        |                       |                       | for                   |
        |                       |                       | JavacPluginParams.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type            Field     Description
          ---------------------------- --------- -------------
          `static JavacPluginParams`   `EMPTY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `JavacPluginParams()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                   Method                      Description
          ----------------------------------------------------------------------------------- --------------------------- -------------
          `static JavacPluginParams.Builder`                                                  `builder()`                  
          `abstract com.google.common.collect.ImmutableSortedSet<String>`                     `getParameters()`            
          `abstract com.google.common.collect.ImmutableList<ResolvedJavacPluginProperties>`   `getPluginProperties()`      
          `boolean`                                                                           `getProcessOnly()`           
          `boolean`                                                                           `isEmpty()`                  
          `JavacPluginParams`                                                                 `withAbiProcessorsOnly()`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY}

        -   #### EMPTY

                public static final JavacPluginParams EMPTY
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### JavacPluginParams

                public JavacPluginParams()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPluginProperties()}

        -   #### getPluginProperties

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<ResolvedJavacPluginProperties> getPluginProperties()
            ```

        []{#getParameters()}

        -   #### getParameters

            ``` methodSignature
            @NaturalOrder
            public abstract com.google.common.collect.ImmutableSortedSet<String> getParameters()
            ```

        []{#getProcessOnly()}

        -   #### getProcessOnly

            ``` methodSignature
            @Default
            public boolean getProcessOnly()
            ```

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static JavacPluginParams.Builder builder()
            ```

        []{#withAbiProcessorsOnly()}

        -   #### withAbiProcessorsOnly

            ``` methodSignature
            public JavacPluginParams withAbiProcessorsOnly()
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
