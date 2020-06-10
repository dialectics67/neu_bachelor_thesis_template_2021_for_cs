## 东北大学本科毕业论文 latex模板 2020
--------------
修改自一位学长的[neu_bachelor_thesis_template](https://github.com/Acytoo/neu_bachelor_thesis_template)。

***以下来自[neu_bachelor_thesis_template](https://github.com/Acytoo/neu_bachelor_thesis_template)。***

---------------
### 使用方法
* `make`    生成论文 main.pdf；
* `make view`    生成论文 main.pdf 并查看生成的论文；
* `make clean`     删除中间文件（不含 main.pdf）；
* `make cleanall`  删除中间文件和生成的论文（main.pdf）；
----------------

--------------------
### 注意

* 请使用xelatex

* 可能需要手动安装参考文献的标准，具体的安装方式请见[GBT7714-2005参考文献标准](https://github.com/Haixing-Hu/GBT7714-2005-BibTeX-Style)。使用GBT7714-2005参考文献标准，请删除cls文件中348行```\bibliographystyle{gbt7714-2005} ```前的注释。

* 如果你的目录页共有奇数页，一定要在目录后面加入一个空白页，或者将目录与正文分开打印，否则正文的第一页可能被打印在目录页的背面。

* 自定义添加图片，表格，记得修改字号为5号。

* 如果缺少相应的字体可能会无法编译或者编译结果与预期不同（虽然这种情况通常不会出现），请自行安装相应的字体。

* 附录里的代码使用了Monaco字体，如果你的电脑没有安装这种字体，可以在这里[下载](https://github.com/todylu/monaco.ttf)安装，或者删掉[cls](https://github.com/Acytoo/neu_bachelor_thesis_template/blob/master/csethesis.cls)文件中，代码段字体的设置项。

* 关于章标题的上下间距，可以参考这个issue:[设置每章的标题的上下间距在哪里可以调整？](https://github.com/ustctug/ustcthesis/issues/102)

***以上来自[neu_bachelor_thesis_template](https://github.com/Acytoo/neu_bachelor_thesis_template)。***

### 解决了的问题

* 解决了windows上章标题上下间距不正确的问题

* 使用无法理解的方法解决了windows下郑重声明和三级标题未加粗的问题

* 修改了图表标题后有冒号的问题

* 将代码修改为能直接插入正文的格式（而非附录）

* 提供了一种临时的解决参考文献/致谢页页眉问题的方法

### 新的注意

* 非windows操作系统可能会引入新的问题

* 封面格式若有明显差异，请尝试直接用学校的模板然后与本模板输出合并

* 默认设置下参考文献/致谢页会多一个章号，暂无完美解决方案，临时的解决方案先输出一个原pdf文件，然后将csethesis.cls中87行的代码替换为86行注释内代码并输出一个新pdf文件，最后将原PDF文件的正文部分与新pdf文件的参考文献/致谢页合并

### 新的使用方法

* 在[这里](https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/)下载texlive并安装，安装过程会很慢，请耐心等候

* 在vscode的拓展中搜索并安装LaTeX Workshop即可使用
