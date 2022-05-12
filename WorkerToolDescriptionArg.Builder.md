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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class WorkerToolDescriptionArg.Builder {#class-workertooldescriptionarg.builder .title title="Class WorkerToolDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.WorkerToolDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [WorkerToolDescriptionArg](WorkerToolDescriptionArg.html "class in com.facebook.buck.shell")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class WorkerToolDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`WorkerToolDescriptionArg`](WorkerToolDescriptionArg.html "class in com.facebook.buck.shell").
    Initialize attributes and then invoke the [`build()`](#build())
    method to create an immutable instance.
    *`Builder` is not thread-safe and generally should not be stored in
    a field or collection, but instead used immediately to create
    instances.*
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `WorkerToolDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](WorkerTo |
        |                       |                       | olDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | WorkerToolDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Wo       |
        |                       |                       | rkerToolDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](WorkerTo |
        |                       |                       | olDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](WorkerTo |
        |                       |                       | olDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | WorkerToolDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | WorkerToolDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Wo       |
        |                       |                       | rkerToolDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Wo       |
        |                       |                       | rkerToolDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Work                 | `build()`             | ::: block             |
        | erToolDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`WorkerToo           |
        |                       |                       | lDescriptionArg`](Wor |
        |                       |                       | kerToolDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.shell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `from​(com.f           | ::: block             |
        | scriptionArg.Builder` | acebook.buck.shell.Wo | Copy abstract value   |
        |                       | rkerToolDescription.A | type                  |
        |                       | bstractWorkerToolDesc | `AbstractWork         |
        |                       | riptionArg instance)` | erToolDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `from​(WorkerToolDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Work                 |
        |                       |                       | erToolDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`env                 |
        |                       |                       | `](WorkerToolDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [`env                 |
        |                       |                       | `](WorkerToolDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [`env                 |
        |                       |                       | `](WorkerToolDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setArgs​(Eithe        | ::: block             |
        | scriptionArg.Builder` | r<StringWithMacros,​co | Initializes the value |
        |                       | m.google.common.colle | for the               |
        |                       | ct.ImmutableList<Stri | [`args`               |
        |                       | ngWithMacros>> args)` | ](WorkerToolDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](WorkerTo |
        |                       |                       | olDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](WorkerToolDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](WorkerToolDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`env                 |
        |                       |                       | `](WorkerToolDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | Exe​(BuildTarget exe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`exe                 |
        |                       |                       | `](WorkerToolDescript |
        |                       |                       | ionArg.html#getExe()) |
        |                       |                       | to exe.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tExe​(Optional<? exten | Initializes the       |
        |                       | ds BuildTarget> exe)` | optional value        |
        |                       |                       | [`exe                 |
        |                       |                       | `](WorkerToolDescript |
        |                       |                       | ionArg.html#getExe()) |
        |                       |                       | to exe.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | WorkerToolDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Wo       |
        |                       |                       | rkerToolDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setMaxWor            | ::: block             |
        | scriptionArg.Builder` | kers​(int maxWorkers)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`maxWorkers`](Work   |
        |                       |                       | erToolDescriptionArg. |
        |                       |                       | html#getMaxWorkers()) |
        |                       |                       | to maxWorkers.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tMaxWorkers​(Optional< | Initializes the       |
        |                       | Integer> maxWorkers)` | optional value        |
        |                       |                       | [`maxWorkers`](Work   |
        |                       |                       | erToolDescriptionArg. |
        |                       |                       | html#getMaxWorkers()) |
        |                       |                       | to maxWorkers.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setMaxWorkersPerThre | ::: block             |
        | scriptionArg.Builder` | adPercent​(int maxWork | Initializes the       |
        |                       | ersPerThreadPercent)` | optional value        |
        |                       |                       | [`maxWork             |
        |                       |                       | ersPerThreadPercent`] |
        |                       |                       | (WorkerToolDescriptio |
        |                       |                       | nArg.html#getMaxWorke |
        |                       |                       | rsPerThreadPercent()) |
        |                       |                       | to                    |
        |                       |                       | maxWor                |
        |                       |                       | kersPerThreadPercent. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setMaxWorkers        | ::: block             |
        | scriptionArg.Builder` | PerThreadPercent​(Opti | Initializes the       |
        |                       | onal<Integer> maxWork | optional value        |
        |                       | ersPerThreadPercent)` | [`maxWork             |
        |                       |                       | ersPerThreadPercent`] |
        |                       |                       | (WorkerToolDescriptio |
        |                       |                       | nArg.html#getMaxWorke |
        |                       |                       | rsPerThreadPercent()) |
        |                       |                       | to                    |
        |                       |                       | maxWor                |
        |                       |                       | kersPerThreadPercent. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](WorkerToolDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setPersistent        | ::: block             |
        | scriptionArg.Builder` | ​(boolean persistent)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`persistent`](Work   |
        |                       |                       | erToolDescriptionArg. |
        |                       |                       | html#getPersistent()) |
        |                       |                       | to persistent.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `se                   | ::: block             |
        | scriptionArg.Builder` | tPersistent​(Optional< | Initializes the       |
        |                       | Boolean> persistent)` | optional value        |
        |                       |                       | [`persistent`](Work   |
        |                       |                       | erToolDescriptionArg. |
        |                       |                       | html#getPersistent()) |
        |                       |                       | to persistent.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `setSoloAsyn          | ::: block             |
        | scriptionArg.Builder` | c​(boolean soloAsync)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`soloAsync`](Wor     |
        |                       |                       | kerToolDescriptionArg |
        |                       |                       | .html#getSoloAsync()) |
        |                       |                       | to soloAsync.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerToolDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setSoloAsync​(Optional | Initializes the       |
        |                       | <Boolean> soloAsync)` | optional value        |
        |                       |                       | [`soloAsync`](Wor     |
        |                       |                       | kerToolDescriptionArg |
        |                       |                       | .html#getSoloAsync()) |
        |                       |                       | to soloAsync.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.shell.WorkerToolDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder from​(WorkerToolDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `WorkerToolDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.shell.WorkerToolDescription.AbstractWorkerToolDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder from​(com.facebook.buck.shell.WorkerToolDescription.AbstractWorkerToolDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractWorkerToolDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder from​(BuildRuleArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.BuildRuleArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder from​(ConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.ConstructorArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.lang.String,com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### putEnv

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder putEnv​(String key,
                                                                 StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](WorkerToolDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](WorkerToolDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`env`](WorkerToolDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllEnv(java.util.Map)}

        -   #### putAllEnv

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](WorkerToolDescriptionArg.html#getEnv()) map. Nulls
            are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setArgs(com.facebook.buck.util.types.Either)}

        -   #### setArgs

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setArgs​(Either<StringWithMacros,​com.google.common.collect.ImmutableList<StringWithMacros>> args)
            ```

            ::: block
            Initializes the value for the
            [`args`](WorkerToolDescriptionArg.html#getArgs()) attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`args`](WorkerToolDescriptionArg.html#getArgs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `args` - The value for args

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExe(com.facebook.buck.core.model.BuildTarget)}

        -   #### setExe

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setExe​(BuildTarget exe)
            ```

            ::: block
            Initializes the optional value
            [`exe`](WorkerToolDescriptionArg.html#getExe()) to exe.
            :::

            [Parameters:]{.paramLabel}
            :   `exe` - The value for exe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExe(java.util.Optional)}

        -   #### setExe

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setExe​(Optional<? extends BuildTarget> exe)
            ```

            ::: block
            Initializes the optional value
            [`exe`](WorkerToolDescriptionArg.html#getExe()) to exe.
            :::

            [Parameters:]{.paramLabel}
            :   `exe` - The value for exe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMaxWorkers(int)}

        -   #### setMaxWorkers

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setMaxWorkers​(int maxWorkers)
            ```

            ::: block
            Initializes the optional value
            [`maxWorkers`](WorkerToolDescriptionArg.html#getMaxWorkers())
            to maxWorkers.
            :::

            [Parameters:]{.paramLabel}
            :   `maxWorkers` - The value for maxWorkers

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMaxWorkers(java.util.Optional)}

        -   #### setMaxWorkers

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setMaxWorkers​(Optional<Integer> maxWorkers)
            ```

            ::: block
            Initializes the optional value
            [`maxWorkers`](WorkerToolDescriptionArg.html#getMaxWorkers())
            to maxWorkers.
            :::

            [Parameters:]{.paramLabel}
            :   `maxWorkers` - The value for maxWorkers

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMaxWorkersPerThreadPercent(int)}

        -   #### setMaxWorkersPerThreadPercent

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setMaxWorkersPerThreadPercent​(int maxWorkersPerThreadPercent)
            ```

            ::: block
            Initializes the optional value
            [`maxWorkersPerThreadPercent`](WorkerToolDescriptionArg.html#getMaxWorkersPerThreadPercent())
            to maxWorkersPerThreadPercent.
            :::

            [Parameters:]{.paramLabel}
            :   `maxWorkersPerThreadPercent` - The value for
                maxWorkersPerThreadPercent

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMaxWorkersPerThreadPercent(java.util.Optional)}

        -   #### setMaxWorkersPerThreadPercent

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setMaxWorkersPerThreadPercent​(Optional<Integer> maxWorkersPerThreadPercent)
            ```

            ::: block
            Initializes the optional value
            [`maxWorkersPerThreadPercent`](WorkerToolDescriptionArg.html#getMaxWorkersPerThreadPercent())
            to maxWorkersPerThreadPercent.
            :::

            [Parameters:]{.paramLabel}
            :   `maxWorkersPerThreadPercent` - The value for
                maxWorkersPerThreadPercent

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPersistent(boolean)}

        -   #### setPersistent

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setPersistent​(boolean persistent)
            ```

            ::: block
            Initializes the optional value
            [`persistent`](WorkerToolDescriptionArg.html#getPersistent())
            to persistent.
            :::

            [Parameters:]{.paramLabel}
            :   `persistent` - The value for persistent

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPersistent(java.util.Optional)}

        -   #### setPersistent

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setPersistent​(Optional<Boolean> persistent)
            ```

            ::: block
            Initializes the optional value
            [`persistent`](WorkerToolDescriptionArg.html#getPersistent())
            to persistent.
            :::

            [Parameters:]{.paramLabel}
            :   `persistent` - The value for persistent

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSoloAsync(boolean)}

        -   #### setSoloAsync

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setSoloAsync​(boolean soloAsync)
            ```

            ::: block
            Initializes the optional value
            [`soloAsync`](WorkerToolDescriptionArg.html#getSoloAsync())
            to soloAsync.
            :::

            [Parameters:]{.paramLabel}
            :   `soloAsync` - The value for soloAsync

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSoloAsync(java.util.Optional)}

        -   #### setSoloAsync

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setSoloAsync​(Optional<Boolean> soloAsync)
            ```

            ::: block
            Initializes the optional value
            [`soloAsync`](WorkerToolDescriptionArg.html#getSoloAsync())
            to soloAsync.
            :::

            [Parameters:]{.paramLabel}
            :   `soloAsync` - The value for soloAsync

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](WorkerToolDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](WorkerToolDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](WorkerToolDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](WorkerToolDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](WorkerToolDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](WorkerToolDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](WorkerToolDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](WorkerToolDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](WorkerToolDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultTargetPlatform(java.util.Optional)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](WorkerToolDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](WorkerToolDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](WorkerToolDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](WorkerToolDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](WorkerToolDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final WorkerToolDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](WorkerToolDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public WorkerToolDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`WorkerToolDescriptionArg`](WorkerToolDescriptionArg.html "class in com.facebook.buck.shell").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of WorkerToolDescriptionArg

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if any required attributes are
                missing
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
