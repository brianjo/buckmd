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
[Package]{.packageLabelInType} [com.facebook.buck.core.rulekey](package-summary.html)
:::

## Class MissingExcludeReporter {#class-missingexcludereporter .title title="Class MissingExcludeReporter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rulekey.MissingExcludeReporter

::: description
-   

    ------------------------------------------------------------------------

        public class MissingExcludeReporter
        extends Object

    ::: block
    Utility for reporting issues of fields/methods not being annotated
    to be added to rulekeys.
    This will only log a violation for a specific field/method once.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `MissingExcludeReporter()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `                     | ::: block             |
        |                       | reportExcludedField​(C | Report a field        |
        |                       | lass<?> instanceClass | that\'s being         |
        |                       | ,                     | processed for         |
        |                       | Field field,          | rulekeys and is       |
        |                       |            ExcludeFro | annotated with        |
        |                       | mRuleKey annotation)` | @[`ExcludeFr          |
        |                       |                       | omRuleKey`](ExcludeFr |
        |                       |                       | omRuleKey.html "annot |
        |                       |                       | ation in com.facebook |
        |                       |                       | .buck.core.rulekey"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `repor                | ::: block             |
        |                       | tExcludedMethod​(Class | Report a method       |
        |                       | <?> instanceClass,    | that\'s being         |
        |                       |                   Met | processed for         |
        |                       | hod method,           | rulekeys and is       |
        |                       |            ExcludeFro | annotated with        |
        |                       | mRuleKey annotation)` | @[`ExcludeFr          |
        |                       |                       | omRuleKey`](ExcludeFr |
        |                       |                       | omRuleKey.html "annot |
        |                       |                       | ation in com.facebook |
        |                       |                       | .buck.core.rulekey"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `reportFiel           | ::: block             |
        |                       | dMissingAnnotation​(Cl | Report a field        |
        |                       | ass<?> instanceClass, | that\'s being         |
        |                       |                       | processed for         |
        |                       |         Field field)` | rulekeys and is       |
        |                       |                       | missing both          |
        |                       |                       | @[`AddToRuleKey`](Ad  |
        |                       |                       | dToRuleKey.html "anno |
        |                       |                       | tation in com.faceboo |
        |                       |                       | k.buck.core.rulekey") |
        |                       |                       | and                   |
        |                       |                       | @[`ExcludeFr          |
        |                       |                       | omRuleKey`](ExcludeFr |
        |                       |                       | omRuleKey.html "annot |
        |                       |                       | ation in com.facebook |
        |                       |                       | .buck.core.rulekey"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `reportMethodMi       | ::: block             |
        |                       | ssingAnnotation​(Class | Report a method       |
        |                       | <?> instanceClass,    | that\'s being         |
        |                       |                       | processed for         |
        |                       |       Method method)` | rulekeys and is       |
        |                       |                       | missing both          |
        |                       |                       | @[`AddToRuleKey`](Ad  |
        |                       |                       | dToRuleKey.html "anno |
        |                       |                       | tation in com.faceboo |
        |                       |                       | k.buck.core.rulekey") |
        |                       |                       | and                   |
        |                       |                       | @[`ExcludeFr          |
        |                       |                       | omRuleKey`](ExcludeFr |
        |                       |                       | omRuleKey.html "annot |
        |                       |                       | ation in com.facebook |
        |                       |                       | .buck.core.rulekey"). |
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

        -   #### MissingExcludeReporter

                public MissingExcludeReporter()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#reportFieldMissingAnnotation(java.lang.Class,java.lang.reflect.Field)}

        -   #### reportFieldMissingAnnotation

            ``` methodSignature
            public static void reportFieldMissingAnnotation​(Class<?> instanceClass,
                                                            Field field)
            ```

            ::: block
            Report a field that\'s being processed for rulekeys and is
            missing both
            @[`AddToRuleKey`](AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey")
            and
            @[`ExcludeFromRuleKey`](ExcludeFromRuleKey.html "annotation in com.facebook.buck.core.rulekey").
            :::

        []{#reportMethodMissingAnnotation(java.lang.Class,java.lang.reflect.Method)}

        -   #### reportMethodMissingAnnotation

            ``` methodSignature
            public static void reportMethodMissingAnnotation​(Class<?> instanceClass,
                                                             Method method)
            ```

            ::: block
            Report a method that\'s being processed for rulekeys and is
            missing both
            @[`AddToRuleKey`](AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey")
            and
            @[`ExcludeFromRuleKey`](ExcludeFromRuleKey.html "annotation in com.facebook.buck.core.rulekey").
            :::

        []{#reportExcludedField(java.lang.Class,java.lang.reflect.Field,com.facebook.buck.core.rulekey.ExcludeFromRuleKey)}

        -   #### reportExcludedField

            ``` methodSignature
            public static void reportExcludedField​(Class<?> instanceClass,
                                                   Field field,
                                                   ExcludeFromRuleKey annotation)
            ```

            ::: block
            Report a field that\'s being processed for rulekeys and is
            annotated with
            @[`ExcludeFromRuleKey`](ExcludeFromRuleKey.html "annotation in com.facebook.buck.core.rulekey").
            :::

        []{#reportExcludedMethod(java.lang.Class,java.lang.reflect.Method,com.facebook.buck.core.rulekey.ExcludeFromRuleKey)}

        -   #### reportExcludedMethod

            ``` methodSignature
            public static void reportExcludedMethod​(Class<?> instanceClass,
                                                    Method method,
                                                    ExcludeFromRuleKey annotation)
            ```

            ::: block
            Report a method that\'s being processed for rulekeys and is
            annotated with
            @[`ExcludeFromRuleKey`](ExcludeFromRuleKey.html "annotation in com.facebook.buck.core.rulekey").
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
