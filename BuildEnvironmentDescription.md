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
[Package]{.packageLabelInType} [com.facebook.buck.util.environment](package-summary.html)
:::

## Class BuildEnvironmentDescription {#class-buildenvironmentdescription .title title="Class BuildEnvironmentDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.environment.BuildEnvironmentDescription

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuildEnvironmentDescription
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                Description
          ------------------- -------------------- -------------
          `static int`        `PROTOCOL_VERSION`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                       Description
          --------------------------------- -------------
          `BuildEnvironmentDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method                                                                                                                                                                                                                                                                                                                                                   Description
          ------------------------------------------------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract int`                                                     `getAvailableCores()`                                                                                                                                                                                                                                                                                                                                     
          `abstract String`                                                  `getBuckCommit()`                                                                                                                                                                                                                                                                                                                                         
          `abstract Optional<Boolean>`                                       `getBuckDirty()`                                                                                                                                                                                                                                                                                                                                          
          `String`                                                           `getBuildType()`                                                                                                                                                                                                                                                                                                                                          
          `abstract com.google.common.collect.ImmutableList<String>`         `getCacheModes()`                                                                                                                                                                                                                                                                                                                                         
          `abstract com.google.common.collect.ImmutableMap<String,​String>`   `getExtraData()`                                                                                                                                                                                                                                                                                                                                          
          `abstract String`                                                  `getHostname()`                                                                                                                                                                                                                                                                                                                                           
          `abstract String`                                                  `getJavaVersion()`                                                                                                                                                                                                                                                                                                                                        
          `int`                                                              `getJsonProtocolVersion()`                                                                                                                                                                                                                                                                                                                                
          `abstract String`                                                  `getOs()`                                                                                                                                                                                                                                                                                                                                                 
          `abstract long`                                                    `getSystemMemory()`                                                                                                                                                                                                                                                                                                                                       
          `abstract String`                                                  `getUser()`                                                                                                                                                                                                                                                                                                                                               
          `static BuildEnvironmentDescription`                               `of​(ExecutionEnvironment executionEnvironment,   com.google.common.collect.ImmutableList<String> cacheModes,   com.google.common.collect.ImmutableMap<String,​String> extraData)`                                                                                                                                                                          
          `static BuildEnvironmentDescription`                               `of​(String user,   String hostname,   String os,   int availableCores,   long systemMemory,   Optional<Boolean> buckDirty,   String buckCommit,   String javaVersion,   int jsonProtocolVersion)`                                                                                                                                                         
          `static BuildEnvironmentDescription`                               `of​(String user,   String hostname,   String os,   int availableCores,   long systemMemory,   Optional<Boolean> buckDirty,   String buckCommit,   String javaVersion,   com.google.common.collect.ImmutableList<String> cacheModes,   com.google.common.collect.ImmutableMap<String,​String> extraData)`                                                   
          `static BuildEnvironmentDescription`                               `of​(String user,   String hostname,   String os,   int availableCores,   long systemMemory,   Optional<Boolean> buckDirty,   String buckCommit,   String javaVersion,   com.google.common.collect.ImmutableList<String> cacheModes,   com.google.common.collect.ImmutableMap<String,​String> extraData,   int jsonProtocolVersion,   String buildType)`    

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

        []{#PROTOCOL_VERSION}

        -   #### PROTOCOL_VERSION

                public static final int PROTOCOL_VERSION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.environment.BuildEnvironmentDescription.PROTOCOL_VERSION)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildEnvironmentDescription

                public BuildEnvironmentDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUser()}

        -   #### getUser

            ``` methodSignature
            public abstract String getUser()
            ```

        []{#getHostname()}

        -   #### getHostname

            ``` methodSignature
            public abstract String getHostname()
            ```

        []{#getOs()}

        -   #### getOs

            ``` methodSignature
            public abstract String getOs()
            ```

        []{#getAvailableCores()}

        -   #### getAvailableCores

            ``` methodSignature
            public abstract int getAvailableCores()
            ```

        []{#getSystemMemory()}

        -   #### getSystemMemory

            ``` methodSignature
            public abstract long getSystemMemory()
            ```

        []{#getBuckDirty()}

        -   #### getBuckDirty

            ``` methodSignature
            public abstract Optional<Boolean> getBuckDirty()
            ```

        []{#getBuckCommit()}

        -   #### getBuckCommit

            ``` methodSignature
            public abstract String getBuckCommit()
            ```

        []{#getJavaVersion()}

        -   #### getJavaVersion

            ``` methodSignature
            public abstract String getJavaVersion()
            ```

        []{#getCacheModes()}

        -   #### getCacheModes

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getCacheModes()
            ```

        []{#getExtraData()}

        -   #### getExtraData

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getExtraData()
            ```

        []{#getJsonProtocolVersion()}

        -   #### getJsonProtocolVersion

            ``` methodSignature
            @Default
            public int getJsonProtocolVersion()
            ```

        []{#getBuildType()}

        -   #### getBuildType

            ``` methodSignature
            @Default
            public String getBuildType()
            ```

        []{#of(com.facebook.buck.util.environment.ExecutionEnvironment,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap)}

        -   #### of

            ``` methodSignature
            public static BuildEnvironmentDescription of​(ExecutionEnvironment executionEnvironment,
                                                         com.google.common.collect.ImmutableList<String> cacheModes,
                                                         com.google.common.collect.ImmutableMap<String,​String> extraData)
            ```

        []{#of(java.lang.String,java.lang.String,java.lang.String,int,long,java.util.Optional,java.lang.String,java.lang.String,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap)}

        -   #### of

            ``` methodSignature
            public static BuildEnvironmentDescription of​(String user,
                                                         String hostname,
                                                         String os,
                                                         int availableCores,
                                                         long systemMemory,
                                                         Optional<Boolean> buckDirty,
                                                         String buckCommit,
                                                         String javaVersion,
                                                         com.google.common.collect.ImmutableList<String> cacheModes,
                                                         com.google.common.collect.ImmutableMap<String,​String> extraData)
            ```

        []{#of(java.lang.String,java.lang.String,java.lang.String,int,long,java.util.Optional,java.lang.String,java.lang.String,int)}

        -   #### of

            ``` methodSignature
            public static BuildEnvironmentDescription of​(String user,
                                                         String hostname,
                                                         String os,
                                                         int availableCores,
                                                         long systemMemory,
                                                         Optional<Boolean> buckDirty,
                                                         String buckCommit,
                                                         String javaVersion,
                                                         int jsonProtocolVersion)
            ```

        []{#of(java.lang.String,java.lang.String,java.lang.String,int,long,java.util.Optional,java.lang.String,java.lang.String,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap,int,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static BuildEnvironmentDescription of​(String user,
                                                         String hostname,
                                                         String os,
                                                         int availableCores,
                                                         long systemMemory,
                                                         Optional<Boolean> buckDirty,
                                                         String buckCommit,
                                                         String javaVersion,
                                                         com.google.common.collect.ImmutableList<String> cacheModes,
                                                         com.google.common.collect.ImmutableMap<String,​String> extraData,
                                                         int jsonProtocolVersion,
                                                         String buildType)
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
