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
[Package]{.packageLabelInType} [com.facebook.buck.core.rulekey](package-summary.html)
:::

## Class RuleKey {#class-rulekey .title title="Class RuleKey"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rulekey.RuleKey

::: description
-   

    ------------------------------------------------------------------------

        public class RuleKey
        extends Object

    ::: block
    RuleKey encapsulates regimented computation of SHA-1 keys that
    incorporate all BuildRule state relevant to idempotency. The
    RuleKey.Builder API conceptually implements the construction of an
    ordered map, and the key/val pairs are digested using an internal
    serialization that guarantees a 1:1 mapping for each distinct vector
    of keys \<header,k1,\...,kn\> in RuleKey.builder(header).set(k1, v1)
    \... .set(kn, vn).build().
    Note carefully that in order to reliably avoid accidental
    collisions, each RuleKey schema, as defined by the key vector, must
    have a distinct header. Otherwise it is possible (if unlikely) for
    serialized value data to alias serialized key data, with the result
    being identical RuleKeys for differing input. In practical terms
    this means that each BuildRule implementer should specify a distinct
    header, and that for all RuleKeys built with a particular header,
    the sequence of set() calls should be identical, even if values are
    missing. The set() methods specifically handle null values to
    accommodate this regime.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                           Description
          ----------------------------------------------------- -------------
          `RuleKey​(com.google.common.hash.HashCode hashCode)`    
          `RuleKey​(String hashString)`                           

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                 Description
          ----------------------------------- ---------------------- -------------
          `boolean`                           `equals​(Object obj)`    
          `com.google.common.hash.HashCode`   `getHashCode()`         
          `int`                               `hashCode()`            
          `String`                            `toString()`            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.hash.HashCode)}

        -   #### RuleKey

                public RuleKey​(com.google.common.hash.HashCode hashCode)

        []{#<init>(java.lang.String)}

        -   #### RuleKey

                public RuleKey​(String hashString)

            [Parameters:]{.paramLabel}
            :   `hashString` - string that conforms to the contract of
                the return value of `HashCode.toString()`.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHashCode()}

        -   #### getHashCode

            ``` methodSignature
            public com.google.common.hash.HashCode getHashCode()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   the `toString()` of the hash code that underlies this
                RuleKey.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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
