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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Class PlatformSerialization {#class-platformserialization .title title="Class PlatformSerialization"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.PlatformSerialization

::: description
-   

    All Implemented Interfaces:
    :   `CustomFieldBehaviorTag`, `CustomFieldSerializationTag`,
        `CustomFieldSerialization<Platform>`

    ------------------------------------------------------------------------

        public class PlatformSerialization
        extends Object
        implements CustomFieldSerialization<Platform>

    ::: block
    This can be used for serialization/deserialization of Platform.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `PlatformSerialization()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                                                             Description
          --------------------------------- ------------------------------------------------------------------ -------------
          `<E extends Exception>Platform`   `deserialize​(ValueCreator<E> deserializer)`                         
          `<E extends Exception>void`       `serialize​(Platform value,          ValueVisitor<E> serializer)`    

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

        []{#<init>()}

        -   #### PlatformSerialization

                public PlatformSerialization()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#serialize(com.facebook.buck.util.environment.Platform,com.facebook.buck.rules.modern.ValueVisitor)}

        -   #### serialize

            ``` methodSignature
            public <E extends Exception> void serialize​(Platform value,
                                                        ValueVisitor<E> serializer)
                                                 throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in
                interface `CustomFieldSerialization<Platform>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#deserialize(com.facebook.buck.rules.modern.ValueCreator)}

        -   #### deserialize

            ``` methodSignature
            public <E extends Exception> Platform deserialize​(ValueCreator<E> deserializer)
                                                       throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deserialize` in
                interface `CustomFieldSerialization<Platform>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`
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
