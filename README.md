# 中南大学硕士学位论文模板 A LATEX template for master thesis submitted to Central South University

## 编译
需要使用 [texlive 2020](https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/) 以上版本编译。*如果用其他低版本的 texlive，则需要将dissertation.tex文件中第29行的`\xeCJKsetup{AutoFakeBold=2.5}`注释掉，否则生成的pdf无法正常复制，影响查重*。 

主文件是dissertation.tex，编译 dissertation.tex 文件便可以得到pdf。
## 正文内容
将 dissertation.tex中的论文作者标题（第186-209行）替换成自己的论文信息，摘要需在abstract.tex中直接修改，正文在 chapter1.tex、chapter2.tex、chapter3.tex、chapter4.tex、chapter5.tex 等文件修改。
## 参考文献
本模板采用bibtex生成参考文献，模板使用了[Zeping Lee](https://github.com/CTeX-org/gbt7714-bibtex-style)制作的bibtex样式，所引用的文献格式会自动按照gbt7714格式编排，不需要手工调整。只需要在bibfile.bib文件中添加文献词条，便可引用。例如在bibfile.bib中包含以下词条：
```
@book{blakely1996potential,
	title={Potential theory in gravity and magnetic applications},
	author={Blakely, Richard J},
	year={1996},
	address={Cambridge},
	publisher={Cambridge university press}
}
```
在正文中可以这样引用：
```
重力方法是一种重要的地球物理勘探方法\cite{blakely1996potential}......
```
那么在生成的pdf中便会显示：
```
重力方法是一种重要的地球物理勘探方法[1]......
```
与此同时，pdf中的参考文献列表自动生成以下内容：
```
[1] Blakely R J. Potential theory in gravity and magnetic applications[M]. Cambridge:
Cambridge university press, 1996.
```
> 注意：1. latex会根据引用文献在文中出现的顺序，自动确定该文献的编号，无需使用者手动设置。
>    2.  通过百度学术、bing 学术、google scholar可以直接导出成 *.bib 文件需要的文献词条格式

## LaTeX资源链接
- [LaTeX安装教程](https://github.com/OsbertWang/install-latex/releases/download/v2020.7.1/Install-LaTeX.pdf)
- [110 分钟了解LaTeX](https://mirrors.tuna.tsinghua.edu.cn/CTAN/info/lshort/chinese/lshort-zh-cn.pdf)
- [中南大学开题报告LaTex模板](https://github.com/zhong-yy/CSU_Thesis_Proposal)
