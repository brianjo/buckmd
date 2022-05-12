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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys.hasher](package-summary.html)
:::

## Class RuleKeyHasherTypes {#class-rulekeyhashertypes .title title="Class RuleKeyHasherTypes"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes

::: description
-   

    ------------------------------------------------------------------------

        public class RuleKeyHasherTypes
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                   Description
          ------------------- ----------------------- -------------
          `static byte`       `ARCHIVE_MEMBER_PATH`    
          `static byte`       `BYTE`                   
          `static byte`       `BYTE_ARRAY`             
          `static byte`       `CONTAINER`              
          `static byte`       `DOUBLE`                 
          `static byte`       `FALSE`                  
          `static byte`       `FLOAT`                  
          `static byte`       `INTEGER`                
          `static byte`       `KEY`                    
          `static byte`       `LONG`                   
          `static byte`       `NON_HASHING_PATH`       
          `static byte`       `NULL`                   
          `static byte`       `PATH`                   
          `static byte`       `PATTERN`                
          `static byte`       `RULE_KEY`               
          `static byte`       `RULE_TYPE`              
          `static byte`       `SHA1`                   
          `static byte`       `SHORT`                  
          `static byte`       `SOURCE_ROOT`            
          `static byte`       `STRING`                 
          `static byte`       `TARGET`                 
          `static byte`       `TARGET_SOURCE_PATH`     
          `static byte`       `TRUE`                   
          `static byte`       `WRAPPER`                

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                  Description
          ------------------- ------------------------------------------------------- -------------
          `static byte`       `containerSubType​(RuleKeyHasher.Container container)`    
          `static byte`       `wrapperSubType​(RuleKeyHasher.Wrapper wrapper)`          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#KEY}

        -   #### KEY

                public static final byte KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.KEY)

        []{#NULL}

        -   #### NULL

                public static final byte NULL

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.NULL)

        []{#TRUE}

        -   #### TRUE

                public static final byte TRUE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.TRUE)

        []{#FALSE}

        -   #### FALSE

                public static final byte FALSE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.FALSE)

        []{#BYTE_ARRAY}

        -   #### BYTE_ARRAY

                public static final byte BYTE_ARRAY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.BYTE_ARRAY)

        []{#BYTE}

        -   #### BYTE

                public static final byte BYTE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.BYTE)

        []{#SHORT}

        -   #### SHORT

                public static final byte SHORT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.SHORT)

        []{#INTEGER}

        -   #### INTEGER

                public static final byte INTEGER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.INTEGER)

        []{#LONG}

        -   #### LONG

                public static final byte LONG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.LONG)

        []{#FLOAT}

        -   #### FLOAT

                public static final byte FLOAT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.FLOAT)

        []{#DOUBLE}

        -   #### DOUBLE

                public static final byte DOUBLE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.DOUBLE)

        []{#STRING}

        -   #### STRING

                public static final byte STRING

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.STRING)

        []{#PATTERN}

        -   #### PATTERN

                public static final byte PATTERN

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.PATTERN)

        []{#SHA1}

        -   #### SHA1

                public static final byte SHA1

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.SHA1)

        []{#PATH}

        -   #### PATH

                public static final byte PATH

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.PATH)

        []{#ARCHIVE_MEMBER_PATH}

        -   #### ARCHIVE_MEMBER_PATH

                public static final byte ARCHIVE_MEMBER_PATH

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.ARCHIVE_MEMBER_PATH)

        []{#NON_HASHING_PATH}

        -   #### NON_HASHING_PATH

                public static final byte NON_HASHING_PATH

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.NON_HASHING_PATH)

        []{#SOURCE_ROOT}

        -   #### SOURCE_ROOT

                public static final byte SOURCE_ROOT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.SOURCE_ROOT)

        []{#RULE_KEY}

        -   #### RULE_KEY

                public static final byte RULE_KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.RULE_KEY)

        []{#RULE_TYPE}

        -   #### RULE_TYPE

                public static final byte RULE_TYPE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.RULE_TYPE)

        []{#TARGET}

        -   #### TARGET

                public static final byte TARGET

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.TARGET)

        []{#TARGET_SOURCE_PATH}

        -   #### TARGET_SOURCE_PATH

                public static final byte TARGET_SOURCE_PATH

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.TARGET_SOURCE_PATH)

        []{#CONTAINER}

        -   #### CONTAINER

                public static final byte CONTAINER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.CONTAINER)

        []{#WRAPPER}

        -   #### WRAPPER

                public static final byte WRAPPER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.keys.hasher.RuleKeyHasherTypes.WRAPPER)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#wrapperSubType(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### wrapperSubType

            ``` methodSignature
            public static byte wrapperSubType​(RuleKeyHasher.Wrapper wrapper)
            ```

        []{#containerSubType(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container)}

        -   #### containerSubType

            ``` methodSignature
            public static byte containerSubType​(RuleKeyHasher.Container container)
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
