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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class UnsortedAndroidResourceDeps {#class-unsortedandroidresourcedeps .title title="Class UnsortedAndroidResourceDeps"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.UnsortedAndroidResourceDeps

::: description
-   

    ------------------------------------------------------------------------

        public class UnsortedAndroidResourceDeps
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                                    Description
          --------------------- ---------------------------------------- -------------
          `static interface `   `UnsortedAndroidResourceDeps.Callback`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------ -------------
          `UnsortedAndroidResourceDeps​(com.google.common.collect.ImmutableSet<HasAndroidResourceDeps> resourceDeps)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Unsorte       | `cr                   | ::: block             |
        | dAndroidResourceDeps` | eateFrom​(Collection<B | Returns transitive    |
        |                       | uildRule> rules,      | android resource deps |
        |                       |       Optional<Unsort | which are \_not\_     |
        |                       | edAndroidResourceDeps | sorted topologically, |
        |                       | .Callback> callback)` | only to be used when  |
        |                       |                       | the order of the      |
        |                       |                       | resource rules does   |
        |                       |                       | not matter, for       |
        |                       |                       | instance, when graph  |
        |                       |                       | enhancing             |
        |                       |                       | UberRDotJava,         |
        |                       |                       | DummyRDotJava,        |
        |                       |                       | AaptPackageResources  |
        |                       |                       | where we only need    |
        |                       |                       | the deps to correctly |
        |                       |                       | order the execution   |
        |                       |                       | of those buildables.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getResourceDeps()`   |                       |
        | com.google.common.col |                       |                       |
        | lect.ImmutableSet<Has |                       |                       |
        | AndroidResourceDeps>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(com.google.common.collect.ImmutableSet)}

        -   #### UnsortedAndroidResourceDeps

                public UnsortedAndroidResourceDeps​(com.google.common.collect.ImmutableSet<HasAndroidResourceDeps> resourceDeps)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResourceDeps()}

        -   #### getResourceDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<HasAndroidResourceDeps> getResourceDeps()
            ```

        []{#createFrom(java.util.Collection,java.util.Optional)}

        -   #### createFrom

            ``` methodSignature
            public static UnsortedAndroidResourceDeps createFrom​(Collection<BuildRule> rules,
                                                                 Optional<UnsortedAndroidResourceDeps.Callback> callback)
            ```

            ::: block
            Returns transitive android resource deps which are \_not\_
            sorted topologically, only to be used when the order of the
            resource rules does not matter, for instance, when graph
            enhancing UberRDotJava, DummyRDotJava, AaptPackageResources
            where we only need the deps to correctly order the execution
            of those buildables.
            :::
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
-   [Nested](#nested.class.summary) \| 
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
