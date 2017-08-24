#### 希腊字母的latex整理
```latex
% #-*- coding:utf-8 -*-
\documentclass[8pt]{beamer}
\usepackage[space]{ctex}
\begin{document}

%%%%%%%%%%整个大标题的设置%%%%%%%%%
\definecolor{seagreen}{RGB}{46, 139, 87}
\setbeamercolor{title}{fg=seagreen, bg=white}
\setbeamerfont{title}{family=\rmfamily, series=\bfseries, size=\huge}

%设置帧标题中心对齐，位置降低2mm。
\setbeamertemplate{frametitle}{\vspace{2mm}\centering\insertframetitle\par}

\title{I am Title}
\author{\large{Jin Xiaohai}}
\institute{\large{Shanghai Institute of Applied Physics, CAS}}
\date{\large{2017/08/24}}
\logo{}

\begin{frame}
\maketitle
\end{frame}


\begin{frame}
  \frametitle{目录页}
  \tableofcontents
\end{frame}


\section{greek}
\begin{frame}
  \frametitle{The greeks letters}
  \begin{columns}%[onlytextwidth]
    \begin{column}{0.5\textwidth}
      \begin{tabbing}
        \color{red}{\heiti latex command} \hspace{6mm} \= \color{pink}{\heiti lower} \hspace{6mm} \= \color{green}{\heiti upper}\\
        $\backslash$alpha         \>              $\alpha$                 \>               \\
        $\backslash$beta          \>              $\beta$                  \>               \\
        $\backslash$gamma         \>              $\gamma$                 \>               \\
        $\backslash$delta         \>              $\delta$                 \> $\Delta$      \\
        $\backslash$epsilon       \>              $\epsilon$               \>               \\
        $\backslash$varepsilon    \>              $\varepsilon$            \>               \\
        $\backslash$zeta          \>              $\zeta$                  \>               \\
        $\backslash$eta           \>              $\eta$                   \>               \\
        $\backslash$eta           \>              $\eta$                   \>               \\
        $\backslash$theta         \>              $\theta$                 \> $\Theta$      \\
        $\backslash$vartheta      \>              $\vartheta$              \>               \\
        $\backslash$iota          \>              $\iota$                  \>               \\
        $\backslash$kappa         \>              $\kappa$                 \>               \\
        $\backslash$lambda        \>              $\lambda$                \> $\Lambda$      \\
        $\backslash$mu            \>              $\mu$                    \>                \\
      \end{tabbing}
    \end{column}
    \begin{column}{0.5\textwidth}
      \begin{tabbing}
        \color{red}{\heiti latex command} \hspace{6mm} \= \color{pink}{\heiti lower} \hspace{6mm} \= \color{green}{\heiti upper}\\
        $\backslash$nu            \>              $\nu$                    \>               \\
        $\backslash$xi            \>              $\xi$                    \> $\Xi$         \\
        $\backslash$pi            \>              $\pi$                    \> $\Pi$         \\
        $\backslash$varpi         \>              $\varpi$                 \> \\
        $\backslash$rho           \>              $\rho$                   \> \\
        $\backslash$varrho        \>              $\varrho$                \>  \\
        $\backslash$sigma         \>              $\sigma$                 \> $\Sigma$ \\
        $\backslash$varsigma      \>              $\varsigma$              \> \\
        $\backslash$tau           \>              $\tau$                    \> \\
        $\backslash$upsilon       \>              $\upsilon$                \> $\Upsilon$ \\
        $\backslash$phi           \>              $\phi$                    \> $\Phi$ \\
        $\backslash$varphi        \>              $\varphi$                \> \\
        $\backslash$chi           \>              $\chi$                   \> \\
        $\backslash$psi           \>              $\psi$                   \> $\Psi$ \\
        $\backslash$omega         \>              $\omega$                  \> $\Omega$ \\
      \end{tabbing}
    \end{column}
  \end{columns}
\end{frame}
\end{document}

%%% Local Variables:
%%% mode: latex
%%% TeX-master: t
%%% End:

```
