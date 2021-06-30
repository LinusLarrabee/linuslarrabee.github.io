---
layout: post
title: Latex基本跨栏操作
subtitle:   以IEEEtrans模版为例
date:       2021-01-17
author:     SH
header-img: img/post-bg-ios9-web.jpg
categories: "work"
catalog: true
tags:
    - latex
    - work
---

图片跨栏示例

```latex
\begin{strip}
\centering\includegraphics[width=0.3\textwidth]{schematic.png}%schematic.png为图片名
\captionof{figure}{Schematic diagram of a ghost imaging system}
\end{strip}
```

图片单栏示例

```latex
\begin{figure}[H] %H为当前位置，!htb为忽略美学标准，htbp为浮动图形
\centering %图片居中
\includegraphics[width=0.3\textwidth]{schematic.png} %插入图片，[]中设置图片大小，{}中是图片文件名
\caption{Main name 2} %最终文档中希望显示的图片标题
\label{Fig.main2} %用于文内引用的标签
\end{figure}
```

公式跨栏示例

```latex
\begin{strip}
\begin{align}
I_0(y,X|a)=-\int dyp(y|a)lnp(y|a)+\int dX\int dyp(y,X|a)ln(p|X,a)
\end{align}
\end{strip}
```

