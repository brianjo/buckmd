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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.edenfs](package-summary.html)
:::

## Interface EdenClient {#interface-edenclient .title title="Interface EdenClient"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface EdenClient

    ::: block
    Client of Eden\'s fbthrift API that is intended to be a thin wrapper
    around `EdenService.Client`\'s API.
    Note that implementations of this interface are not guaranteed to be
    thread-safe.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                             Method                                                    Description
          --------------------------------------------- --------------------------------------------------------- -------------
          `List<com.facebook.eden.thrift.SHA1Result>`   `getSHA1​(String mountPoint,        List<String> paths)`    
          `List<com.facebook.eden.thrift.MountInfo>`    `listMounts()`                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSHA1(java.lang.String,java.util.List)}

        -   #### getSHA1

            ``` methodSignature
            List<com.facebook.eden.thrift.SHA1Result> getSHA1​(String mountPoint,
                                                              List<String> paths)
                                                       throws IOException,
                                                              com.facebook.thrift.TException,
                                                              com.facebook.eden.thrift.EdenError
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `com.facebook.thrift.TException`
            :   `com.facebook.eden.thrift.EdenError`

        []{#listMounts()}

        -   #### listMounts

            ``` methodSignature
            List<com.facebook.eden.thrift.MountInfo> listMounts()
                                                         throws com.facebook.eden.thrift.EdenError,
                                                                IOException,
                                                                com.facebook.thrift.TException
            ```

            [Throws:]{.throwsLabel}
            :   `com.facebook.eden.thrift.EdenError`
            :   `IOException`
            :   `com.facebook.thrift.TException`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
