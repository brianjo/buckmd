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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class ResourceAmounts {#class-resourceamounts .title title="Class ResourceAmounts"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.ResourceAmounts

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ResourceAmounts
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static int`          | `RESOURCE_TYPE_COUNT` | ::: block             |
        |                       |                       | If you add or remove  |
        |                       |                       | resource types above  |
        |                       |                       | please make sure you  |
        |                       |                       | update the number     |
        |                       |                       | below.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `ResourceAmounts()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                       Description
          -------------------------- ------------------------------------------------------------ -------------
          `boolean`                  `allValuesLessThanOrEqual​(ResourceAmounts amounts)`           
          `ResourceAmounts`          `append​(ResourceAmounts amounts)`                             
          `boolean`                  `containsValuesLessThan​(ResourceAmounts amounts)`             
          `abstract int`             `getCpu()`                                                    
          `abstract int`             `getDiskIO()`                                                 
          `abstract int`             `getMemory()`                                                 
          `abstract int`             `getNetworkIO()`                                              
          `static ResourceAmounts`   `of()`                                                        
          `static ResourceAmounts`   `of​(int cpu,   int memory,   int diskIO,   int networkIO)`    
          `ResourceAmounts`          `subtract​(ResourceAmounts amounts)`                           
          `static ResourceAmounts`   `zero()`                                                      

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

        []{#RESOURCE_TYPE_COUNT}

        -   #### RESOURCE_TYPE_COUNT

                public static final int RESOURCE_TYPE_COUNT

            ::: block
            If you add or remove resource types above please make sure
            you update the number below.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.concurrent.ResourceAmounts.RESOURCE_TYPE_COUNT)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ResourceAmounts

                public ResourceAmounts()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCpu()}

        -   #### getCpu

            ``` methodSignature
            public abstract int getCpu()
            ```

        []{#getMemory()}

        -   #### getMemory

            ``` methodSignature
            public abstract int getMemory()
            ```

        []{#getDiskIO()}

        -   #### getDiskIO

            ``` methodSignature
            public abstract int getDiskIO()
            ```

        []{#getNetworkIO()}

        -   #### getNetworkIO

            ``` methodSignature
            public abstract int getNetworkIO()
            ```

        []{#zero()}

        -   #### zero

            ``` methodSignature
            public static ResourceAmounts zero()
            ```

        []{#of()}

        -   #### of

            ``` methodSignature
            public static ResourceAmounts of()
            ```

        []{#of(int,int,int,int)}

        -   #### of

            ``` methodSignature
            public static ResourceAmounts of​(int cpu,
                                             int memory,
                                             int diskIO,
                                             int networkIO)
            ```

        []{#append(com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### append

            ``` methodSignature
            public ResourceAmounts append​(ResourceAmounts amounts)
            ```

        []{#subtract(com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### subtract

            ``` methodSignature
            public ResourceAmounts subtract​(ResourceAmounts amounts)
            ```

        []{#containsValuesLessThan(com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### containsValuesLessThan

            ``` methodSignature
            public boolean containsValuesLessThan​(ResourceAmounts amounts)
            ```

        []{#allValuesLessThanOrEqual(com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### allValuesLessThanOrEqual

            ``` methodSignature
            public boolean allValuesLessThanOrEqual​(ResourceAmounts amounts)
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
-   Nested \| 
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
