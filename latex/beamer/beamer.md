### beamer模版
* 捣腾了半天,写了个beamer模版,代码在此自己去看吧
```latex
% -*- coding:utf-8 -*-
\documentclass[11pt]{beamer}
\usepackage[space]{ctex}

%%%%%%%%%% 定义待使用的颜色%%%%%%%%%
\definecolor{seagreen}{RGB}{46, 139, 87}
\definecolor{darkstategray}{RGB}{47, 79, 79}
\definecolor{snow}{RGB}{205, 201, 201}
\definecolor{seashell}{RGB}{238, 229, 222}
\definecolor{antiquewhite}{RGB}{205, 192, 176}
\definecolor{darkmagenta}{RGB}{139, 0, 139}
\definecolor{darkblue}{RGB}{0, 0, 139}
%%%%%%%%%% 整个大标题的设置%%%%%%%%%
% 设置大标题的颜色和背景颜色，以及字体的控制。
\setbeamertemplate{title}{\vspace{-3mm}}
\setbeamercolor{title}{fg=seagreen, bg=white}
\setbeamerfont{title}{family=\rmfamily, series=\bfseries}

%%%%%%%%%% 帧标题的控制%%%%%%%%%%%%%
% 设置帧标题中心对齐，位置降低2.5mm。
\setbeamertemplate{frametitle}{\vspace{0mm}\centering\insertframetitle\par}
% 帧标题颜色为seagreen，背景为白色。
\setbeamercolor{frametitle}{fg=seagreen, bg=white}
% 帧标题字体的控制
\setbeamerfont{frametitle}{family=\sffamily, series=\bfseries, shape=\sffamily}

%%%%%%%%%%% 图表的标题%%%%%%%%%%%%%
% 给插图或者表添加序号。
\setbeamertemplate{caption}[numbered]
% 将图和表的字体改为强调字体
\setbeamerfont{caption}{family=\em}

%%%%%%%%%%% 文本的控制%%%%%%%%%%%%%
% 设置常规文本的颜色和背景色
\setbeamercolor{normal text}{fg=black, bg=white}
% 将强调的文本(使用\alert命令)颜色设为紫色
\setbeamercolor{alerted text}{fg=purple}

%%%%%%%%%%% 列表的控制%%%%%%%%%%%%
% 将常规列表的标志样式改为球形
\setbeamertemplate{itemize item}[ball]
\setbeamercolor{item}{fg=snow, bg=white}

%%%%%%%% 底边导航条的控制%%%%%%%%%
% wd为盒子的宽度, 下面的vspace*命令想要有效beamercolorbox必须带dp参数.
\setbeamertemplate{footline}{
  \vspace*{-4mm}{
    \leavevmode%
    \hbox{%
      \begin{beamercolorbox}[wd=0.25\paperwidth, ht=1ex, dp=1ex, center]{author in 
          head/foot}\usebeamerfont{author in head/foot} \color{seagreen}{\insertshortauthor}
      \end{beamercolorbox}%
      
      \begin{beamercolorbox}[wd=0.5\paperwidth, ht=1ex, dp=1ex, center]{title in 
          head/foot}\usebeamerfont{title in head/foot} \color{seagreen}{会议名字}
      \end{beamercolorbox}%

      \begin{beamercolorbox}[wd=0.25\paperwidth, ht=1ex, dp=1ex, center]{date 
          in head/foot} \usebeamerfont{date in head/foot} \color{seagreen}{\insertshortdate{}} 
        \hspace*{2.5mm} \color{darkblue}{\insertframenumber{}}
      \end{beamercolorbox}%
    }
    \vskip0pt}%
}

%%%%%%%%%% 设置目录颜色为黑%%%%%%%%%%%
\hypersetup{linkcolor=black}

%%%%%%%%%% 符号条的操作设置%%%%%%%%%%%
% \setbeamertemplate{navigation symbols}[only frame symbol]
% 如果看着不爽可以直接取消,取消的方式为
\setbeamertemplate{navigation symbols}{}    

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% 

\title{I am Title}
\author{金小海}
\institute{Shanghai Institute of Applied Physics, CAS}
\date{February 5, 2017}
\logo{}

\begin{document}

\begin{frame}
  \maketitle
\end{frame}

\begin{frame}
  \frametitle{Outline}
  \tableofcontents
\end{frame}

\section{旺财}
\begin{frame}
  \frametitle{憨睡的旺财}
  \begin{figure}[!ht]
    \centering
    \includegraphics[height=0.8\textheight, width=\textwidth]{./wangcai.jpg}
    % \caption{傻货}
    \label{fig:wangcai}
  \end{figure}
\end{frame}

\end{document}

%%% Local Variables:
%%% mode: latex
%%% TeX-master: t
%%% End:
```

> 补充下我是用xelatex编译的.
