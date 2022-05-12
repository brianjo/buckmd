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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.abi](package-summary.html)
:::

## Class SourceAbiCompatibleVisitor {#class-sourceabicompatiblevisitor .title title="Class SourceAbiCompatibleVisitor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.objectweb.asm.ClassVisitor

    -   -   com.facebook.buck.jvm.java.abi.SourceAbiCompatibleVisitor

::: description
-   

    ------------------------------------------------------------------------

        public class SourceAbiCompatibleVisitor
        extends org.objectweb.asm.ClassVisitor

    ::: block
    This class fixes up a few details of class ABIs so that they match
    the way source ABIs generate the same details. It allows us to take
    potentially risky shortcuts in source ABIs without losing the
    ability to verify them by binary comparison against class ABIs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.org.objectweb.asm.ClassVisitor}

            ### Fields inherited from class org.objectweb.asm.ClassVisitor

            `api, cv`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------- -------------
          `SourceAbiCompatibleVisitor​(org.objectweb.asm.ClassVisitor cv,                           AbiGenerationMode compatibilityMode)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                                                                                   Description
          ----------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                              `visit​(int version,      int access,      String name,      String signature,      String superName,      String[] interfaces)`           
          `org.objectweb.asm.FieldVisitor`    `visitField​(int access,           String name,           String desc,           String signature,           Object value)`                
          `void`                              `visitInnerClass​(String name,                String outerName,                String innerName,                int access)`               
          `org.objectweb.asm.MethodVisitor`   `visitMethod​(int access,            String name,            String desc,            String signature,            String[] exceptions)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.objectweb.asm.ClassVisitor}

            ### Methods inherited from class org.objectweb.asm.ClassVisitor

            `visitAnnotation, visitAttribute, visitEnd, visitModule, visitNestHost, visitNestMember, visitOuterClass, visitSource, visitTypeAnnotation`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(org.objectweb.asm.ClassVisitor,com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### SourceAbiCompatibleVisitor

                public SourceAbiCompatibleVisitor​(org.objectweb.asm.ClassVisitor cv,
                                                  AbiGenerationMode compatibilityMode)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visit(int,int,java.lang.String,java.lang.String,java.lang.String,java.lang.String[])}

        -   #### visit

            ``` methodSignature
            public void visit​(int version,
                              int access,
                              String name,
                              String signature,
                              String superName,
                              String[] interfaces)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `visit` in class `org.objectweb.asm.ClassVisitor`

        []{#visitMethod(int,java.lang.String,java.lang.String,java.lang.String,java.lang.String[])}

        -   #### visitMethod

            ``` methodSignature
            @Nullable
            public org.objectweb.asm.MethodVisitor visitMethod​(int access,
                                                               String name,
                                                               String desc,
                                                               String signature,
                                                               String[] exceptions)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `visitMethod` in class `org.objectweb.asm.ClassVisitor`

        []{#visitField(int,java.lang.String,java.lang.String,java.lang.String,java.lang.Object)}

        -   #### visitField

            ``` methodSignature
            public org.objectweb.asm.FieldVisitor visitField​(int access,
                                                             String name,
                                                             String desc,
                                                             String signature,
                                                             Object value)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `visitField` in class `org.objectweb.asm.ClassVisitor`

        []{#visitInnerClass(java.lang.String,java.lang.String,java.lang.String,int)}

        -   #### visitInnerClass

            ``` methodSignature
            public void visitInnerClass​(String name,
                                        String outerName,
                                        String innerName,
                                        int access)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `visitInnerClass` in
                class `org.objectweb.asm.ClassVisitor`
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
