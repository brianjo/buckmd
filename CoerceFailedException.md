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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class CoerceFailedException {#class-coercefailedexception .title title="Class CoerceFailedException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   com.facebook.buck.rules.coercer.CoerceFailedException

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`

    ------------------------------------------------------------------------

        public class CoerceFailedException
        extends Exception

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.rules.coercer.CoerceFailedException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                     Description
          ------------------------------------------------------------------------------- -------------
          `CoerceFailedException​(String message)`                                          
          `CoerceFailedException​(String message,                      Throwable cause)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                                                  Description
          -------------------------------- ------------------------------------------------------------------------------------------------------- -------------
          `static CoerceFailedException`   `simple​(Object object,       com.google.common.reflect.TypeToken<?> resultType)`                         
          `static CoerceFailedException`   `simple​(Object object,       com.google.common.reflect.TypeToken<?> resultType,       String detail)`    
          `static CoerceFailedException`   `simple​(Object object,       Type resultType)`                                                           
          `static CoerceFailedException`   `simple​(Object object,       Type resultType,       String detail)`                                      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Throwable}

            ### Methods inherited from class java.lang.[Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `addSuppressed, fillInStackTrace, getCause, getLocalizedMessage, getMessage, getStackTrace, getSuppressed, initCause, printStackTrace, printStackTrace, printStackTrace, setStackTrace, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String)}

        -   #### CoerceFailedException

                public CoerceFailedException​(String message)

        []{#<init>(java.lang.String,java.lang.Throwable)}

        -   #### CoerceFailedException

                public CoerceFailedException​(String message,
                                             Throwable cause)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#simple(java.lang.Object,java.lang.reflect.Type)}

        -   #### simple

            ``` methodSignature
            public static CoerceFailedException simple​(Object object,
                                                       Type resultType)
            ```

        []{#simple(java.lang.Object,com.google.common.reflect.TypeToken)}

        -   #### simple

            ``` methodSignature
            public static CoerceFailedException simple​(Object object,
                                                       com.google.common.reflect.TypeToken<?> resultType)
            ```

        []{#simple(java.lang.Object,java.lang.reflect.Type,java.lang.String)}

        -   #### simple

            ``` methodSignature
            public static CoerceFailedException simple​(Object object,
                                                       Type resultType,
                                                       String detail)
            ```

        []{#simple(java.lang.Object,com.google.common.reflect.TypeToken,java.lang.String)}

        -   #### simple

            ``` methodSignature
            public static CoerceFailedException simple​(Object object,
                                                       com.google.common.reflect.TypeToken<?> resultType,
                                                       String detail)
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
