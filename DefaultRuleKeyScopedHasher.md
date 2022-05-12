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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class DefaultRuleKeyScopedHasher\<HASH\> {#class-defaultrulekeyscopedhasherhash .title title="Class DefaultRuleKeyScopedHasher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.DefaultRuleKeyScopedHasher\<HASH\>

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyScopedHasher`

    ------------------------------------------------------------------------

        public class DefaultRuleKeyScopedHasher<HASH>
        extends Object
        implements RuleKeyScopedHasher

    ::: block
    A wrapper of
    [`RuleKeyHasher`](hasher/RuleKeyHasher.html "interface in com.facebook.buck.rules.keys.hasher")
    that provides scoped hashing facilities.
    Important: Container, wrapper and key signatures only get hashed if
    their scope was non-empty. I.e. if at least one thing gets hashed
    under their scope. This is to support rule key builders that ignore
    some fields.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                                Description
          ------------------- ---------------------------------------------------- -------------
          `static class `     `DefaultRuleKeyScopedHasher.DefaultContainerScope`    

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.keys.RuleKeyScopedHasher}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.keys.[RuleKeyScopedHasher](RuleKeyScopedHasher.html "interface in com.facebook.buck.rules.keys")

            `RuleKeyScopedHasher.ContainerScope`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RuleKeyScopedH       | `containe             | ::: block             |
        | asher.ContainerScope` | rScope​(RuleKeyHasher. | Hashes the container  |
        |                       | Container container)` | iff non-empty (i.e.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `getHasher()`         |                       |
        | gRuleKeyHasher<HASH>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Scope`               | `                     | ::: block             |
        |                       | keyScope​(String key)` | Hashes the key iff    |
        |                       |                       | non-empty (i.e.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Scope`               | `pa                   | ::: block             |
        |                       | thKeyScope​(Path key)` | Hashes the key iff    |
        |                       |                       | non-empty (i.e.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Scope`               | `wr                   | ::: block             |
        |                       | apperScope​(RuleKeyHas | Hashes the wrapper    |
        |                       | her.Wrapper wrapper)` | iff non-empty (i.e.   |
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

        []{#getHasher()}

        -   #### getHasher

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> getHasher()
            ```

        []{#keyScope(java.lang.String)}

        -   #### keyScope

            ``` methodSignature
            public Scope keyScope​(String key)
            ```

            ::: block
            Hashes the key iff non-empty (i.e. if anything gets hashed
            during its scope).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `keyScope` in interface `RuleKeyScopedHasher`

        []{#pathKeyScope(java.nio.file.Path)}

        -   #### pathKeyScope

            ``` methodSignature
            public Scope pathKeyScope​(Path key)
            ```

            ::: block
            Hashes the key iff non-empty (i.e. if anything gets hashed
            during its scope).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `pathKeyScope` in interface `RuleKeyScopedHasher`

        []{#wrapperScope(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### wrapperScope

            ``` methodSignature
            public Scope wrapperScope​(RuleKeyHasher.Wrapper wrapper)
            ```

            ::: block
            Hashes the wrapper iff non-empty (i.e. if any element gets
            hashed during its scope).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `wrapperScope` in interface `RuleKeyScopedHasher`

        []{#containerScope(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container)}

        -   #### containerScope

            ``` methodSignature
            public RuleKeyScopedHasher.ContainerScope containerScope​(RuleKeyHasher.Container container)
            ```

            ::: block
            Hashes the container iff non-empty (i.e. if any element gets
            hashed during its scope).
            Note that an element scope needs to be created for each
            element!
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `containerScope` in interface `RuleKeyScopedHasher`
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
-   [Nested](#nested.class.summary) \| 
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
