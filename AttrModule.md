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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.function.attr](package-summary.html)
:::

## Class AttrModule {#class-attrmodule .title title="Class AttrModule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.function.attr.AttrModule

::: description
-   

    All Implemented Interfaces:
    :   `AttrModuleApi`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ------------------------------------------------------------------------

        public class AttrModule
        extends Object
        implements AttrModuleApi

    ::: block
    Class that actually instantiates Attribute objects for user defined
    rules
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `AttrModule()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                  Description
          ------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AttributeHolder`   `boolAttribute​(boolean defaultValue,              String doc,              boolean mandatory)`                                                                                                                                                                                           
          `AttributeHolder`   `depAttribute​(Object defaultValue,             String doc,             boolean mandatory,             com.google.devtools.build.lib.syntax.SkylarkList<Provider<?>> providers)`                                                                                                          
          `AttributeHolder`   `depListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,                 String doc,                 boolean mandatory,                 boolean allowEmpty,                 com.google.devtools.build.lib.syntax.SkylarkList<Provider<?>> providers)`    
          `AttributeHolder`   `intAttribute​(Integer defaultValue,             String doc,             Boolean mandatory,             com.google.devtools.build.lib.syntax.SkylarkList<Integer> values)`                                                                                                                
          `AttributeHolder`   `intListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<Integer> defaultValue,                 String doc,                 boolean mandatory,                 boolean allowEmpty)`                                                                                            
          `AttributeHolder`   `outputAttribute​(Object defaultValue,                String doc,                boolean mandatory,                com.google.devtools.build.lib.events.Location location)`                                                                                                               
          `AttributeHolder`   `outputListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,                    String doc,                    boolean mandatory,                    boolean allowEmpty)`                                                                                 
          `void`              `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`                                                                                                                                                                                                            
          `AttributeHolder`   `sourceAttribute​(Object defaultValue,                String doc,                boolean mandatory)`                                                                                                                                                                                      
          `AttributeHolder`   `sourceListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,                    String doc,                    boolean mandatory,                    boolean allowEmpty)`                                                                                 
          `AttributeHolder`   `stringAttribute​(String defaultValue,                String doc,                Boolean mandatory,                com.google.devtools.build.lib.syntax.SkylarkList<String> values)`                                                                                                      
          `AttributeHolder`   `stringListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,                    String doc,                    boolean mandatory,                    boolean allowEmpty)`                                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        -   #### AttrModule

                public AttrModule()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`

        []{#intAttribute(java.lang.Integer,java.lang.String,java.lang.Boolean,com.google.devtools.build.lib.syntax.SkylarkList)}

        -   #### intAttribute

            ``` methodSignature
            public AttributeHolder intAttribute​(Integer defaultValue,
                                                String doc,
                                                Boolean mandatory,
                                                com.google.devtools.build.lib.syntax.SkylarkList<Integer> values)
                                         throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `intAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#intListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean)}

        -   #### intListAttribute

            ``` methodSignature
            public AttributeHolder intListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<Integer> defaultValue,
                                                    String doc,
                                                    boolean mandatory,
                                                    boolean allowEmpty)
                                             throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `intListAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#stringAttribute(java.lang.String,java.lang.String,java.lang.Boolean,com.google.devtools.build.lib.syntax.SkylarkList)}

        -   #### stringAttribute

            ``` methodSignature
            public AttributeHolder stringAttribute​(String defaultValue,
                                                   String doc,
                                                   Boolean mandatory,
                                                   com.google.devtools.build.lib.syntax.SkylarkList<String> values)
                                            throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `stringAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#stringListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean)}

        -   #### stringListAttribute

            ``` methodSignature
            public AttributeHolder stringListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,
                                                       String doc,
                                                       boolean mandatory,
                                                       boolean allowEmpty)
                                                throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `stringListAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#boolAttribute(boolean,java.lang.String,boolean)}

        -   #### boolAttribute

            ``` methodSignature
            public AttributeHolder boolAttribute​(boolean defaultValue,
                                                 String doc,
                                                 boolean mandatory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `boolAttribute` in interface `AttrModuleApi`

        []{#sourceListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean)}

        -   #### sourceListAttribute

            ``` methodSignature
            public AttributeHolder sourceListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,
                                                       String doc,
                                                       boolean mandatory,
                                                       boolean allowEmpty)
                                                throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `sourceListAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#sourceAttribute(java.lang.Object,java.lang.String,boolean)}

        -   #### sourceAttribute

            ``` methodSignature
            public AttributeHolder sourceAttribute​(Object defaultValue,
                                                   String doc,
                                                   boolean mandatory)
                                            throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `sourceAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#depAttribute(java.lang.Object,java.lang.String,boolean,com.google.devtools.build.lib.syntax.SkylarkList)}

        -   #### depAttribute

            ``` methodSignature
            public AttributeHolder depAttribute​(Object defaultValue,
                                                String doc,
                                                boolean mandatory,
                                                com.google.devtools.build.lib.syntax.SkylarkList<Provider<?>> providers)
                                         throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `depAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#depListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean,com.google.devtools.build.lib.syntax.SkylarkList)}

        -   #### depListAttribute

            ``` methodSignature
            public AttributeHolder depListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,
                                                    String doc,
                                                    boolean mandatory,
                                                    boolean allowEmpty,
                                                    com.google.devtools.build.lib.syntax.SkylarkList<Provider<?>> providers)
                                             throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `depListAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#outputAttribute(java.lang.Object,java.lang.String,boolean,com.google.devtools.build.lib.events.Location)}

        -   #### outputAttribute

            ``` methodSignature
            public AttributeHolder outputAttribute​(Object defaultValue,
                                                   String doc,
                                                   boolean mandatory,
                                                   com.google.devtools.build.lib.events.Location location)
                                            throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `outputAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#outputListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean)}

        -   #### outputListAttribute

            ``` methodSignature
            public AttributeHolder outputListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,
                                                       String doc,
                                                       boolean mandatory,
                                                       boolean allowEmpty)
                                                throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `outputListAttribute` in interface `AttrModuleApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
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
