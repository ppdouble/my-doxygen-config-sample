Follow link [how-to-use-doxyge    n-to-create-uml-class-diagrams-from-c-source](https://stackoverflow.com/questions/4755913/how-to-use-doxygen-to-create-uml-class-diagrams-from-c-source)

使用 doxygen 生成 UML 和 文档


**Edition**

fedora 29 workstation x86_64

doxygen-1.8.14-7.fc29.x86_64

graphviz-2.40.1-39.fc29.x86_64

`doxygen -g newconfigdoxygen.config`

修改生成的配置文件

```text
EXTRACT_ALL          = YES
CLASS_DIAGRAMS      = YES
HIDE_UNDOC_RELATIONS = NO
HAVE_DOT             = YES
CLASS_GRAPH          = YES
COLLABORATION_GRAPH  = YES
UML_LOOK             = YES
UML_LIMIT_NUM_FIELDS = 50
TEMPLATE_RELATIONS   = YES
DOT_GRAPH_MAX_NODES  = 100
MAX_DOT_GRAPH_DEPTH  = 0
DOT_TRANSPARENT      = YES
DOT_IMAGE_FORMAT = svg
INTERACTIVE_SVG = YES
OUTPUT_DIRECTORY       = relative
CREATE_SUBDIRS         = YES
```
更多使用方法 参照 `man doxygen`
