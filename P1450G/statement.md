## Description

<div><p><span class="tex-font-style-bf">Please pay attention to the unusual memory limit in this problem.</span></p><p><span class="tex-font-style-it">In a parallel universe, Satan is called "Trygub". For that reason, the letters of his namesake were deleted from the alphabet in ancient times.</span></p><p>The government has $n$ workers standing in a row and numbered with integers from $1$ to $n$ from left to right. Their job categories can be represented as a string $s$ of length $n$, where the character $s_i$ represents the job category of the $i$-th worker.</p><p>A new law will be approved to increase the equality between the workers. The government decided to make everyone have the same job category by performing the following operation any number of times (possibly zero).</p><p>There is a fixed <span class="tex-font-style-bf">rational</span> parameter $k=\frac ab$ describing how easy it is to convince the public, and it will be used to determine the success of an operation.</p><p>In an operation, the government first selects a job category $x$ with at least one worker at the current moment. Suppose $i_1,\ldots, i_m$ ($i_1&lt;\ldots&lt;i_m$) are the positions of all the workers with job category $x$. If $k\cdot (i_m-i_1+1)\le m$, the government is able to choose any job category $y$ with at least one worker at the current moment and change the job category of <span class="tex-font-style-bf">all</span> workers with job category $x$ to job category $y$.</p><p>If it is possible to make all workers have job category $x$, we say that $x$ is obtainable. Can you tell the government the set of obtainable job categories?</p></div><div class="input-specification"><p>The first line contains three integers $n, a, b$ ($1 \le n \le 5000$, $1\le a\le b\le 10^5$) — the number of workers and the numerator and denominator of the parameter $k$, respectively.</p><p>The second line contains a string $s$ of length $n$, consisting of lowercase English characters — the job categories of each worker. <span class="tex-font-style-bf">The characters '<span class="tex-font-style-tt">t</span>', '<span class="tex-font-style-tt">r</span>', '<span class="tex-font-style-tt">y</span>', '<span class="tex-font-style-tt">g</span>', '<span class="tex-font-style-tt">u</span>', and '<span class="tex-font-style-tt">b</span>' do not appear in the string $s$.</span></p></div><div class="output-specification"><p>Print an integer $c$ equal to the number of obtainable job categories followed by $c$ space-separated characters&nbsp;— the obtainable job categories sorted in the lexicographical order.</p></div>

## Input

<p>The first line contains three integers $n, a, b$ ($1 \le n \le 5000$, $1\le a\le b\le 10^5$) — the number of workers and the numerator and denominator of the parameter $k$, respectively.</p><p>The second line contains a string $s$ of length $n$, consisting of lowercase English characters — the job categories of each worker. <span class="tex-font-style-bf">The characters '<span class="tex-font-style-tt">t</span>', '<span class="tex-font-style-tt">r</span>', '<span class="tex-font-style-tt">y</span>', '<span class="tex-font-style-tt">g</span>', '<span class="tex-font-style-tt">u</span>', and '<span class="tex-font-style-tt">b</span>' do not appear in the string $s$.</span></p>

## Output

<p>Print an integer $c$ equal to the number of obtainable job categories followed by $c$ space-separated characters&nbsp;— the obtainable job categories sorted in the lexicographical order.</p>





```input1
7 1 2
comicom
```




```output1
3 c m o
```



## Note

<p>The first operation must select the job category '<span class="tex-font-style-tt">i</span>' because all other job categories cannot satisfy the condition, therefore '<span class="tex-font-style-tt">i</span>' is not obtainable.</p><p>Below is showed how to obtain '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">m</span>', and '<span class="tex-font-style-tt">o</span>'. The square brackets denote the segment containing all workers of the selected category, the red color denotes this category and the blue color denotes the new category after the change.</p><ul><li> Get '<span class="tex-font-style-tt">c</span>': <ol> <li> ($\texttt{com}\color{red}{\texttt{[i]}}\texttt{com} \rightarrow \texttt{com}\color{#1E90FF}{\texttt{[o]}}\texttt{com}$) </li><li> ($\texttt{c}\color{red}{\texttt{[o}}\texttt{m}\color{red}{\texttt{o}}\texttt{c}\color{red}{\texttt{o]}}\texttt{m} \rightarrow \texttt{c}\color{#1E90FF}{\texttt{[m}}\texttt{m}\color{#1E90FF}{\texttt{m}}\texttt{c}\color{#1E90FF}{\texttt{m]}}\texttt{m}$) </li><li> ($\texttt{c}\color{red}{\texttt{[mmm}}\texttt{c}\color{red}{\texttt{mm]}} \rightarrow \texttt{c}\color{#1E90FF}{\texttt{[ccc}}\texttt{c}\color{#1E90FF}{\texttt{cc]}}$) </li></ol></li><li> Get '<span class="tex-font-style-tt">m</span>': <ol> <li> ($\texttt{com}\color{red}{\texttt{[i]}}\texttt{com} \rightarrow \texttt{com}\color{#1E90FF}{\texttt{[o]}}\texttt{com}$) </li><li> ($\texttt{c}\color{red}{\texttt{[o}}\texttt{m}\color{red}{\texttt{o}}\texttt{c}\color{red}{\texttt{o]}}\texttt{m} \rightarrow \texttt{c}\color{#1E90FF}{\texttt{[c}}\texttt{m}\color{#1E90FF}{\texttt{c}}\texttt{c}\color{#1E90FF}{\texttt{c]}}\texttt{m}$) </li><li> ($\color{red}{\texttt{[cc}}\texttt{m}\color{red}{\texttt{ccc]}}\texttt{m} \rightarrow \color{#1E90FF}{\texttt{[mm}}\texttt{m}\color{#1E90FF}{\texttt{mmm]}}\texttt{m}$) </li></ol></li><li> Get '<span class="tex-font-style-tt">o</span>': <ol> <li> ($\texttt{com}\color{red}{\texttt{[i]}}\texttt{com} \rightarrow \texttt{com}\color{#1E90FF}{\texttt{[c]}}\texttt{com}$) </li><li> ($\color{red}{\texttt{[c}}\texttt{om}\color{red}{\texttt{cc]}}\texttt{om} \rightarrow \color{#1E90FF}{\texttt{[m}}\texttt{om}\color{#1E90FF}{\texttt{mm]}}\texttt{om}$) </li><li> ($\color{red}{\texttt{[m}}\texttt{o}\color{red}{\texttt{mmm}}\texttt{o}\color{red}{\texttt{m]}} \rightarrow \color{#1E90FF}{\texttt{[o}}\texttt{o}\color{#1E90FF}{\texttt{ooo}}\texttt{o}\color{#1E90FF}{\texttt{o]}}$) </li></ol></li></ul>
