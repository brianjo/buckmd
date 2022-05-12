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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.function.attr](package-summary.html)
:::

## Interface AttrModuleApi {#interface-attrmoduleapi .title title="Interface AttrModuleApi"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AttrModule`

    ------------------------------------------------------------------------

        public interface AttrModuleApi
        extends com.google.devtools.build.lib.skylarkinterface.SkylarkValue

    ::: block
    Skylark module used to configure the attribute schema for user
    defined rules
    :::
:::

::: summary
-   ::: {.section role="region"}
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
          `AttributeHolder`   `sourceAttribute​(Object defaultValue,                String doc,                boolean mandatory)`                                                                                                                                                                                      
          `AttributeHolder`   `sourceListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,                    String doc,                    boolean mandatory,                    boolean allowEmpty)`                                                                                 
          `AttributeHolder`   `stringAttribute​(String defaultValue,                String doc,                Boolean mandatory,                com.google.devtools.build.lib.syntax.SkylarkList<String> values)`                                                                                                      
          `AttributeHolder`   `stringListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,                    String doc,                    boolean mandatory,                    boolean allowEmpty)`                                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, repr, str`

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
    -   []{#method.detail}

        ### Method Detail

        []{#intAttribute(java.lang.Integer,java.lang.String,java.lang.Boolean,com.google.devtools.build.lib.syntax.SkylarkList)}

        -   #### intAttribute

            ``` methodSignature
            AttributeHolder intAttribute​(Integer defaultValue,
                                         String doc,
                                         Boolean mandatory,
                                         com.google.devtools.build.lib.syntax.SkylarkList<Integer> values)
                                  throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#intListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean)}

        -   #### intListAttribute

            ``` methodSignature
            AttributeHolder intListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<Integer> defaultValue,
                                             String doc,
                                             boolean mandatory,
                                             boolean allowEmpty)
                                      throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#stringAttribute(java.lang.String,java.lang.String,java.lang.Boolean,com.google.devtools.build.lib.syntax.SkylarkList)}

        -   #### stringAttribute

            ``` methodSignature
            AttributeHolder stringAttribute​(String defaultValue,
                                            String doc,
                                            Boolean mandatory,
                                            com.google.devtools.build.lib.syntax.SkylarkList<String> values)
                                     throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#stringListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean)}

        -   #### stringListAttribute

            ``` methodSignature
            AttributeHolder stringListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,
                                                String doc,
                                                boolean mandatory,
                                                boolean allowEmpty)
                                         throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#boolAttribute(boolean,java.lang.String,boolean)}

        -   #### boolAttribute

            ``` methodSignature
            AttributeHolder boolAttribute​(boolean defaultValue,
                                          String doc,
                                          boolean mandatory)
                                   throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#sourceListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean)}

        -   #### sourceListAttribute

            ``` methodSignature
            AttributeHolder sourceListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,
                                                String doc,
                                                boolean mandatory,
                                                boolean allowEmpty)
                                         throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#sourceAttribute(java.lang.Object,java.lang.String,boolean)}

        -   #### sourceAttribute

            ``` methodSignature
            AttributeHolder sourceAttribute​(Object defaultValue,
                                            String doc,
                                            boolean mandatory)
                                     throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#depAttribute(java.lang.Object,java.lang.String,boolean,com.google.devtools.build.lib.syntax.SkylarkList)}

        -   #### depAttribute

            ``` methodSignature
            AttributeHolder depAttribute​(Object defaultValue,
                                         String doc,
                                         boolean mandatory,
                                         com.google.devtools.build.lib.syntax.SkylarkList<Provider<?>> providers)
                                  throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#depListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean,com.google.devtools.build.lib.syntax.SkylarkList)}

        -   #### depListAttribute

            ``` methodSignature
            AttributeHolder depListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,
                                             String doc,
                                             boolean mandatory,
                                             boolean allowEmpty,
                                             com.google.devtools.build.lib.syntax.SkylarkList<Provider<?>> providers)
                                      throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#outputAttribute(java.lang.Object,java.lang.String,boolean,com.google.devtools.build.lib.events.Location)}

        -   #### outputAttribute

            ``` methodSignature
            AttributeHolder outputAttribute​(Object defaultValue,
                                            String doc,
                                            boolean mandatory,
                                            com.google.devtools.build.lib.events.Location location)
                                     throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#outputListAttribute(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,boolean,boolean)}

        -   #### outputListAttribute

            ``` methodSignature
            AttributeHolder outputListAttribute​(com.google.devtools.build.lib.syntax.SkylarkList<String> defaultValue,
                                                String doc,
                                                boolean mandatory,
                                                boolean allowEmpty)
                                         throws com.google.devtools.build.lib.syntax.EvalException
            ```

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