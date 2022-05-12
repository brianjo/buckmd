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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.compatible](package-summary.html)
:::

## Class BuckStarlarkStructObject {#class-buckstarlarkstructobject .title title="Class BuckStarlarkStructObject"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject

::: description
-   

    All Implemented Interfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BuiltInProviderInfo`

    ------------------------------------------------------------------------

        public abstract class BuckStarlarkStructObject
        extends Object
        implements com.google.devtools.build.lib.syntax.ClassObject, com.google.devtools.build.lib.skylarkinterface.SkylarkValue

    ::: block
    Marks a Java object as accessible by Skylark as a struct-like object
    called `ClassObject`. This also marks it as a `SkylarkValue`.
    A struct like object is an object containing fields accessible via
    the dot syntax, like `  obj.field`.

    We currently do not support method calls.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `BuckStarlarkStructObject()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                                                                          Description
          ------------------------------------------------------------------- ------------------------------------------------------------------------------- -------------
          `protected abstract Class<?>`                                       `getDeclaredClass()`                                                             
          `String`                                                            `getErrorMessageForUnknownField​(String field)`                                   
          `com.google.common.collect.ImmutableCollection<String>`             `getFieldNames()`                                                                
          `protected com.google.common.collect.ImmutableMap<String,​Method>`   `getMethods()`                                                                   
          `Object`                                                            `getValue​(String name)`                                                          
          `void`                                                              `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable, isImmutable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuckStarlarkStructObject

                public BuckStarlarkStructObject()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValue(java.lang.String)}

        -   #### getValue

            ``` methodSignature
            @Nullable
            public Object getValue​(String name)
                            throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValue` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#getMethods()}

        -   #### getMethods

            ``` methodSignature
            protected com.google.common.collect.ImmutableMap<String,​Method> getMethods()
            ```

        []{#getDeclaredClass()}

        -   #### getDeclaredClass

            ``` methodSignature
            protected abstract Class<?> getDeclaredClass()
            ```

            [Returns:]{.returnLabel}
            :   the class for which all declared methods on it are
                considered skylark accessible.

        []{#getFieldNames()}

        -   #### getFieldNames

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<String> getFieldNames()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFieldNames` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

        []{#getErrorMessageForUnknownField(java.lang.String)}

        -   #### getErrorMessageForUnknownField

            ``` methodSignature
            @Nullable
            public String getErrorMessageForUnknownField​(String field)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getErrorMessageForUnknownField` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`
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
