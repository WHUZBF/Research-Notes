# Research-Notes

有趣的文献都在这里了，顺带一点文献背后有意思的数学和物理

# 目录

在这里放个目录，算是Todo list:

## 流体引力对偶

- [ ] 流体力学简介（hydrodynamics极限）

- [ ] 经典的流体引力对偶

- [ ] 利用经典double copy做流体Maxwell对偶

- [ ] NSE与散射振幅

## 纠缠熵与散射振幅

- [ ] Clifford Cheung 的天才想法（等学长毕业论文写完了补）
- [ ] 张量网络
- [ ] 量子信息张量网络方法计算微扰散射理论中纠缠熵的变化

## 黑洞

只计划搞点经典的黑洞，然后提一下量子效应
- [ ] 球对称施瓦西解
- [ ] 黑洞与时空奇点
- [ ] 施瓦西黑洞
- [ ] 带电球对称你黑洞
- [ ] 克尔黑洞
- [ ] 黑洞热力学（从热力学类比出发，提一下半经典引力可证明黑洞真的有热辐射）
- [ ] 全息原理 （argue一下黑洞信息悖论，无毛定理啥的，重点是说熵正比于面积而不是体积，说明信息被编码在黑洞表面，暗示着引力和边界上低一维场论的对偶）

## AdS/CFT对应

只打算搞点不涉及到弦论的，或者说只求知道字典，会计算，知道个大概物理图像
- [ ] 大$N$展开
- [ ] 形而上与形而下

## 超对称

- [ ] 标准模型
- [ ] 超对称代数与超空间（使用srednicki的记号）
- [ ] Wess-Zumino模型

## p-adic

## 计算代数几何及其在物理中的应用

这部分看张扬老师讲义写个备忘录就好

可以先写这个

- [ ] overview，对江云峰老师的讲座给个笔记

## 费曼图花式计算技巧

接上面一章节

这个先不急，感觉可以从头看书学，先写写Baikov形式

- [ ] IBP
- [ ] 微分方程法
- [ ] Baikov形式

## 物理疑难杂症

- [ ] 量子场论中的散射到底是什么？（这里我想讲清楚真空态到底属于什么绘景？渐近态是什么？粒子态是怎么构造出来的（不是从poincare表示出发，而是考虑QFT的希尔伯特空间）以及散射振幅$\mathcal{S}$矩阵到底怎么定义的？）


## 数学疑难杂症

- [x] 为啥要有张量积？直积直和到底有啥区别？内外直和又是什么？（限于线性空间的讨论） 

- [ ] 格拉斯曼几何

- [x] 李超代数

- [x] 随机矩阵

  

# LaTeX 模板

本笔记用[李文威老师的代数学方法模板](https://github.com/wenweili/AlJabr-1)写成

不知道为啥，直接copy这个模板编译时会显示字体缺失：

```latex
Template-AJbook.tex: 错误: 79: Package fontspec Error: The font "Noto Sans CJK SC" cannot be found. ^^I\frontmatter
```

在这个网址[notofonts/noto-cjk: Noto CJK fonts (github.com)](https://github.com/notofonts/noto-cjk)下载字体安装就好，注意要右键选择“为所有用户安装”，然后再在命令行输入：

```powershell
fc-cache
```

清空缓存，输入：

```
fc-list -f "%{family}\n" :lang=zh-cn >d:\list.txt
```

查询已安装字体名称，如果字体名称引用不一致要更改代码，见[知乎回答](https://zhuanlan.zhihu.com/p/495831411#:~:text=%E5%9C%A8Windows%E5%91%BD%E4%BB%A4%E7%AA%97%E5%8F%A3%E4%B8%AD%E8%BE%93%E5%85%A5fc-cache%20%E5%91%BD%E4%BB%A4%E5%88%B7%E6%96%B0%E5%AD%97%E4%BD%93%E7%BC%93%E5%AD%98%E5%90%8E%E5%86%8D%E5%B0%9D%E8%AF%95%E3%80%82%20%E5%A6%82%E6%9E%9C%E4%BD%A0%E5%AE%89%E8%A3%85%E4%BA%86%E8%BE%83%E5%A4%9A%E5%AD%97%E4%BD%93%EF%BC%8C%E5%88%B7%20%E6%96%B0%E5%8F%AF%E8%83%BD%E8%BE%83%E6%85%A2%E3%80%82%20%E5%A6%82%E6%9E%9C%E5%88%B7%E6%96%B0%E7%BC%93%E5%AD%98%E6%97%A0%E6%95%88%EF%BC%8C%E8%80%83%E8%99%91%E9%87%8D%E6%96%B0%E5%AE%89%E8%A3%85%E5%AF%B9%E5%BA%94%E7%9A%84%E5%AD%97%E4%BD%93%E3%80%82,%E6%B3%A8%E6%84%8F%E5%9C%A8%E5%AE%89%E8%A3%85%E5%AD%97%E4%BD%93%E6%97%B6%EF%BC%8C%E9%80%9A%E8%BF%87%20%E5%8F%B3%E9%94%AE%E7%82%B9%E5%87%BB%EF%BC%88%E8%80%8C%E4%B8%8D%E6%98%AF%E5%8F%8C%E5%87%BB%E6%89%93%E5%BC%80%EF%BC%89%E5%AD%97%E4%BD%93%E6%96%87%E4%BB%B6%EF%BC%8C%E7%84%B6%E5%90%8E%E9%80%89%E6%8B%A9%E2%80%9C%E4%B8%BA%E6%89%80%E6%9C%89%E7%94%A8%E6%88%B7%E5%AE%89%E8%A3%85%E2%80%9D%E3%80%82%20%E5%A6%82%20%E6%9E%9C%E5%8F%8C%E5%87%BB%E5%AD%97%E4%BD%93%E6%96%87%E4%BB%B6%E5%90%8E%E5%AE%89%E8%A3%85%EF%BC%8C%E5%8F%AF%E8%83%BD%E4%BC%9A%E5%AF%BC%E8%87%B4%20LaTeX%20%E4%BB%8D%E7%84%B6%E6%97%A0%E6%B3%95%E6%89%BE%E5%88%B0%E5%AD%97%E4%BD%93%E3%80%82)。

但是这个时候依旧会报错：

```
Template-AJbook.tex: 错误: 85: Package fontspec Error: The font "Noto Sans CJK SC Black" cannot be found. ^^I\section*{简要说明}
```

两个小时之后我终于找到了问题，前面那个网址下载的字体不知道为啥不同字形的引用名相同，所以需要去[noto-cjk/Sans/OTF/SimplifiedChinese at main · notofonts/noto-cjk (github.com)](https://github.com/notofonts/noto-cjk/tree/main/Sans/OTF/SimplifiedChinese)下载安装所需要的三种字体，regular，black和medium。然后分别点击右键择“为所有用户安装”，然后用下面代码刷新三次：

```powershell
fc-cache
```
再利用
```
fc-list -f "%{family}\n" :lang=zh-cn >d:\list.txt
```
这个时候字体引用名就不同了，分开成了三个，最后再用：
```powershell
fc-cache -fsv
```
刷新三次，然后就能正常编译了。但是这个时候章节名称字体还是有问题，不是黑体，需要在titles-setup.tex文件中：

```latex
% 用 titlesec 设置各章标题
\titleformat{name=\chapter}
	{\filright\sffamily\CJKfamily{hei2}\bfseries\Huge}	% Format
	{}	% Label
	{0mm}	% Sep
	{\MakeChapBox{\thechapter}{#1}}	% Before-code
	[]	% After-code
\titlespacing*{name=\chapter}	% 设置间隔
	{1pc}{*4}{1em}	% {left}{before-sep}{after-sep}

\titleformat{name=\chapter, numberless}
	{\filcenter\sffamily\CJKfamily{hei2}\bfseries\Huge}	% Format
	{}	% Label
	{0mm}	% Sep
	{\MakeChapBoxSingle{#1}}	% Before-code
	[{\if@mainmatter
		\addcontentsline{toc}{chapter}{#1}
		\markboth{#1}{}
	\fi}]	% After-code: 无号章如果出现在正文中, 就加入目录并相应地设置天眉.
```

将上面这一段中的hei2全部改为sectionfont，字体的设置就完全和GitHub上的模板pdf一模一样了。

然后是索引和参考文献的问题，我这里索引目录出现了两次，不过我不需要，所以索引我完全去掉了，但是参考文献的生成还要琢磨一下，进入AJbook.cls文件，将其中的：

```latex
% 使用 biblatex + biber 制作书目
\RequirePackage[backend=biber, hyperref=auto, backref=true, backrefstyle=three]{biblatex}
```

中的backend参数改为bibtex即可。