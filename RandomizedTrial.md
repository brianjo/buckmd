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
[Package]{.packageLabelInType} [com.facebook.buck.util.randomizedtrial](package-summary.html)
:::

## Class RandomizedTrial {#class-randomizedtrial .title title="Class RandomizedTrial"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.randomizedtrial.RandomizedTrial

::: description
-   

    ------------------------------------------------------------------------

        public class RandomizedTrial
        extends Object

    ::: block
    Simple implementation of A/B testing. Each RandomizedTrial selects a
    group to which buck instance belongs to.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stat                 | `getGroup​(St          | ::: block             |
        | ic <T extends Enum<T> | ring name,         St | Returns a group for   |
        |  & WithProbability>T` | ring buildId,         | trial with given      |
        |                       |  Class<T> enumClass)` | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getGroup​(Stri        | ::: block             |
        | <T extends Enum<T>>T` | ng name,         Stri | Returns a group for   |
        |                       | ng buildId,         M | trial with given      |
        |                       | ap<T,​Double> enumValu | name.                 |
        |                       | esWithProbabilities)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `getGroupStable​(Strin | ::: block             |
        | ic <T extends Enum<T> | g name,               | Returns a group for   |
        |  & WithProbability>T` |  Class<T> enumClass)` | trial with given      |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `g                    | ::: block             |
        | <T extends Enum<T>>T` | etGroupStable​(String  | Returns a group for   |
        |                       | name,               M | trial with given      |
        |                       | ap<T,​Double> enumValu | name.                 |
        |                       | esWithProbabilities)` | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#getGroupStable(java.lang.String,java.lang.Class)}

        -   #### getGroupStable

            ``` methodSignature
            public static <T extends Enum<T> & WithProbability> T getGroupStable​(String name,
                                                                                 Class<T> enumClass)
            ```

            ::: block
            Returns a group for trial with given name.
            This choice is stable for each test/user/hostname.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - name of trial.
            :   `enumClass` - Class of an enum which conforms to
                [`WithProbability`](WithProbability.html "interface in com.facebook.buck.util.randomizedtrial")
                interface.

        []{#getGroupStable(java.lang.String,java.util.Map)}

        -   #### getGroupStable

            ``` methodSignature
            public static <T extends Enum<T>> T getGroupStable​(String name,
                                                               Map<T,​Double> enumValuesWithProbabilities)
            ```

            ::: block
            Returns a group for trial with given name.
            This choice is stable for each test/user/hostname.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - name of trial.
            :   `enumValuesWithProbabilities` - Map of enum values to
                probabilities.

        []{#getGroup(java.lang.String,java.lang.String,java.util.Map)}

        -   #### getGroup

            ``` methodSignature
            public static <T extends Enum<T>> T getGroup​(String name,
                                                         String buildId,
                                                         Map<T,​Double> enumValuesWithProbabilities)
            ```

            ::: block
            Returns a group for trial with given name.
            This choice is stable for a particular
            buildId/test/user/hostname.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - name of trial.
            :   `enumValuesWithProbabilities` - Map of enum values to
                probabilities.

        []{#getGroup(java.lang.String,java.lang.String,java.lang.Class)}

        -   #### getGroup

            ``` methodSignature
            public static <T extends Enum<T> & WithProbability> T getGroup​(String name,
                                                                           String buildId,
                                                                           Class<T> enumClass)
            ```

            ::: block
            Returns a group for trial with given name.
            This choice is stable for a particular
            buildId/test/user/hostname.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - name of trial.
            :   `enumClass` - Class of an enum which conforms to
                [`WithProbability`](WithProbability.html "interface in com.facebook.buck.util.randomizedtrial")
                interface.
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
