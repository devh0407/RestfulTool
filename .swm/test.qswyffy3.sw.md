---
title: test
---
asd

<p align="center"><img src="https://firebasestorage.googleapis.com/v0/b/swimmio-content/o/repositories%2FZ2l0aHViJTNBJTNBUmVzdGZ1bFRvb2wlM0ElM0FkZXZoMDQwNw%3D%3D%2Faec82943-aab3-44f8-9a18-03b06b8da01f.gif?alt=media&amp;token=9e4f75c5-9099-4d06-9dee-66b2e5db09e1"></p>

<SwmSnippet path="/src/com/github/restful/tool/actions/EditorOption.java" line="13">

---

import导包

```java
import com.intellij.openapi.actionSystem.AnActionEvent;
import com.intellij.openapi.actionSystem.LangDataKeys;
import com.intellij.openapi.editor.Editor;
import java.lang.String;
import com.intellij.psi.PsiElement;
import com.intellij.psi.PsiFile;
import org.jetbrains.annotations.NotNull;
import org.jetbrains.annotations.Nullable;
```

---

</SwmSnippet>

<SwmSnippet path="src/com/github/restful/tool/actions/EditorOption.java" line="28">

---

真正的按钮行为

```
    /**
     * 获取当前正在编辑行的elem
     *
     * @param e AnActionEvent
     * @return PsiElement
     * @since 2.0.0
     */
    @Nullable
    static PsiElement getCurrentEditorElement(@NotNull AnActionEvent e) {
        System.out.println("e" + e.toString);
        Editor editor = e.getData(LangDataKeys.EDITOR);
        if (editor == null) {
            return null;
        }
        PsiFile psiFile = e.getData(LangDataKeys.PSI_FILE);
        if (psiFile == null) {
            return null;
        }
```

---

</SwmSnippet>

<SwmSnippet path="/src/com/github/restful/tool/actions/EditorOption.java" line="38">

---

处理内容

```java
        Editor editor = e.getData(LangDataKeys.EDITOR);
        if (editor == null) {
            return null;
        }
```

---

</SwmSnippet>

<SwmSnippet path="/src/com/github/restful/tool/actions/RefreshAction.java" line="27">

---

test

```java
        RightToolWindow toolWindow = RestfulToolWindowFactory.getToolWindow(e.getProject());
        if (toolWindow == null) {
            return;
        }
```

---

</SwmSnippet>

<SwmMeta version="3.0.0" repo-id="Z2l0aHViJTNBJTNBUmVzdGZ1bFRvb2wlM0ElM0FkZXZoMDQwNw==" repo-name="RestfulTool"><sup>Powered by [Swimm](https://app.swimm.io/)</sup></SwmMeta>
