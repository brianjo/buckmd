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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain](package-summary.html)
:::

## Class ProvisioningProfileMetadata {#class-provisioningprofilemetadata .title title="Class ProvisioningProfileMetadata"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.ProvisioningProfileMetadata

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class ProvisioningProfileMetadata
        extends Object
        implements AddsToRuleKey

    ::: block
    Metadata contained in a provisioning profile (.mobileprovision).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                   Description
          ------------------- --------------------------------------- -------------
          `static class `     `ProvisioningProfileMetadata.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                       Description
          --------------------------------- -------------
          `ProvisioningProfileMetadata()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `builder()`           |                       |
        | tatic ProvisioningPro |                       |                       |
        | fileMetadata.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getAppID()`          | ::: block             |
        |  Pair<String,​String>` |                       | Returns a (prefix,    |
        |                       |                       | identifier) pair for  |
        |                       |                       | which the profile is  |
        |                       |                       | valid.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.googl   | `getDeveloperCerti    | ::: block             |
        | e.common.collect.Immu | ficateFingerprints()` | SHA1 hashes of the    |
        | tableSet<com.google.c |                       | certificates in the   |
        | ommon.hash.HashCode>` |                       | \"De                  |
        |                       |                       | veloperCertificates\" |
        |                       |                       | section.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getEntitlements()`   | ::: block             |
        | ogle.common.collect.I |                       | Key/value pairs of    |
        | mmutableMap<String,​co |                       | the \"Entitlements\"  |
        | m.dd.plist.NSObject>` |                       | dictionary in the     |
        |                       |                       | embedded plist.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Date`       | `getExpirationDate()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getMer               |                       |
        | ogle.common.collect.I | geableEntitlements()` |                       |
        | mmutableMap<String,​co |                       |                       |
        | m.dd.plist.NSObject>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getPlatforms()`      | ::: block             |
        | ogle.common.collect.I |                       | The set of platforms  |
        | mmutableList<String>` |                       | the profile is valid  |
        |                       |                       | for.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getProfilePath()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getUUID()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `p                    | ::: block             |
        | tic Optional<String>` | refixFromEntitlements | Takes an ImmutableMap |
        |                       | ​(com.google.common.co | representing an       |
        |                       | llect.ImmutableMap<St | entitlements file,    |
        |                       | ring,​com.dd.plist.NSO | returns the           |
        |                       | bject> entitlements)` | application prefix if |
        |                       |                       | it can be inferred    |
        |                       |                       | from keys in the      |
        |                       |                       | entitlement.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `spli                 | ::: block             |
        |  Pair<String,​String>` | tAppID​(String appID)` | Takes a application   |
        |                       |                       | identifier and splits |
        |                       |                       | it into prefix and    |
        |                       |                       | bundle ID.            |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ProvisioningProfileMetadata

                public ProvisioningProfileMetadata()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAppID()}

        -   #### getAppID

            ``` methodSignature
            public abstract Pair<String,​String> getAppID()
            ```

            ::: block
            Returns a (prefix, identifier) pair for which the profile is
            valid.
            e.g. (ABCDE12345, com.example.TestApp) or (ABCDE12345, \*)
            :::

        []{#getExpirationDate()}

        -   #### getExpirationDate

            ``` methodSignature
            public abstract Date getExpirationDate()
            ```

        []{#getUUID()}

        -   #### getUUID

            ``` methodSignature
            public abstract String getUUID()
            ```

        []{#getProfilePath()}

        -   #### getProfilePath

            ``` methodSignature
            public abstract Path getProfilePath()
            ```

        []{#getPlatforms()}

        -   #### getPlatforms

            ``` methodSignature
            @Default
            public com.google.common.collect.ImmutableList<String> getPlatforms()
            ```

            ::: block
            The set of platforms the profile is valid for.
            :::

        []{#getEntitlements()}

        -   #### getEntitlements

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​com.dd.plist.NSObject> getEntitlements()
            ```

            ::: block
            Key/value pairs of the \"Entitlements\" dictionary in the
            embedded plist.
            :::

        []{#getDeveloperCertificateFingerprints()}

        -   #### getDeveloperCertificateFingerprints

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<com.google.common.hash.HashCode> getDeveloperCertificateFingerprints()
            ```

            ::: block
            SHA1 hashes of the certificates in the
            \"DeveloperCertificates\" section.
            :::

        []{#splitAppID(java.lang.String)}

        -   #### splitAppID

            ``` methodSignature
            public static Pair<String,​String> splitAppID​(String appID)
            ```

            ::: block
            Takes a application identifier and splits it into prefix and
            bundle ID.
            Prefix is always a ten-character alphanumeric sequence.
            Bundle ID may be a fully-qualified name or a wildcard ending
            in \*.
            :::

        []{#prefixFromEntitlements(com.google.common.collect.ImmutableMap)}

        -   #### prefixFromEntitlements

            ``` methodSignature
            public static Optional<String> prefixFromEntitlements​(com.google.common.collect.ImmutableMap<String,​com.dd.plist.NSObject> entitlements)
            ```

            ::: block
            Takes an ImmutableMap representing an entitlements file,
            returns the application prefix if it can be inferred from
            keys in the entitlement. Otherwise, it returns empty.
            :::

        []{#getMergeableEntitlements()}

        -   #### getMergeableEntitlements

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​com.dd.plist.NSObject> getMergeableEntitlements()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ProvisioningProfileMetadata.Builder builder()
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
