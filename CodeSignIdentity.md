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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain](package-summary.html)
:::

## Class CodeSignIdentity {#class-codesignidentity .title title="Class CodeSignIdentity"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.CodeSignIdentity

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class CodeSignIdentity
        extends Object
        implements AddsToRuleKey

    ::: block
    Represents a identity used in code signing.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `AD_HOC`              | ::: block             |
        | tic CodeSignIdentity` |                       | A pseudo-identity for |
        |                       |                       | ad hoc code signing.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `CodeSignIdentity()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract             | `getFingerprint()`    | ::: block             |
        | Optional<com.google.c |                       | Returns the           |
        | ommon.hash.HashCode>` |                       | identity\'s           |
        |                       |                       | certificate hash,     |
        |                       |                       | defined to be unique  |
        |                       |                       | for each identity.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `ge                   | ::: block             |
        |                       | tSubjectCommonName()` | Returns the full name |
        |                       |                       | of the identity.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `of​(Optio             |                       |
        | tic CodeSignIdentity` | nal<? extends com.goo |                       |
        |                       | gle.common.hash.HashC |                       |
        |                       | ode> fingerPrint,   S |                       |
        |                       | tring subjectCommonNa |                       |
        |                       | me,   boolean useSubj |                       |
        |                       | ectCommonNameToSign)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `of                   |                       |
        | tic CodeSignIdentity` | ​(Optional<com.google. |                       |
        |                       | common.hash.HashCode> |                       |
        |                       |  fingerPrint,   Strin |                       |
        |                       | g subjectCommonName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `ofAdhocSigne         |                       |
        | tic CodeSignIdentity` | dWithSubjectCommonNam |                       |
        |                       | e​(String commonName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `shouldUseSubje       |                       |
        |                       | ctCommonNameToSign()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `toFingerprin         | ::: block             |
        | Optional<com.google.c | t​(String identifier)` | Convert a `String`    |
        | ommon.hash.HashCode>` |                       | into a fingerprint    |
        |                       |                       | `HashCode` if it\'s   |
        |                       |                       | in the correct        |
        |                       |                       | format.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#AD_HOC}

        -   #### AD_HOC

                public static final CodeSignIdentity AD_HOC

            ::: block
            A pseudo-identity for ad hoc code signing.
            See the [codesign man
            page](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/codesign.1.html).

            Binaries signed with this identity will not be installable
            on real devices. This is only intended for Buck unit tests.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CodeSignIdentity

                public CodeSignIdentity()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#ofAdhocSignedWithSubjectCommonName(java.lang.String)}

        -   #### ofAdhocSignedWithSubjectCommonName

            ``` methodSignature
            public static CodeSignIdentity ofAdhocSignedWithSubjectCommonName​(String commonName)
            ```

        []{#getFingerprint()}

        -   #### getFingerprint

            ``` methodSignature
            public abstract Optional<com.google.common.hash.HashCode> getFingerprint()
            ```

            ::: block
            Returns the identity\'s certificate hash, defined to be
            unique for each identity.
            If absent, this identity represents an ad-hoc signing
            identity.
            :::

        []{#getSubjectCommonName()}

        -   #### getSubjectCommonName

            ``` methodSignature
            public abstract String getSubjectCommonName()
            ```

            ::: block
            Returns the full name of the identity. e.g. \"iPhone
            Developer: John Doe (ABCDE12345)\"
            Not guaranteed to be unique.
            :::

        []{#shouldUseSubjectCommonNameToSign()}

        -   #### shouldUseSubjectCommonNameToSign

            ``` methodSignature
            public abstract boolean shouldUseSubjectCommonNameToSign()
            ```

            [Returns:]{.returnLabel}
            :   True if
                [`getSubjectCommonName()`](#getSubjectCommonName()) can
                be used to sign if
                [`getFingerprint()`](#getFingerprint()) is empty.

        []{#of(java.util.Optional,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static CodeSignIdentity of​(Optional<com.google.common.hash.HashCode> fingerPrint,
                                              String subjectCommonName)
            ```

        []{#of(java.util.Optional,java.lang.String,boolean)}

        -   #### of

            ``` methodSignature
            public static CodeSignIdentity of​(Optional<? extends com.google.common.hash.HashCode> fingerPrint,
                                              String subjectCommonName,
                                              boolean useSubjectCommonNameToSign)
            ```

        []{#toFingerprint(java.lang.String)}

        -   #### toFingerprint

            ``` methodSignature
            public static Optional<com.google.common.hash.HashCode> toFingerprint​(String identifier)
            ```

            ::: block
            Convert a `String` into a fingerprint `HashCode` if it\'s in
            the correct format.
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
