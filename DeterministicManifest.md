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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip](package-summary.html)
:::

## Class DeterministicManifest {#class-deterministicmanifest .title title="Class DeterministicManifest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.util.jar.Manifest](http://docs.oracle.com/javase/7/docs/api/java/util/jar/Manifest.html?is-external=true "class or interface in java.util.jar"){.externalLink}

    -   -   com.facebook.buck.util.zip.DeterministicManifest

::: description
-   

    All Implemented Interfaces:
    :   `Cloneable`

    ------------------------------------------------------------------------

        public class DeterministicManifest
        extends Manifest

    ::: block
    A manifest implementation whose formatted output is deterministic
    given the same input (entries and attributes are sorted). The JDK
    implementation in `java.util.Manifest` does not have this property.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                               Description
          ----------------------------------------- -------------
          `DeterministicManifest()`                  
          `DeterministicManifest​(InputStream is)`    
          `DeterministicManifest​(Manifest man)`      

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                              Description
          ------------------- --------------------------------------------------------------------------------------------------- -------------
          `boolean`           `hasEntries()`                                                                                       
          `void`              `setEntryAttribute​(String entryName,                  String key,                  String value)`    
          `void`              `setManifestAttribute​(String key,                     String value)`                                 
          `void`              `write​(OutputStream out)`                                                                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.util.jar.Manifest}

            ### Methods inherited from class java.util.jar.[Manifest](http://docs.oracle.com/javase/7/docs/api/java/util/jar/Manifest.html?is-external=true "class or interface in java.util.jar"){.externalLink}

            `clear, clone, equals, getAttributes, getEntries, getMainAttributes, hashCode, read`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### DeterministicManifest

                public DeterministicManifest()

        []{#<init>(java.io.InputStream)}

        -   #### DeterministicManifest

                public DeterministicManifest​(InputStream is)
                                      throws IOException

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#<init>(java.util.jar.Manifest)}

        -   #### DeterministicManifest

                public DeterministicManifest​(Manifest man)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setEntryAttribute(java.lang.String,java.lang.String,java.lang.String)}

        -   #### setEntryAttribute

            ``` methodSignature
            public void setEntryAttribute​(String entryName,
                                          String key,
                                          String value)
            ```

        []{#setManifestAttribute(java.lang.String,java.lang.String)}

        -   #### setManifestAttribute

            ``` methodSignature
            public void setManifestAttribute​(String key,
                                             String value)
            ```

        []{#hasEntries()}

        -   #### hasEntries

            ``` methodSignature
            public boolean hasEntries()
            ```

        []{#write(java.io.OutputStream)}

        -   #### write

            ``` methodSignature
            public void write​(OutputStream out)
                       throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `write` in class `Manifest`

            [Throws:]{.throwsLabel}
            :   `IOException`
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
