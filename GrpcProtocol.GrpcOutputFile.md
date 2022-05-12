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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.grpc](package-summary.html)
:::

## Class GrpcProtocol.GrpcOutputFile {#class-grpcprotocol.grpcoutputfile .title title="Class GrpcProtocol.GrpcOutputFile"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcProtocol.GrpcOutputFile

::: description
-   

    All Implemented Interfaces:
    :   `Protocol.OutputFile`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [GrpcProtocol](GrpcProtocol.html "class in com.facebook.buck.remoteexecution.grpc")

    ------------------------------------------------------------------------

        public static class GrpcProtocol.GrpcOutputFile
        extends Object
        implements Protocol.OutputFile

    ::: block
    Wrapped Grpc OutputFile.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                               Description
          ------------------------------------------------------------------------- -------------
          `GrpcOutputFile​(build.bazel.remote.execution.v2.OutputFile outputFile)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                Description
          ------------------- --------------------- -------------
          `Protocol.Digest`   `getDigest()`          
          `boolean`           `getIsExecutable()`    
          `String`            `getPath()`            

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

        []{#<init>(build.bazel.remote.execution.v2.OutputFile)}

        -   #### GrpcOutputFile

                public GrpcOutputFile​(build.bazel.remote.execution.v2.OutputFile outputFile)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public String getPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPath` in interface `Protocol.OutputFile`

        []{#getDigest()}

        -   #### getDigest

            ``` methodSignature
            public Protocol.Digest getDigest()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDigest` in interface `Protocol.OutputFile`

        []{#getIsExecutable()}

        -   #### getIsExecutable

            ``` methodSignature
            public boolean getIsExecutable()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIsExecutable` in interface `Protocol.OutputFile`
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