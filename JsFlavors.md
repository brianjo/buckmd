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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Class JsFlavors {#class-jsflavors .title title="Class JsFlavors"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.js.JsFlavors

::: description
-   

    ------------------------------------------------------------------------

        public class JsFlavors
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type               Field                     Description
          ------------------------------- ------------------------- -------------
          `static UserFlavor`             `ANDROID`                  
          `static InternalFlavor`         `ANDROID_RESOURCES`        
          `static UserFlavor`             `DEPENDENCY_FILE`          
          `static InternalFlavor`         `FORCE_JS_BUNDLE`          
          `static UserFlavor`             `IOS`                      
          `static InternalFlavor`         `LIBRARY_FILES`            
          `static UserFlavor`             `MISC`                     
          `static FlavorDomain<String>`   `OPTIMIZATION_DOMAIN`      
          `static FlavorDomain<Object>`   `OUTPUT_OPTIONS_DOMAIN`    
          `static FlavorDomain<String>`   `PLATFORM_DOMAIN`          
          `static FlavorDomain<String>`   `RAM_BUNDLE_DOMAIN`        
          `static UserFlavor`             `RAM_BUNDLE_FILES`         
          `static UserFlavor`             `RAM_BUNDLE_INDEXED`       
          `static UserFlavor`             `RELEASE`                  
          `static UserFlavor`             `SOURCE_MAP`               

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method                                                                                                                                                                                        Description
          --------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static String`                                                 `bundleJobArgs​(Set<Flavor> flavors)`                                                                                                                                                           
          `static Optional<Either<SourcePath,​Pair<SourcePath,​String>>>`   `extractSourcePath​(com.google.common.collect.ImmutableBiMap<Flavor,​Either<SourcePath,​Pair<SourcePath,​String>>> flavorsToSources,                  java.util.stream.Stream<Flavor> flavors)`    
          `static Flavor`                                                 `fileFlavorForSourcePath​(Path path)`                                                                                                                                                           
          `static boolean`                                                `isFileFlavor​(Flavor flavor)`                                                                                                                                                                  
          `static String`                                                 `platformArgForRelease​(Set<Flavor> flavors)`                                                                                                                                                   
          `static boolean`                                                `validateFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors,                Iterable<FlavorDomain<?>> allowableDomains)`                                                           

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
    -   []{#field.detail}

        ### Field Detail

        []{#ANDROID}

        -   #### ANDROID

                public static final UserFlavor ANDROID

        []{#IOS}

        -   #### IOS

                public static final UserFlavor IOS

        []{#RELEASE}

        -   #### RELEASE

                public static final UserFlavor RELEASE

        []{#RAM_BUNDLE_FILES}

        -   #### RAM_BUNDLE_FILES

                public static final UserFlavor RAM_BUNDLE_FILES

        []{#RAM_BUNDLE_INDEXED}

        -   #### RAM_BUNDLE_INDEXED

                public static final UserFlavor RAM_BUNDLE_INDEXED

        []{#SOURCE_MAP}

        -   #### SOURCE_MAP

                public static final UserFlavor SOURCE_MAP

        []{#MISC}

        -   #### MISC

                public static final UserFlavor MISC

        []{#DEPENDENCY_FILE}

        -   #### DEPENDENCY_FILE

                public static final UserFlavor DEPENDENCY_FILE

        []{#OPTIMIZATION_DOMAIN}

        -   #### OPTIMIZATION_DOMAIN

                public static final FlavorDomain<String> OPTIMIZATION_DOMAIN

        []{#PLATFORM_DOMAIN}

        -   #### PLATFORM_DOMAIN

                public static final FlavorDomain<String> PLATFORM_DOMAIN

        []{#RAM_BUNDLE_DOMAIN}

        -   #### RAM_BUNDLE_DOMAIN

                public static final FlavorDomain<String> RAM_BUNDLE_DOMAIN

        []{#OUTPUT_OPTIONS_DOMAIN}

        -   #### OUTPUT_OPTIONS_DOMAIN

                public static final FlavorDomain<Object> OUTPUT_OPTIONS_DOMAIN

        []{#ANDROID_RESOURCES}

        -   #### ANDROID_RESOURCES

                public static final InternalFlavor ANDROID_RESOURCES

        []{#FORCE_JS_BUNDLE}

        -   #### FORCE_JS_BUNDLE

                public static final InternalFlavor FORCE_JS_BUNDLE

        []{#LIBRARY_FILES}

        -   #### LIBRARY_FILES

                public static final InternalFlavor LIBRARY_FILES
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#validateFlavors(com.google.common.collect.ImmutableSet,java.lang.Iterable)}

        -   #### validateFlavors

            ``` methodSignature
            public static boolean validateFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors,
                                                  Iterable<FlavorDomain<?>> allowableDomains)
            ```

        []{#fileFlavorForSourcePath(java.nio.file.Path)}

        -   #### fileFlavorForSourcePath

            ``` methodSignature
            public static Flavor fileFlavorForSourcePath​(Path path)
            ```

        []{#extractSourcePath(com.google.common.collect.ImmutableBiMap,java.util.stream.Stream)}

        -   #### extractSourcePath

            ``` methodSignature
            public static Optional<Either<SourcePath,​Pair<SourcePath,​String>>> extractSourcePath​(com.google.common.collect.ImmutableBiMap<Flavor,​Either<SourcePath,​Pair<SourcePath,​String>>> flavorsToSources,
                                                                                                             java.util.stream.Stream<Flavor> flavors)
            ```

        []{#isFileFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### isFileFlavor

            ``` methodSignature
            public static boolean isFileFlavor​(Flavor flavor)
            ```

        []{#bundleJobArgs(java.util.Set)}

        -   #### bundleJobArgs

            ``` methodSignature
            public static String bundleJobArgs​(Set<Flavor> flavors)
            ```

        []{#platformArgForRelease(java.util.Set)}

        -   #### platformArgForRelease

            ``` methodSignature
            public static String platformArgForRelease​(Set<Flavor> flavors)
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
