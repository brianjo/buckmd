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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.test.selectors {#package-com.facebook.buck.test.selectors .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [TestSelector](                   | ::: block                         |
    | TestSelector.html "interface in c | A way of matching a test-method   |
    | om.facebook.buck.test.selectors") | in a test-class, and saying       |
    |                                   | whether or not to include any     |
    |                                   | matches in a test run.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [PatternTestSelector](Pat         | ::: block                         |
    | ternTestSelector.html "class in c | A                                 |
    | om.facebook.buck.test.selectors") | [`TestDescription`]               |
    |                                   | (TestDescription.html "class in c |
    |                                   | om.facebook.buck.test.selectors") |
    |                                   | will match if this selector\'s    |
    |                                   | class-part is a substring of the  |
    |                                   | [`TestDescription`](Te            |
    |                                   | stDescription.html "class in com. |
    |                                   | facebook.buck.test.selectors")\'s |
    |                                   | full class-name, or if this       |
    |                                   | selector\'s class-name, when      |
    |                                   | interpreted as a java.util.regex  |
    |                                   | regular-expression, matches the   |
    |                                   | [`TestDescription`](Te            |
    |                                   | stDescription.html "class in com. |
    |                                   | facebook.buck.test.selectors")\'s |
    |                                   | full class-name.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SimpleTestSelector](Si           | ::: block                         |
    | mpleTestSelector.html "class in c | A                                 |
    | om.facebook.buck.test.selectors") | [`TestDescription`]               |
    |                                   | (TestDescription.html "class in c |
    |                                   | om.facebook.buck.test.selectors") |
    |                                   | will match if this selector\'s    |
    |                                   | class-part is identical to the    |
    |                                   | TestDescriptions class name (same |
    |                                   | for the method name).             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestDescription]                 | ::: block                         |
    | (TestDescription.html "class in c | A non-JUnit specific way of       |
    | om.facebook.buck.test.selectors") | describing a test-method inside a |
    |                                   | test-class.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestSelectorList](               | ::: block                         |
    | TestSelectorList.html "class in c | A collection of                   |
    | om.facebook.buck.test.selectors") | [`PatternTestSelector`](Pat       |
    |                                   | ternTestSelector.html "class in c |
    |                                   | om.facebook.buck.test.selectors") |
    |                                   | instances which, as a group, can  |
    |                                   | decide whether or not to include  |
    |                                   | a given                           |
    |                                   | [`TestDescription`](              |
    |                                   | TestDescription.html "class in co |
    |                                   | m.facebook.buck.test.selectors"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [T                                | ::: block                         |
    | estSelectorList.Builder](TestSele | Build a new                       |
    | ctorList.Builder.html "class in c | [`TestSelectorList`](             |
    | om.facebook.buck.test.selectors") | TestSelectorList.html "class in c |
    |                                   | om.facebook.buck.test.selectors") |
    |                                   | from a list of strings, each of   |
    |                                   | which is parsed by                |
    |                                   | [`PatternTestSelector`](Patt      |
    |                                   | ernTestSelector.html "class in co |
    |                                   | m.facebook.buck.test.selectors"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [TestS                            | ::: block                         |
    | electorParseException](TestSelect | Errors specific to parsing test   |
    | orParseException.html "class in c | selectors.                        |
    | om.facebook.buck.test.selectors") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Annotation Type                   | Description                       |
    +===================================+===================================+
    | [Nullabl                          | ::: block                         |
    | e](Nullable.html "annotation in c | Defining \@Nullable locally here  |
    | om.facebook.buck.test.selectors") | because we cannot import          |
    |                                   | javax.annotation.Nullable;        |
    |                                   | according to comment in           |
    |                                   | src/com/                          |
    |                                   | facebook/buck/test/selectors/BUCK |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Annotation Types Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
