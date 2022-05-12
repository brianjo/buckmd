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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.interfaces](package-summary.html)
:::

## Interface MetadataProvider {#interface-metadataprovider .title title="Interface MetadataProvider"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface MetadataProvider

    ::: block
    Provides RemoteExecutionMetadata to send along GRPC requests.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                           Method                                                                           Description
          --------------------------------------------------------------------------- -------------------------------------------------------------------------------- -------------
          `com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata`           `get()`                                                                           
          `com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata.Builder`   `getBuilderForAction​(String actionDigest,                    String ruleName)`    
          `com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata`           `getForAction​(String actionDigest,             String ruleName)`                  

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

        []{#get()}

        -   #### get

            ``` methodSignature
            com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata get()
            ```

        []{#getBuilderForAction(java.lang.String,java.lang.String)}

        -   #### getBuilderForAction

            ``` methodSignature
            com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata.Builder getBuilderForAction​(String actionDigest,
                                                                                                        String ruleName)
            ```

        []{#getForAction(java.lang.String,java.lang.String)}

        -   #### getForAction

            ``` methodSignature
            com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata getForAction​(String actionDigest,
                                                                                         String ruleName)
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
