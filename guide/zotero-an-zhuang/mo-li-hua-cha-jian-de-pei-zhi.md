# 茉莉花插件的配置

比起其他的文献管理软件，原生的 Zotero 对中文支持并没有好到哪里去，但是得益于开源社区的维护，我们可以通过第三方 translator 库 [github.com/l0o0/translators\_CN](https://github.com/l0o0/translators\_CN) 极大的提高其中文文献抓取能力。

该库的主要维护者还开发了插件 [Jasminum - 茉莉花](https://github.com/l0o0/jasminum) 来继续增强 Zotero 的中文支持，茉莉花插件提供了如下功能：

> 1. 拆分或合并 Zotero 中条目作者姓和名
> 2. 根据知网上下载的文献文件来抓取引用信息（就是根据文件名）
> 3. 添加中文 PDF/CAJ 时，自动拉取知网数据，该功能默认关闭。需要到设置中开启，注意添加的文件名需要含有中文，全英文没有效果（还是根据文件名）
> 4. 为知网的学位论文 PDF 添加书签
> 5. 更新中文 translators
> 6. 拉取文献引用次数，是否核心期刊

就安装而言，

1. 下载安装 Jasminum 插件：在 [Latest Release · l0o0/jasminum (github.com)](https://github.com/l0o0/jasminum/releases/latest) 下载 `.xpi` 文件。在 Zotero——Tools——Add-ons——右上角小齿轮⚙——Install Add-on From File...——选中第二步保存的文件——确定——重启 Zotero。
2. 下载安装 PDFtk：下载并安装 [PDFtk server](https://www.pdflabs.com/tools/pdftk-server/) ，记录安装路径（eg. `C: \Program Files (x86)\PDFtk`）。在 Zotero——edit——Preferences——Jasminum——Setting——PDFtk Server Execute File Path 中填写 `<PDFtk install dir>/bin` （eg. `C: \Program Files (x86)\PDFtk\bin`）（即 PDFtk 可执行文件所在目录）。MAC 用户参考 [这里](https://github.com/l0o0/jasminum#%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8) 。
3. 安装中文 Translator：与上一步同一界面——Unofficial Translator Repository——Refresh——Update all。
4. 更新中文 Translator：打开已安装 Zotero Connector 的浏览器，右击 Zotero Connector 图标进入拓展选项，Advanced——Update Translators。
