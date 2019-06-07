# WHUT Bachelor Thesis v 0.1b

=================================================================
## Introduction

This template is for undergraduate thesis at [Wuhan University of Techology](http://english.whut.edu.cn). 
LaTeX is a popular typesetting document preparation system in many scientific fields.
All questions and suggestions are welcomed, please file an issue in this repo.



## 简介
本模板是[武汉理工大学](http://www.whut.edu.cn)本科生毕业论文LaTeX免费模板。LaTeX是一个流行的编辑科学类文章的工具。
大多数科学类书籍，期刊，文章都采用了LaTeX。
使用这个模板可以使你从无聊的格式限制中解脱出来，从而更专注地阐述自己的想法。
希望本模板能够帮助你入门LaTeX, 如果你有关于本模板的良好意见和建议，请在顶栏的问题(issue)一栏中提出。


## 使用方法

* 建议使用[VS Code](https://code.visualstudio.com/)的[LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)插件进行编辑，编译链设置如下：
```
    "latex-workshop.latex.tools": [
        {
            // 编译工具和命令
            "name": "xelatex",
            "command": "xelatex",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "%DOCFILE%"
            ]
        },
        {
            "name": "biber",
            "command": "biber",
            "args": [
                "%DOCFILE%"
            ]
        },
        {
            "name": "bibtex",
            "command": "bibtex",
            "args": [
                "%DOCFILE%"
            ]
        }

    ],
    "latex-workshop.latex.recipes": [
        {
            "name": "xelatex",
            "tools": [
                "xelatex"
            ]
        },
        {
            "name": "xelatex -> bibtex -> xelatex*2",
            "tools": [
                "xelatex",
                "bibtex",
                "xelatex",
                "xelatex"
            ]
        },
    ]
```
* 设定主文档为`thesis.tex`，尝试进行编译


