\documentclass[oneside,english]{amsart}
\usepackage[T1]{fontenc}
\usepackage[latin9]{inputenc}
\usepackage{mathrsfs}
\usepackage{amstext}
\usepackage{amsthm}
\usepackage{amssymb}
\usepackage[none]{hyphenat}
\usepackage[T1]{fontenc}
\theoremstyle{definition}
\newtheorem*{Prop}{Proposition}
\newtheorem*{sol*}{\protect\solutionname}

\makeatother

\usepackage{babel}
\providecommand{\solutionname}{Solution}

\makeatletter
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% Textclass specific LaTeX commands.
\numberwithin{equation}{section}
\numberwithin{figure}{section}

\makeatother

\usepackage{babel}

\begin{document}

\subsection*{Nate D'Alesio MTH 471 Asssignment 3}


\begin{enumerate}
\item Let $f$ and $g$ be continuous functions from $\mathbb{R}$ to $\mathbb{R}$.
Let $E$ be a dense subset of $\mathbb{R}$. Use sequences
to show that $f(E)$ is dense in $f(\mathbb{R})$. 
\begin{proof}
    If $y\in f(\mathbb{R})$ and $y\in f(E)$ then we are good. Suppose $y\in f(\mathbb{R})$ and $y\not\in f(E)$. There is a $x\in\mathbb{R}$ such that $y=f(x)$. We claim $y$ is a limit point of $f(E)$. It is clear $x\not\in E$ otherwise $y\in f(E)$. Since $E$ is dense in $\mathbb{R}$, there is a sequence $\{x_n\}_{n=1}^\infty$ in $E$ such that $\lim_{n\to\infty}x_{n}=x$. Since  $f$ is continuous, $\lim_{n\to\infty}f(x_{n})=f(x)$. So if $f(x)=f(x_n)$ for some $n$, then $y=f(x)\in f(E)$, a contradiction.
\end{proof}
\item Define 
\[
f(x)=\begin{cases}
\sin\left(\frac{1}{x}\right) & \text{if \ensuremath{x\neq0}},\\
0 & \text{if \ensuremath{x=0}}.
\end{cases}
\]
Assuming that the function $g(x)=\sin x$ is continuous at all $x\in\mathbb{R}$,
show that $f(x)$ is continuous on $\mathbb{R}\backslash\left\{ 0\right\} $.
Is $f(x)$ continuous at zero? Explain.
\begin{proof}
    Since $g(x)=\sin x$ is continuous on $\mathbb{R}$ and $f(x)=\sin(\frac{1}{x})$ is a composition of $g(x)$ with $\frac{1}{x}$ which is continuous on $\mathbb{R}\backslash\left\{ 0\right\}$, then $f(x)$ is continuous on $\mathbb{R}\backslash\left\{ 0\right\}$.
    It is not continuous at zero since there is a sequence $\{x_n\}_{n=1}^\infty$ where $x_n=\frac{1}{\pi(\frac{1}{2}+n)}$, $n\in\mathbb{N}$, then $\lim_{n\to\infty}\sin(\frac{1}{x_n})$ is 1 when $n$ is even and -1 when $n$ is odd.
\end{proof}
\item Suppose that $f$ is a real-valued uniformly continuous function on
the bounded subset $E$ of $\mathbb{R}$. Prove that $f$ is bounded
on $E$. Furthermore, argue that the conclusion is false if $E$ is
not bounded. 
\begin{proof}
    Suppose $f$ is not bounded on $E$. Then for all $n\in\mathbb{N}$, there exists a $x_n\in E$ such that $\mid f(x_n)\mid > n$. We get $x_n$ to be a bounded sequence because $E$ is bounded. Then, $x_n$ has a convergent subsequence $x_{n_k}$ by the Bolzano-Weierstrass Theorem. Therefore, $x_{n_k}$ is a Cauchy sequence and is bounded since it converges. There exists $N>0$ such that $\mid f(x_{n_k})\mid \leq N$ for all $k$. However, if $k>N$, then $\mid f(x_{n_k})\mid>n_k>k>N$, a contradiction. Thus, $f$ is bounded on $E$.\\
    To show that the conclusion is false if $E$ is not bounded, consider the function $f(x) = x$ on $\mathbb{R}$. This function is uniformly continuous on $\mathbb{R}$ but is not bounded.
\end{proof}
\item Suppose that $f:[0,1]\rightarrow[0,1]$ is continuous. Prove that
there is an $x\in[0,1]$ for which $f(x)=x$. 
\item We define a function $f:X\rightarrow Y$ to be \emph{open} if $f\left(V\right)$
is an open set in $Y$ for every open $V$ in $X$. Prove that every
continuous open function from $\mathbb{R}$ to $\mathbb{R}$ is strictly
monotonic. 
\item In this problem you will prove the following theorem:\\
\\
\textbf{Theorem: }Let $f$ be monotonically increasing on $\left(a,b\right)$.
(That is, for $x<y$ is $(a,b)$ we have $f(x)\leq f(y)$.) Denote
$\lim_{x\to x_{0}^{+}}f(x)$ by $f\left(x_{0}+\right)$ and denote
$\lim_{x\to x_{0}^{-}}f(x)$ by $f\left(x_{0}-\right)$. Then $f\left(y-\right)$
and $f\left(y+\right)$ exist for every $y\in\left(a,b\right)$. More
precisely,
\[
\sup\left\{ f(t):a<t<x\right\} =f\left(x-\right)\leq f\left(x\right)\leq f\left(x+\right)=\inf\left\{ f(t):x<t<b\right\} .
\]
Furthermore, if $a<x<y<b$, then $f\left(x+\right)\leq f\left(x-\right)$.

\begin{proof}
    For $x\in(a,b)$, the set $\left\{ f(t):a<t<x\right\}$ is bounded above by the increasing function $f(x)$. Since the set is non-empty and bounded above, there exists an $A$ in the set such that $A=\sup\left\{ f(t):a<t<x\right\}$ by the Completeness Axiom. Given $\epsilon>0$, $A-\epsilon$ is not an upper bound to $\left\{ f(t):a<t<x\right\}$. There is a $t\in(a,b)$ such that $A-\epsilon<f(t)\leq A$. Then, there exists a $\delta>0$ such that $f(x-\delta)\geq f(t)$ where $A-\epsilon<f(x-\delta)\leq A$. Since $f$ is increasing, if $x-\delta<t<x$, then $f(x-\delta)\leq f(t)\leq A$. Therefore, $A-\epsilon<f(t)$ and we get $\mid f(t)-A\mid < \epsilon$. We conclude that $f(x-)=A$.\\
    \\
    For $y\in(a,b)$ in $\left\{ f(t):y<t<b\right\}$, it is bounded below by the increasing function $f(y)$. Since the set is non-empty and bounded below, there exists a $B$
    in the set such that $B=\inf\left\{ f(t):y<t<b\right\}$ by the Completeness Axiom. Since $B$ is the greatest lower bound, given $\epsilon>0$, there exists a $t\in(a,b)$ where $B\leq f(t)<B+\epsilon$. Then, there exists a $\delta>0$ such that $f(y+\delta)\leq f(t)$ where $B\leq f(y+\delta)<B+\epsilon$. Since $f$ is increasing, if $y<t<y+\delta$, then $f(y)\leq f(t)\leq f(y+\delta)$. Therefore, $B+\epsilon> f(t)$ and we get $\mid f(t)-B\mid < \epsilon$. Thus, $f(y+)=B$.\\
    \\
    From the arguments above, 
\end{proof}
\end{enumerate}

\end{document}
