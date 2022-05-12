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
[Package]{.packageLabelInType} [com.facebook.buck.android.aapt](package-summary.html)
:::

## Class RDotTxtResourceCollector {#class-rdottxtresourcecollector .title title="Class RDotTxtResourceCollector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.aapt.RDotTxtResourceCollector

::: description
-   

    ------------------------------------------------------------------------

        public class RDotTxtResourceCollector
        extends Object

    ::: block
    Responsible for collecting resources parsed by
    [`MiniAapt`](MiniAapt.html "class in com.facebook.buck.android.aapt")
    and assigning unique integer ids to those resources. Resource ids
    are of the type `0x7fxxyyyy`, where `xx` represents the resource
    type, and `yyyy` represents the id within that resource type.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `RDotTxtResourceCollector()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method                                                                                                                                                                                                                                                                                                                           Description
          --------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                `addCustomDrawableResourceIfNotPresent​(RDotTxtEntry.RType rType,                                      String name,                                      Path path,                                      DocumentLocation documentLocation,                                      RDotTxtEntry.CustomDrawableType drawableType)`    
          `void`                `addIntArrayResourceIfNotPresent​(RDotTxtEntry.RType rType,                                String name,                                int numValues,                                Path path,                                DocumentLocation documentLocation)`                                                                 
          `void`                `addIntResourceIfNotPresent​(RDotTxtEntry.RType rType,                           String name,                           Path path,                           DocumentLocation documentLocation)`                                                                                                                                   
          `void`                `addResource​(RDotTxtEntry.RType rType,            RDotTxtEntry.IdType idType,            String name,            String idValue,            String parent,            Path path,            DocumentLocation documentLocation)`                                                                                                   
          `Set<RDotTxtEntry>`   `getResources()`                                                                                                                                                                                                                                                                                                                  

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

        []{#<init>()}

        -   #### RDotTxtResourceCollector

                public RDotTxtResourceCollector()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addIntResourceIfNotPresent(com.facebook.buck.android.aapt.RDotTxtEntry.RType,java.lang.String,java.nio.file.Path,com.facebook.buck.util.xml.DocumentLocation)}

        -   #### addIntResourceIfNotPresent

            ``` methodSignature
            public void addIntResourceIfNotPresent​(RDotTxtEntry.RType rType,
                                                   String name,
                                                   Path path,
                                                   DocumentLocation documentLocation)
            ```

        []{#addCustomDrawableResourceIfNotPresent(com.facebook.buck.android.aapt.RDotTxtEntry.RType,java.lang.String,java.nio.file.Path,com.facebook.buck.util.xml.DocumentLocation,com.facebook.buck.android.aapt.RDotTxtEntry.CustomDrawableType)}

        -   #### addCustomDrawableResourceIfNotPresent

            ``` methodSignature
            public void addCustomDrawableResourceIfNotPresent​(RDotTxtEntry.RType rType,
                                                              String name,
                                                              Path path,
                                                              DocumentLocation documentLocation,
                                                              RDotTxtEntry.CustomDrawableType drawableType)
            ```

        []{#addIntArrayResourceIfNotPresent(com.facebook.buck.android.aapt.RDotTxtEntry.RType,java.lang.String,int,java.nio.file.Path,com.facebook.buck.util.xml.DocumentLocation)}

        -   #### addIntArrayResourceIfNotPresent

            ``` methodSignature
            public void addIntArrayResourceIfNotPresent​(RDotTxtEntry.RType rType,
                                                        String name,
                                                        int numValues,
                                                        Path path,
                                                        DocumentLocation documentLocation)
            ```

        []{#addResource(com.facebook.buck.android.aapt.RDotTxtEntry.RType,com.facebook.buck.android.aapt.RDotTxtEntry.IdType,java.lang.String,java.lang.String,java.lang.String,java.nio.file.Path,com.facebook.buck.util.xml.DocumentLocation)}

        -   #### addResource

            ``` methodSignature
            public void addResource​(RDotTxtEntry.RType rType,
                                    RDotTxtEntry.IdType idType,
                                    String name,
                                    String idValue,
                                    @Nullable
                                    String parent,
                                    Path path,
                                    DocumentLocation documentLocation)
            ```

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            public Set<RDotTxtEntry> getResources()
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
