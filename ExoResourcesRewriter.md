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
[Package]{.packageLabelInType} [com.facebook.buck.android.resources](package-summary.html)
:::

## Class ExoResourcesRewriter {#class-exoresourcesrewriter .title title="Class ExoResourcesRewriter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.resources.ExoResourcesRewriter

::: description
-   

    ------------------------------------------------------------------------

        public class ExoResourcesRewriter
        extends Object

    ::: block
    ExoResourceRewriter is the core of constructing build outputs for
    exo-for-resources.
    Some background: Android\'s resources are packaged into the APK
    primarily in the resources.arsc file with some references out to
    other files in the APK\'s res/ directory (.png/.xml mostly). The
    resources.arsc file is a binary file in a format that isn\'t really
    well documented, but you can get a good idea of its structure by
    looking at ResourceTable and other classes in this package. At
    runtime, Android constructs an AssetManager from the APK and
    resource lookups go through that. While this is primarily done for
    an app\'s own resources, the framework may construct one to access
    an app\'s resources directly (e.g. for driving animations, for
    intent pickers, etc) and apps can access resources of other apps
    (e.g. a launcher app will access names/icons).

    For exo-for-resources, we determine a minimal set of resources
    (including referenced files) that need to be in the main APK. This
    set includes all resources referenced from the AndroidManifest.xml
    or from any animation. We construct a resources.arsc for these
    resources and then the primary apk includes those resources. To
    avoid odd issues, we rewrite the full resources.arsc and all
    compiled .xml files such that references match between the primary
    apk and the exo resources (and without this, we have run into
    issues).

    For assets, we don\'t package any into the main apk. For exo
    resources, assets are put into a separate zip from the exo .arsc
    (and resource files).

    TODO(cjhopman): The underlying c++ resource handling supports some
    things that we should take advantage of. First, we are able to
    easily have multiple resource apks (including multiple .arsc with
    the same package id) as long as we don\'t have the same
    package-id/type-id pair in different .arsc files. Second, there\'s
    no restriction that all resources of the same type actually have the
    same type id (e.g. we could have strings with type id 0x01, 0x02,
    and 0x03). I\'m pretty sure that aapt\'s
    \--feature-of/\--feature-after work by using different type ids for
    the same type.

    Using these, we should be able to split resources across some larger
    number of .zips in such a way that users will typically only need to
    install a small number of resources (for example, in a particular
    large app that I\'ve looked at, a vast majority of resource size is
    spent on just the \'strings\' type). It\'s probably also possible
    for us to construct multiple top-level aapt targets that handle
    smaller subsets of the resources (e.g. construct a separate
    \'strings\' top-level aapt rule). While it would be hard to
    construct multiple aapt rules for a particular type (adding
    restrictions on resource overriding would make it easier) we could
    still easily split a particular type into multiple exo resources
    zips (using different type ids).

    It might be possible to get even more ids to work by using a
    different package id (other than 0x7f). I believe the package id
    space is partitioned like so:

    -   0x01- framework
    -   0x02 - 0x7f - potentially any of these are used by OEM overlays.
        OEM overlays, just like the framework, will be loaded into the
        zygote.
    -   0x7f - the app
    -   0x80 and above - (KK+) dynamically loaded resource libraries
        (like GMS and WebView resources), some of these get loaded after
        your process starts by the framework code that processes your
        apps AndroidManifest, the WebView resources get loaded at
        runtime, the first time you new up a WebView instance.

    As the normal Android build system doesn\'t use anything other than
    0x7f, and that\'s always been the only package id used by
    applications, and that we have some leeway in the type id space, I
    didn\'t think it was worth it now to further investigate the
    feasibility/difficulty of using different package ids.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                   Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static void`       `rewrite​(Path inputPath,        Path inputRDotTxt,        Path primaryResources,        Path exoResources,        Path outputRDotTxt)`    

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
    -   []{#method.detail}

        ### Method Detail

        []{#rewrite(java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path)}

        -   #### rewrite

            ``` methodSignature
            public static void rewrite​(Path inputPath,
                                       Path inputRDotTxt,
                                       Path primaryResources,
                                       Path exoResources,
                                       Path outputRDotTxt)
                                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
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
