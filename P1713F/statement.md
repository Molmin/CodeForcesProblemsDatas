## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">My orzlers, we can optimize this problem from $O(S^3)$ to $O\left(T^\frac{5}{9}\right)$!</span></div><div class="epigraph-source">— Spyofgame, founder of Orzlim religion</div></div><p>A long time ago, Spyofgame invented the famous array $a$ ($1$-indexed) of length $n$ that contains information about the world and life. After that, he decided to convert it into the matrix $b$ ($0$-indexed) of size $(n + 1) \times (n + 1)$ which contains information about the world, life and beyond.</p><p>Spyofgame converted $a$ into $b$ with the following rules.</p><ul> <li> $b_{i,0} = 0$ if $0 \leq i \leq n$; </li><li> $b_{0,i} = a_{i}$ if $1 \leq i \leq n$; </li><li> $b_{i,j} = b_{i,j-1} \oplus b_{i-1,j}$ if $1 \leq i, j \leq n$. </li></ul><p>Here $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Today, archaeologists have discovered the famous matrix $b$. However, many elements of the matrix has been lost. They only know the values of $b_{i,n}$ for $1 \leq i \leq n$ (note that these are some elements of the last <span class="tex-font-style-bf">column</span>, not the last <span class="tex-font-style-bf">row</span>).</p><p>The archaeologists want to know what a possible array of $a$ is. Can you help them reconstruct any array that could be $a$?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $b_{1,n}, b_{2,n}, \ldots, b_{n,n}$ ($0 \leq b_{i,n} &lt; 2^{30}$).</p></div><div class="output-specification"><p>If some array $a$ is consistent with the information, print a line containing $n$ integers $a_1, a_2, \ldots, a_n$. If there are multiple solutions, output any.</p><p>If such an array does not exist, output $-1$ instead.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $b_{1,n}, b_{2,n}, \ldots, b_{n,n}$ ($0 \leq b_{i,n} &lt; 2^{30}$).</p>

## Output

<p>If some array $a$ is consistent with the information, print a line containing $n$ integers $a_1, a_2, \ldots, a_n$. If there are multiple solutions, output any.</p><p>If such an array does not exist, output $-1$ instead.</p>





```input1
3
0 2 1
```




```input2
1
199633
```




```input3
10
346484077 532933626 858787727 369947090 299437981 416813461 865836801 141384800 157794568 691345607
```




```output1
1 2 3
```




```output2
199633
```




```output3
725081944 922153789 481174947 427448285 516570428 509717938 855104873 280317429 281091129 1050390365
```



## Note

<p>If we let $a = [1,2,3]$, then $b$ will be:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\bf{0}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\bf{1}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\bf{2}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\bf{3}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\bf{0}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\bf{0}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\bf{0}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr></tbody></table> </center><p>The values of $b_{1,n}, b_{2,n}, \ldots, b_{n,n}$ generated are $[0,2,1]$ which is consistent with what the archaeologists have discovered.</p>
