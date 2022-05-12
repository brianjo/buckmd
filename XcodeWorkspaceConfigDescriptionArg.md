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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.common](package-summary.html)
:::

## Class XcodeWorkspaceConfigDescriptionArg {#class-xcodeworkspaceconfigdescriptionarg .title title="Class XcodeWorkspaceConfigDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.common.XcodeWorkspaceConfigDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class XcodeWorkspaceConfigDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `XcodeWorkspaceConfigDescription.AbstractXcodeWorkspaceConfigDescriptionArg`.
    Use the builder to create immutable instances:
    `XcodeWorkspaceConfigDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `X                    | ::: block             |
        |                       | codeWorkspaceConfigDe | Builds instances of   |
        |                       | scriptionArg.Builder` | type                  |
        |                       |                       | [`Xco                 |
        |                       |                       | deWorkspaceConfigDesc |
        |                       |                       | riptionArg`](XcodeWor |
        |                       |                       | kspaceConfigDescripti |
        |                       |                       | onArg.html "class in  |
        |                       |                       | com.facebook.buck.fea |
        |                       |                       | tures.apple.common"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static X             | `builder()`           | ::: block             |
        | codeWorkspaceConfigDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`Xco                 |
        |                       |                       | deWorkspaceConfigDesc |
        |                       |                       | riptionArg`](XcodeWor |
        |                       |                       | kspaceConfigDescripti |
        |                       |                       | onArg.html "class in  |
        |                       |                       | com.facebook.buck.fea |
        |                       |                       | tures.apple.common"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `XcodeWorkspace       |
        |                       |                       | ConfigDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `ge                   |                       |
        | om.google.common.coll | tActionConfigNames()` |                       |
        | ect.ImmutableMap<Sche |                       |                       |
        | meActionType,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.g       | `getAddit             |                       |
        | oogle.common.collect. | ionalSchemeActions()` |                       |
        | ImmutableMap<SchemeAc |                       |                       |
        | tionType,​com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<XCScheme.Additi |                       |                       |
        | onalActions,​com.googl |                       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableList<String>>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getA                 |                       |
        |                       | pplicationLanguage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `ge                   |                       |
        |                       | tApplicationRegion()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getCo                |                       |
        | gle.common.collect.Im | mmandLineArguments()` |                       |
        | mutableMap<SchemeActi |                       |                       |
        | onType,​com.google.com |                       |                       |
        | mon.collect.Immutable |                       |                       |
        | Map<String,​String>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getEn                |                       |
        | gle.common.collect.Im | vironmentVariables()` |                       |
        | mutableMap<SchemeActi |                       |                       |
        | onType,​com.google.com |                       |                       |
        | mon.collect.Immutable |                       |                       |
        | Map<String,​String>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getExpa              |                       |
        | gle.common.collect.Im | ndVariablesBasedOn()` |                       |
        | mutableMap<SchemeActi |                       |                       |
        | onType,​BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getEx                |                       |
        |                       | plicitRunnablePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getExtraSchemes()`   |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableSortedMap |                       |                       |
        | <String,​BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getE                 |                       |
        | n.collect.ImmutableSo | xtraShallowTargets()` |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExtraTargets()`   |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExtraTests()`     |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `g                    |                       |
        |                       | etIsRemoteRunnable()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getLaunchStyle()`    |                       |
        | tional<XCScheme.Launc |                       |                       |
        | hAction.LaunchStyle>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getNotif             |                       |
        |                       | icationPayloadFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getSrcTarget()`      |                       |
        | ptional<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getWasCrea           | ::: block             |
        |                       | tedForAppExtension()` | Add value to scheme   |
        |                       |                       | to indicate it will   |
        |                       |                       | be used to work on an |
        |                       |                       | app extension.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `getWatchInterface()` |                       |
        | nal<XCScheme.LaunchAc |                       |                       |
        | tion.WatchInterface>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getWorkspaceName()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `srcTarget`,          |
        |                       |                       | `extraTests`,         |
        |                       |                       | `extraTargets`,       |
        |                       |                       | `                     |
        |                       |                       | extraShallowTargets`, |
        |                       |                       | `workspaceName`,      |
        |                       |                       | `actionConfigNames`,  |
        |                       |                       | `extraSchemes`,       |
        |                       |                       | `e                    |
        |                       |                       | nvironmentVariables`, |
        |                       |                       | `c                    |
        |                       |                       | ommandLineArguments`, |
        |                       |                       | `                     |
        |                       |                       | applicationLanguage`, |
        |                       |                       | `applicationRegion`,  |
        |                       |                       | `exp                  |
        |                       |                       | andVariablesBasedOn`, |
        |                       |                       | `wasCre               |
        |                       |                       | atedForAppExtension`, |
        |                       |                       | `isRemoteRunnable`,   |
        |                       |                       | `e                    |
        |                       |                       | xplicitRunnablePath`, |
        |                       |                       | `noti                 |
        |                       |                       | ficationPayloadFile`, |
        |                       |                       | `watchInterface`,     |
        |                       |                       | `launchStyle`,        |
        |                       |                       | `addi                 |
        |                       |                       | tionalSchemeActions`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `labels`, `licenses`, |
        |                       |                       | `name`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `XcodeWorkspace       |
        |                       |                       | ConfigDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSrcTarget()}

        -   #### getSrcTarget

            ``` methodSignature
            public Optional<BuildTarget> getSrcTarget()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `srcTarget` attribute

        []{#getExtraTests()}

        -   #### getExtraTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getExtraTests()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `extraTests` attribute

        []{#getExtraTargets()}

        -   #### getExtraTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getExtraTargets()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `extraTargets` attribute

        []{#getExtraShallowTargets()}

        -   #### getExtraShallowTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getExtraShallowTargets()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `extraShallowTargets` attribute

        []{#getWorkspaceName()}

        -   #### getWorkspaceName

            ``` methodSignature
            public Optional<String> getWorkspaceName()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `workspaceName` attribute

        []{#getActionConfigNames()}

        -   #### getActionConfigNames

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<SchemeActionType,​String> getActionConfigNames()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `actionConfigNames` attribute

        []{#getExtraSchemes()}

        -   #### getExtraSchemes

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​BuildTarget> getExtraSchemes()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `extraSchemes` attribute

        []{#getEnvironmentVariables()}

        -   #### getEnvironmentVariables

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<String,​String>>> getEnvironmentVariables()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `environmentVariables` attribute

        []{#getCommandLineArguments()}

        -   #### getCommandLineArguments

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<String,​String>>> getCommandLineArguments()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `commandLineArguments` attribute

        []{#getApplicationLanguage()}

        -   #### getApplicationLanguage

            ``` methodSignature
            public Optional<String> getApplicationLanguage()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationLanguage` attribute

        []{#getApplicationRegion()}

        -   #### getApplicationRegion

            ``` methodSignature
            public Optional<String> getApplicationRegion()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationRegion` attribute

        []{#getExpandVariablesBasedOn()}

        -   #### getExpandVariablesBasedOn

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<SchemeActionType,​BuildTarget>> getExpandVariablesBasedOn()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `expandVariablesBasedOn` attribute

        []{#getWasCreatedForAppExtension()}

        -   #### getWasCreatedForAppExtension

            ``` methodSignature
            public Optional<Boolean> getWasCreatedForAppExtension()
            ```

            ::: block
            Add value to scheme to indicate it will be used to work on
            an app extension. This should cause Xcode to automatically
            begin debugging the extension when it\'s launched.
            :::

        []{#getIsRemoteRunnable()}

        -   #### getIsRemoteRunnable

            ``` methodSignature
            public Optional<Boolean> getIsRemoteRunnable()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `isRemoteRunnable` attribute

        []{#getExplicitRunnablePath()}

        -   #### getExplicitRunnablePath

            ``` methodSignature
            public Optional<String> getExplicitRunnablePath()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `explicitRunnablePath` attribute

        []{#getNotificationPayloadFile()}

        -   #### getNotificationPayloadFile

            ``` methodSignature
            public Optional<String> getNotificationPayloadFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `notificationPayloadFile` attribute

        []{#getWatchInterface()}

        -   #### getWatchInterface

            ``` methodSignature
            public Optional<XCScheme.LaunchAction.WatchInterface> getWatchInterface()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `watchInterface` attribute

        []{#getLaunchStyle()}

        -   #### getLaunchStyle

            ``` methodSignature
            public Optional<XCScheme.LaunchAction.LaunchStyle> getLaunchStyle()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `launchStyle` attribute

        []{#getAdditionalSchemeActions()}

        -   #### getAdditionalSchemeActions

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<XCScheme.AdditionalActions,​com.google.common.collect.ImmutableList<String>>>> getAdditionalSchemeActions()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `additionalSchemeActions` attribute

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleArg`]{.descfrmTypeLabel}
            :::

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `compatibleWith` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleArg`]{.descfrmTypeLabel}
            :::

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultTargetPlatform` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `defaultTargetPlatform` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            [Description copied from
            interface: `ConstructorArg`]{.descfrmTypeLabel}
            :::

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `name` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `XcodeWorkspaceConfigDescriptionArg` that have equal
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `srcTarget`,
            `extraTests`, `extraTargets`, `extraShallowTargets`,
            `workspaceName`, `actionConfigNames`, `extraSchemes`,
            `environmentVariables`, `commandLineArguments`,
            `applicationLanguage`, `applicationRegion`,
            `expandVariablesBasedOn`, `wasCreatedForAppExtension`,
            `isRemoteRunnable`, `explicitRunnablePath`,
            `notificationPayloadFile`, `watchInterface`, `launchStyle`,
            `additionalSchemeActions`, `compatibleWith`,
            `defaultTargetPlatform`, `labels`, `licenses`, `name`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value
            `XcodeWorkspaceConfigDescriptionArg` with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static XcodeWorkspaceConfigDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`XcodeWorkspaceConfigDescriptionArg`](XcodeWorkspaceConfigDescriptionArg.html "class in com.facebook.buck.features.apple.common").
            :::

            [Returns:]{.returnLabel}
            :   A new XcodeWorkspaceConfigDescriptionArg builder
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
