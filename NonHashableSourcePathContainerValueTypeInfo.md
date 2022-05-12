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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.impl](package-summary.html)
:::

## Class NonHashableSourcePathContainerValueTypeInfo {#class-nonhashablesourcepathcontainervaluetypeinfo .title title="Class NonHashableSourcePathContainerValueTypeInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.impl.NonHashableSourcePathContainerValueTypeInfo

::: description
-   

    All Implemented Interfaces:
    :   `ValueTypeInfo<NonHashableSourcePathContainer>`

    ------------------------------------------------------------------------

        public class NonHashableSourcePathContainerValueTypeInfo
        extends Object
        implements ValueTypeInfo<NonHashableSourcePathContainer>

    ::: block
    ValueTypeInfo for a NonHashableSourcePathContainer. Derives
    deps+inputs from the contained SourcePath.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                       Description
          ------------------------------------------------- -------------
          `NonHashableSourcePathContainerValueTypeInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                                                                        Description
          ------------------------------------------------------- ----------------------------------------------------------------------------- -------------
          `<E extends Exception>NonHashableSourcePathContainer`   `create​(ValueCreator<E> creator)`                                              
          `<E extends Exception>void`                             `visit​(NonHashableSourcePathContainer value,      ValueVisitor<E> visitor)`    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### NonHashableSourcePathContainerValueTypeInfo

                public NonHashableSourcePathContainerValueTypeInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visit(com.facebook.buck.core.sourcepath.NonHashableSourcePathContainer,com.facebook.buck.rules.modern.ValueVisitor)}

        -   #### visit

            ``` methodSignature
            public <E extends Exception> void visit​(NonHashableSourcePathContainer value,
                                                    ValueVisitor<E> visitor)
                                             throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visit` in
                interface `ValueTypeInfo<NonHashableSourcePathContainer>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#create(com.facebook.buck.rules.modern.ValueCreator)}

        -   #### create

            ``` methodSignature
            public <E extends Exception> NonHashableSourcePathContainer create​(ValueCreator<E> creator)
                                                                        throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `create` in
                interface `ValueTypeInfo<NonHashableSourcePathContainer>`

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
