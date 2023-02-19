## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Come, let's build a world where even the weak are not forgotten!</span></div><div class="epigraph-source">—Kijin Seija, <span class="tex-font-style-it">Double Dealing Characters</span></div></div><p>Shinmyoumaru has a mallet that can turn objects bigger or smaller. She is testing it out on a sequence $a$ and a number $v$ whose initial value is $1$. She wants to make $v = \gcd\limits_{i\ne j}\{a_i\cdot a_j\}$ by <span class="tex-font-style-bf">no more than</span> $10^5$ operations ($\gcd\limits_{i\ne j}\{a_i\cdot a_j\}$ denotes the $\gcd$ of all products of two distinct elements of the sequence $a$). </p><p>In each operation, she picks a subsequence $b$ of $a$, and does one of the followings: </p><ul> <li> <span class="tex-font-style-bf">Enlarge</span>: $v = v \cdot \mathrm{lcm}(b)$ </li><li> <span class="tex-font-style-bf">Reduce</span>: $v = \frac{v}{\mathrm{lcm}(b)}$ </li></ul><p>Note that she does <span class="tex-font-style-bf">not</span> need to guarantee that $v$ is an integer, that is, $v$ does <span class="tex-font-style-bf">not</span> need to be a multiple of $\mathrm{lcm}(b)$ when performing Reduce.</p><p>Moreover, she wants to guarantee that the total length of $b$ chosen over the operations does not exceed $10^6$. Fine a possible operation sequence for her. <span class="tex-font-style-bf">You don't need to minimize anything</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2\leq n\leq 10^5$) — the size of sequence $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\cdots,a_n$ ($1\leq a_i\leq 10^6$) — the sequence $a$.</p><p>It can be shown that the answer exists.</p></div><div class="output-specification"><p>The first line contains a non-negative integer $k$ ($0\leq k\leq 10^5$) — the number of operations.</p><p>The following $k$ lines contains several integers. For each line, the first two integers $f$ ($f\in\{0,1\}$) and $p$ ($1\le p\le n$) stand for the option you choose ($0$ for Enlarge and $1$ for Reduce) and the length of $b$. The other $p$ integers of the line $i_1,i_2,\ldots,i_p$ ($1\le i_1&lt;i_2&lt;\ldots&lt;i_p\le n$) represents the indexes of the subsequence. Formally, $b_j=a_{i_j}$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2\leq n\leq 10^5$) — the size of sequence $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\cdots,a_n$ ($1\leq a_i\leq 10^6$) — the sequence $a$.</p><p>It can be shown that the answer exists.</p>

## Output

<p>The first line contains a non-negative integer $k$ ($0\leq k\leq 10^5$) — the number of operations.</p><p>The following $k$ lines contains several integers. For each line, the first two integers $f$ ($f\in\{0,1\}$) and $p$ ($1\le p\le n$) stand for the option you choose ($0$ for Enlarge and $1$ for Reduce) and the length of $b$. The other $p$ integers of the line $i_1,i_2,\ldots,i_p$ ($1\le i_1&lt;i_2&lt;\ldots&lt;i_p\le n$) represents the indexes of the subsequence. Formally, $b_j=a_{i_j}$.</p>





```input1
3
6 10 15
```




```input2
4
2 4 8 16
```




```output1
1
0 3 1 2 3
```




```output2
2
0 1 4
1 1 1
```



## Note

<p>Test case 1:</p><p>$\gcd\limits_{i\ne j}\{a_i\cdot a_j\}=\gcd\{60,90,150\}=30$.</p><p>Perform $v = v\cdot \operatorname{lcm}\{a_1,a_2,a_3\}=30$.</p><p>Test case 2:</p><p>$\gcd\limits_{i\ne j}\{a_i\cdot a_j\}=8$.</p><p>Perform $v = v\cdot \operatorname{lcm}\{a_4\}=16$.</p><p>Perform $v = \frac{v}{\operatorname{lcm}\{a_1\}}=8$.</p>
