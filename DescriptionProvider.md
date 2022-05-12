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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph](package-summary.html)
:::

## Interface DescriptionProvider {#interface-descriptionprovider .title title="Interface DescriptionProvider"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `org.pf4j.ExtensionPoint`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidDescriptionsProvider`, `AppleDescriptionProvider`,
        `CxxDescriptionsProvider`, `DDescriptionsProvider`,
        `DotNetRuleProvider`, `FileDescriptionsProvider`,
        `FilegroupDescriptionsProvider`, `GoDescriptionsProvider`,
        `GroovyDescriptionsProvider`, `GwtDescriptionsProvider`,
        `HalideDescriptionsProvider`, `HaskellDescriptionsProvider`,
        `JavaDescriptionProvider`, `JavaDescriptionsProvider`,
        `JsDescriptionsProvider`, `KotlinDescriptionsProvider`,
        `LegacyToolchainDescriptionProvider`, `LuaDescriptionsProvider`,
        `OcamlDescriptionsProvider`, `PythonDescriptionsProvider`,
        `RustDescriptionsProvider`, `ScalaDescriptionsProvider`,
        `ShellDescriptionsProvider`, `SwiftDescriptionsProvider`,
        `TestRunnerDescriptionsProvider`, `VersionDescriptionsProvider`,
        `XCodeDescriptionProvider`, `ZipDescriptionProvider`

    ------------------------------------------------------------------------

        public interface DescriptionProvider
        extends org.pf4j.ExtensionPoint

    ::: block
    An `ExtensionPoint` which provides a way to register an arbitrary
    set of
    [`Description`](../../description/Description.html "interface in com.facebook.buck.core.description")s.
    Clients that want to provide descriptions need to implement this
    interface and annotation that class with `Extension` annotation.

    For example:

           @Extension
           public class LanguageDescriptionProvider implements DescriptionProvider {
             @Override
             public Collection<<Description<?>> getDescriptions() {
               return Arrays.asList(
                 new LanguageRuleDescription()
               );
             }
           }
         

    Then the target with the client provider should be added to the
    dependencies of `  //src/com/facebook/buck/cli:main` target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type              Method                                                  Description
          ------------------------------ ------------------------------------------------------- -------------
          `Collection<Description<?>>`   `getDescriptions​(DescriptionCreationContext context)`    

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

        []{#getDescriptions(com.facebook.buck.core.description.DescriptionCreationContext)}

        -   #### getDescriptions

            ``` methodSignature
            Collection<Description<?>> getDescriptions​(DescriptionCreationContext context)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
