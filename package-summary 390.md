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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.remoteexecution {#package-com.facebook.buck.remoteexecution .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AsyncBlobFetcher](Async          | ::: block                         |
    | BlobFetcher.html "interface in co | Interface used by                 |
    | m.facebook.buck.remoteexecution") | OutputsMaterializer to fetch      |
    |                                   | outputs from the CAS.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CasBlobUploader](CasB            | ::: block                         |
    | lobUploader.html "interface in co | Interface used to upload          |
    | m.facebook.buck.remoteexecution") | inputs/outputs to the CAS.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ContentAddressed                 | ::: block                         |
    | StorageClient](ContentAddressedSt | This is a simple                  |
    | orageClient.html "interface in co | ContentAddressedStorageClient     |
    | m.facebook.buck.remoteexecution") | interface used for remote         |
    |                                   | execution.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ContentAddressedS                | ::: block                         |
    | torageClient.FileMaterializer](Co | Interface for filesystem          |
    | ntentAddressedStorageClient.FileM | operations required for           |
    | aterializer.html "interface in co | materialization.                  |
    | m.facebook.buck.remoteexecution") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Re                               | ::: block                         |
    | moteExecutionClients](RemoteExecu | A Remote Execution service        |
    | tionClients.html "interface in co | consists of two primary things,   |
    | m.facebook.buck.remoteexecution") | an execution service and a CAS.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutio                   | ::: block                         |
    | nServiceClient](RemoteExecutionSe | Interface for a client of the     |
    | rviceClient.html "interface in co | remote execution service.         |
    | m.facebook.buck.remoteexecution") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecuti                    | ::: block                         |
    | onServiceClient.ExecutionHandle]( | Handle for an execution in        |
    | RemoteExecutionServiceClient.Exec | progress.                         |
    | utionHandle.html "interface in co | :::                               |
    | m.facebook.buck.remoteexecution") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecuti                    | ::: block                         |
    | onServiceClient.ExecutionResult]( | Represents the result of remote   |
    | RemoteExecutionServiceClient.Exec | execution.                        |
    | utionResult.html "interface in co | :::                               |
    | m.facebook.buck.remoteexecution") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UploadDataSupplier](UploadD      | ::: block                         |
    | ataSupplier.html "interface in co | Used for wrapping access to data  |
    | m.facebook.buck.remoteexecution") | for uploads.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WorkerRequ                       | ::: block                         |
    | irementsProvider](WorkerRequireme | Provides rule\'s RE worker        |
    | ntsProvider.html "interface in co | requirements for given target     |
    | m.facebook.buck.remoteexecution") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [CasBlobUpl                       | ::: block                         |
    | oader.UploadResult](CasBlobUpload | Result (status/error message) of  |
    | er.UploadResult.html "class in co | an upload.                        |
    | m.facebook.buck.remoteexecution") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileBasedWorkerRequireme         | ::: block                         |
    | ntsProvider](FileBasedWorkerRequi | Provides rule\'s RE worker        |
    | rementsProvider.html "class in co | requirements based on JSON file   |
    | m.facebook.buck.remoteexecution") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | MetadataProviderFactory](Metadata | Static class providing factory    |
    | ProviderFactory.html "class in co | methods for instances of          |
    | m.facebook.buck.remoteexecution") | MetadataProviders.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoOpWorkerRequ                   | ::: block                         |
    | irementsProvider](NoOpWorkerRequi | WorkerRequirementsProvider that   |
    | rementsProvider.html "class in co | always returns default            |
    | m.facebook.buck.remoteexecution") | WorkerRequirements                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
