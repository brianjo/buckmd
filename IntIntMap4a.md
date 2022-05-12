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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.objectfile](package-summary.html)
:::

## Class IntIntMap4a {#class-intintmap4a .title title="Class IntIntMap4a"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.objectfile.IntIntMap4a

::: description
-   

    All Implemented Interfaces:
    :   `IntIntMap`

    ------------------------------------------------------------------------

        public class IntIntMap4a
        extends Object
        implements IntIntMap

    ::: block
    An extremely fast int-int map for large data sets which avoids
    boxing costs. Original source from
    https://github.com/mikvor/hashmapTest. For performance information,
    see
    http://java-performance.info/implementing-world-fastest-java-int-to-int-hash-map/
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                          Description
          ------------------------------------------------------------------------------------ -------------
          `IntIntMap4a​(int size,            float fillFactor,            int noValueMarker)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                         Description
          ------------------- ------------------------------ -------------
          `int`               `get​(int key)`                  
          `int`               `put​(int key,    int value)`    
          `int`               `remove​(int key)`               
          `int`               `size()`                        

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

        []{#<init>(int,float,int)}

        -   #### IntIntMap4a

                public IntIntMap4a​(int size,
                                   float fillFactor,
                                   int noValueMarker)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(int)}

        -   #### get

            ``` methodSignature
            public int get​(int key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `IntIntMap`

        []{#put(int,int)}

        -   #### put

            ``` methodSignature
            public int put​(int key,
                           int value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in interface `IntIntMap`

        []{#remove(int)}

        -   #### remove

            ``` methodSignature
            public int remove​(int key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `remove` in interface `IntIntMap`

        []{#size()}

        -   #### size

            ``` methodSignature
            public int size()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `size` in interface `IntIntMap`
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
