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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Class CustomBehaviorUtils {#class-custombehaviorutils .title title="Class CustomBehaviorUtils"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.CustomBehaviorUtils

::: description
-   

    ------------------------------------------------------------------------

        public class CustomBehaviorUtils
        extends Object

    ::: block
    Utilities for dealing with CustomFieldBehavior and
    CustomClassBehavior.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `CustomBehaviorUtils()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <U e          | `get​(                 | ::: block             |
        | xtends CustomFieldBeh | Class<U> behaviorClas | Returns the field     |
        | aviorTag>Optional<U>` | s,    List<Class<? ex | behavior behavior of  |
        |                       | tends CustomFieldBeha | the requested type    |
        |                       | viorTag>> behaviors)` | (if there is one).    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <C e          | `                     | ::: block             |
        | xtends CustomClassBeh | getBehavior​(Class<?>  | Returns the class     |
        | aviorTag>Optional<Cus | clazz,            Cla | behavior of the       |
        | tomClassBehaviorTag>` | ss<C> behaviorClass)` | requested type (if    |
        |                       |                       | there is one).        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### CustomBehaviorUtils

                public CustomBehaviorUtils()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBehavior(java.lang.Class,java.lang.Class)}

        -   #### getBehavior

            ``` methodSignature
            public static <C extends CustomClassBehaviorTag> Optional<CustomClassBehaviorTag> getBehavior​(Class<?> clazz,
                                                                                                          Class<C> behaviorClass)
            ```

            ::: block
            Returns the class behavior of the requested type (if there
            is one).
            :::

        []{#get(java.lang.Class,java.util.List)}

        -   #### get

            ``` methodSignature
            public static <U extends CustomFieldBehaviorTag> Optional<U> get​(Class<U> behaviorClass,
                                                                             List<Class<? extends CustomFieldBehaviorTag>> behaviors)
            ```

            ::: block
            Returns the field behavior behavior of the requested type
            (if there is one).
            :::
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
