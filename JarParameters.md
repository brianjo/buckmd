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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JarParameters {#class-jarparameters .title title="Class JarParameters"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JarParameters

::: description
-   

    ------------------------------------------------------------------------

        public abstract class JarParameters
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                     Description
          ------------------- ------------------------- -------------
          `static class `     `JarParameters.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `JarParameters()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method                         Description
          --------------------------------------------------------------- ------------------------------ -------------
          `static JarParameters.Builder`                                  `builder()`                     
          `boolean`                                                       `getDisallowAllDuplicates()`    
          `Level`                                                         `getDuplicatesLogLevel()`       
          `abstract com.google.common.collect.ImmutableSortedSet<Path>`   `getEntriesToJar()`             
          `boolean`                                                       `getHashEntries()`              
          `abstract Path`                                                 `getJarPath()`                  
          `abstract Optional<String>`                                     `getMainClass()`                
          `abstract Optional<Path>`                                       `getManifestFile()`             
          `boolean`                                                       `getMergeManifests()`           
          `java.util.function.Predicate<Object>`                          `getRemoveEntryPredicate()`     

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### JarParameters

                public JarParameters()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHashEntries()}

        -   #### getHashEntries

            ``` methodSignature
            @Default
            public boolean getHashEntries()
            ```

        []{#getMergeManifests()}

        -   #### getMergeManifests

            ``` methodSignature
            @Default
            public boolean getMergeManifests()
            ```

        []{#getDisallowAllDuplicates()}

        -   #### getDisallowAllDuplicates

            ``` methodSignature
            @Default
            public boolean getDisallowAllDuplicates()
            ```

        []{#getJarPath()}

        -   #### getJarPath

            ``` methodSignature
            public abstract Path getJarPath()
            ```

        []{#getRemoveEntryPredicate()}

        -   #### getRemoveEntryPredicate

            ``` methodSignature
            @Default
            public java.util.function.Predicate<Object> getRemoveEntryPredicate()
            ```

        []{#getEntriesToJar()}

        -   #### getEntriesToJar

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedSet<Path> getEntriesToJar()
            ```

        []{#getMainClass()}

        -   #### getMainClass

            ``` methodSignature
            public abstract Optional<String> getMainClass()
            ```

        []{#getManifestFile()}

        -   #### getManifestFile

            ``` methodSignature
            public abstract Optional<Path> getManifestFile()
            ```

        []{#getDuplicatesLogLevel()}

        -   #### getDuplicatesLogLevel

            ``` methodSignature
            @Default
            public Level getDuplicatesLogLevel()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static JarParameters.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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
