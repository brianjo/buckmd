::: {#fb-root}
:::

::: topbar
[](http://buck.build/)

# Buck

-   
-   [Docs](/setup/getting_started.html)
-   [Issues](https://github.com/facebook/buck/issues)
-   [GitHub](https://github.com/facebook/buck)
:::

::: socialBanner
Support Ukraine. [Help Provide Humanitarian Aid to
Ukraine](https://opensource.fb.com/support-ukraine).
:::

::: hero
::: width
# A high-performance build tool

[Getting
Started](/setup/getting_started.html){.button} [GitHub](https://github.com/facebook/buck){.button}

![Chrome Tracing
Sample](/static/buck-build-15fps.gif){#super_console_sample}
:::
:::

::: {.section .content}
::: width
::: overview
Buck is a build system developed and used by Facebook. It encourages the
creation of small, reusable modules consisting of code and resources,
and supports a variety of languages on many platforms.

## Why Buck?

Buck can help you and your team in many ways:

-   **Speed up your builds.** Buck builds independent artifacts in
    parallel to take advantage of multiple cores on your machine.
    Further, it reduces incremental build times by keeping track of
    unchanged modules so that the minimal set of modules is rebuilt.
-   **Add reproducibility to your builds.** Buck only uses the declared
    inputs, which means everybody gets the same results.
-   **Get correct incremental builds.** Buck looks at the contents of
    your inputs, not their timestamps to figure out what needs to be
    built. As a result, incremental builds should always be correct, so
    there\'s no need to perform a clean build.
-   **Understand your dependencies.** With
    [`buck query`](/command/query.html), you can better understand your
    dependencies and what is required to build your product.
-   **Integrate with your IDE.** With
    [`buck project`](/command/project.html), your project can be better
    understood by your IDE, making you and your team more productive.
:::
:::
:::

::: width
© Copyright Facebook, 2013 - 2020
:::
