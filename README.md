# ructhesis  

**如果已经有ructhesis.cls文件的可以直接使用。**  

在main.tex文件下使用如下命令：  

这里我们使用xelatex作为引擎，第一步为编译main.tex文件，第二步处理参考文献，然后再编译两遍生成pdf文件  

`$ xelatex main.tex`  
`$ bibtex main.tex`  
`$ xelatex main.tex`  
`$ xelatex main.tex` 

###必要的字体文件

- Times New Roman  PostScript名称：TimesNewRomanPSMT   
- Arial PostScript名称：ArialMT  
- Courier New  PostScript名称：CourierNewPSMT  
- 宋体  PostScript名称：SimSun  
- 黑体  PostScript名称：SimHei  
- 仿宋  PostScript名称：FangSong  

**需要生成封皮的还需要自行下载安装**  
方正小标宋字体 PostScript名称:FZXBSJW–GB1-0

###必要的宏包
**全部都是TeX Live自带的**
- ctexbook
- geometry
- hyperref
- graphicx
- titletoc
- ifxetex
- ifthen
- calc
- lscape
- multicol
- color
- pstricks

###想编译模板文件和生成手册的可以执行下述代码
生成模板文件ructhesis.cls  
`$ latex ructhesis.ins`  
生成手册ructhesis.pdf  
`$ xelatex ructhesis.dtx`  
`$ makeindex -s gind.ist -o ructhesis.ind ructhesis.idx `  
`$ makeindex -s gglo.ist -o ructhesis.gls ructhesis.glo `  
`$ xelatex ructhesis.dtx`  
`$ xelatex ructhesis.dtx`  

###联系  
如果模板本身的问题可以上[GitHub](https://github.com/ZebinWang/ructhesis)上发一篇issue。   
如果想贡献代码的请联系我<email:me@zebinwang.com>

