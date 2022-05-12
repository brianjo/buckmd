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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.android.dalvik {#package-com.facebook.buck.android.dalvik .title title="Package"}
:::

::: contentContainer
-   
      Interface                                                                                       Description
      ----------------------------------------------------------------------------------------------- -------------
      [ZipSplitter](ZipSplitter.html "interface in com.facebook.buck.android.dalvik")                  
      [ZipSplitterFactory](ZipSplitterFactory.html "interface in com.facebook.buck.android.dalvik")    

      : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [CanaryFactor                     | ::: block                         |
    | y](CanaryFactory.html "class in c | Helper to create a \"canary\"     |
    | om.facebook.buck.android.dalvik") | class for the secondary DEX.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DalvikAware                      | ::: block                         |
    | OutputStreamHelper](DalvikAwareOu | Helper to write a Zip file used   |
    | tputStreamHelper.html "class in c | by                                |
    | om.facebook.buck.android.dalvik") | [                                 |
    |                                   | `DalvikAwareZipSplitter`](DalvikA |
    |                                   | wareZipSplitter.html "class in co |
    |                                   | m.facebook.buck.android.dalvik"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DalvikAwareZipSplitter](Dalvik   | ::: block                         |
    | AwareZipSplitter.html "class in c | Implementation of                 |
    | om.facebook.buck.android.dalvik") | [`ZipSplitter`]                   |
    |                                   | (ZipSplitter.html "interface in c |
    |                                   | om.facebook.buck.android.dalvik") |
    |                                   | that uses estimates from          |
    |                                   | [`DalvikStatsTool`]               |
    |                                   | (DalvikStatsTool.html "class in c |
    |                                   | om.facebook.buck.android.dalvik") |
    |                                   | to determine how many classes to  |
    |                                   | pack into a dex.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DalvikAware                      |                                   |
    | ZipSplitterFactory](DalvikAwareZi |                                   |
    | pSplitterFactory.html "class in c |                                   |
    | om.facebook.buck.android.dalvik") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DalvikStatsTool]                 | ::: block                         |
    | (DalvikStatsTool.html "class in c | Tool to get stats about dalvik    |
    | om.facebook.buck.android.dalvik") | classes.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DalvikStatsTool.Stats](Dalvi     | ::: block                         |
    | kStatsTool.Stats.html "class in c | Stats about a java class.         |
    | om.facebook.buck.android.dalvik") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [EstimateDexWeightStep](Estim     |                                   |
    | ateDexWeightStep.html "class in c |                                   |
    | om.facebook.buck.android.dalvik") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                                           Description
      -------------------------------------------------------------------------------------------------------------- -------------
      [ZipSplitter.DexSplitStrategy](ZipSplitter.DexSplitStrategy.html "enum in com.facebook.buck.android.dalvik")    

      : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
