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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.impl](package-summary.html)
:::

## Class HashCodeValueTypeInfo {#class-hashcodevaluetypeinfo .title title="Class HashCodeValueTypeInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.impl.HashCodeValueTypeInfo

::: description
-   

    All Implemented Interfaces:
    :   `ValueTypeInfo<com.google.common.hash.HashCode>`

    ------------------------------------------------------------------------

        public class HashCodeValueTypeInfo
        extends Object
        implements ValueTypeInfo<com.google.common.hash.HashCode>

    ::: block
    ValueTypeInfo for HashCode. These are basically treated as just the
    underlying hashcode string.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                         Field        Description
          --------------------------------------------------------- ------------ -------------
          `static ValueTypeInfo<com.google.common.hash.HashCode>`   `INSTANCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `HashCodeValueTypeInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                        Method                                                                         Description
          -------------------------------------------------------- ------------------------------------------------------------------------------ -------------
          `<E extends Exception>com.google.common.hash.HashCode`   `create​(ValueCreator<E> creator)`                                               
          `<E extends Exception>void`                              `visit​(com.google.common.hash.HashCode value,      ValueVisitor<E> visitor)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ValueTypeInfo}

            ### Methods inherited from interface com.facebook.buck.rules.modern.[ValueTypeInfo](../ValueTypeInfo.html "interface in com.facebook.buck.rules.modern")

            `createNotNull`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#INSTANCE}

        -   #### INSTANCE

                public static final ValueTypeInfo<com.google.common.hash.HashCode> INSTANCE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### HashCodeValueTypeInfo

                public HashCodeValueTypeInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visit(com.google.common.hash.HashCode,com.facebook.buck.rules.modern.ValueVisitor)}

        -   #### visit

            ``` methodSignature
            public <E extends Exception> void visit​(com.google.common.hash.HashCode value,
                                                    ValueVisitor<E> visitor)
                                             throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visit` in
                interface `ValueTypeInfo<com.google.common.hash.HashCode>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#create(com.facebook.buck.rules.modern.ValueCreator)}

        -   #### create

            ``` methodSignature
            public <E extends Exception> com.google.common.hash.HashCode create​(ValueCreator<E> creator)
                                                                         throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `create` in
                interface `ValueTypeInfo<com.google.common.hash.HashCode>`

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::