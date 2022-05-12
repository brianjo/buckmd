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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.go](package-summary.html)
:::

## Enum GoOs {#enum-goos .title title="Enum GoOs"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[GoOs](GoOs.html "enum in com.facebook.buck.features.go")\>

    -   -   com.facebook.buck.features.go.GoOs

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<GoOs>`

    ------------------------------------------------------------------------

        public enum GoOs
        extends Enum<GoOs>

    ::: block
    Represents the GOOS values in Go found at:
    https://github.com/golang/go/blob/master/src/go/build/syslist.go
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `AIX`            
          `ANDROID`        
          `DARWIN`         
          `DRAGONFLY`      
          `FREEBSD`        
          `HURD`           
          `JS`             
          `LINUX`          
          `NACL`           
          `NETBSD`         
          `OPENBSD`        
          `PLAN9`          
          `SOLARIS`        
          `WINDOWS`        
          `ZOS`            

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static GoOs`         | `fromPlatfor          | ::: block             |
        |                       | m​(Platform platform)` | returns the           |
        |                       |                       | corresponding GoOs    |
        |                       |                       | for a given Platform  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static GoOs`         | `fro                  | ::: block             |
        |                       | mString​(String name)` | Finds the GoOs from   |
        |                       |                       | it\'s name.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getEnvVarValue()`    | ::: block             |
        |                       |                       | Returns the           |
        |                       |                       | environment variable  |
        |                       |                       | to be used for GOOS   |
        |                       |                       | to Go tools.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static GoOs`         | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static GoOs[]`       | `values()`            | ::: block             |
        |                       |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#AIX}

        -   #### AIX

                public static final GoOs AIX

        []{#ANDROID}

        -   #### ANDROID

                public static final GoOs ANDROID

        []{#DARWIN}

        -   #### DARWIN

                public static final GoOs DARWIN

        []{#DRAGONFLY}

        -   #### DRAGONFLY

                public static final GoOs DRAGONFLY

        []{#FREEBSD}

        -   #### FREEBSD

                public static final GoOs FREEBSD

        []{#HURD}

        -   #### HURD

                public static final GoOs HURD

        []{#JS}

        -   #### JS

                public static final GoOs JS

        []{#LINUX}

        -   #### LINUX

                public static final GoOs LINUX

        []{#NACL}

        -   #### NACL

                public static final GoOs NACL

        []{#NETBSD}

        -   #### NETBSD

                public static final GoOs NETBSD

        []{#OPENBSD}

        -   #### OPENBSD

                public static final GoOs OPENBSD

        []{#PLAN9}

        -   #### PLAN9

                public static final GoOs PLAN9

        []{#SOLARIS}

        -   #### SOLARIS

                public static final GoOs SOLARIS

        []{#WINDOWS}

        -   #### WINDOWS

                public static final GoOs WINDOWS

        []{#ZOS}

        -   #### ZOS

                public static final GoOs ZOS
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static GoOs[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (GoOs c : GoOs.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static GoOs valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null

        []{#getEnvVarValue()}

        -   #### getEnvVarValue

            ``` methodSignature
            public String getEnvVarValue()
            ```

            ::: block
            Returns the environment variable to be used for GOOS to Go
            tools.
            :::

        []{#fromString(java.lang.String)}

        -   #### fromString

            ``` methodSignature
            public static GoOs fromString​(String name)
                                   throws NoSuchElementException
            ```

            ::: block
            Finds the GoOs from it\'s name.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - name of the GoOS as defined from Go itself

            [Returns:]{.returnLabel}
            :   GoOs for the matching name

            [Throws:]{.throwsLabel}
            :   `NoSuchElementException`

        []{#fromPlatform(com.facebook.buck.util.environment.Platform)}

        -   #### fromPlatform

            ``` methodSignature
            public static GoOs fromPlatform​(Platform platform)
                                     throws HumanReadableException
            ```

            ::: block
            returns the corresponding GoOs for a given Platform
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - the
                [`Platform`](../../util/environment/Platform.html "enum in com.facebook.buck.util.environment")
                to lookup

            [Returns:]{.returnLabel}
            :   GoOs for the matching platform

            [Throws:]{.throwsLabel}
            :   `HumanReadableException` - when a specific GoOS is not
                found for the Platform
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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
