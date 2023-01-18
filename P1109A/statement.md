## Description

<div><p>Sasha likes programming. Once, during a very long contest, Sasha decided that he was a bit tired and needed to relax. So he did. But since Sasha isn't an ordinary guy, he prefers to relax unusually. During leisure time Sasha likes to upsolve unsolved problems because upsolving is very useful.</p><p>Therefore, Sasha decided to upsolve the following problem:</p><p>You have an array $a$ with $n$ integers. You need to count the number of <span class="tex-font-style-it">funny</span> pairs $(l, r)$ $(l \leq r)$. To check if a pair $(l, r)$ is a <span class="tex-font-style-it">funny</span> pair, take $mid = \frac{l + r - 1}{2}$, then if $r - l + 1$ is an <span class="tex-font-style-bf">even</span> number and $a_l \oplus a_{l+1} \oplus \ldots \oplus a_{mid} = a_{mid + 1} \oplus a_{mid + 2} \oplus \ldots \oplus a_r$, then the pair is <span class="tex-font-style-it">funny</span>. In other words, $\oplus$ of elements of the left half of the subarray from $l$ to $r$ should be equal to $\oplus$ of elements of the right half. Note that $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>It is time to continue solving the contest, so Sasha asked you to solve this task.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 3 \cdot 10^5$)&nbsp;— the size of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{20}$)&nbsp;— array itself.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of <span class="tex-font-style-it">funny</span> pairs. You should consider only pairs where $r - l + 1$ is even number.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 3 \cdot 10^5$)&nbsp;— the size of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{20}$)&nbsp;— array itself.</p>

## Output

<p>Print one integer&nbsp;— the number of <span class="tex-font-style-it">funny</span> pairs. You should consider only pairs where $r - l + 1$ is even number.</p>





```input1
5
1 2 3 4 5

```




```input2
6
3 2 2 3 7 6

```




```input3
3
42 4 2

```




```output1
1

```




```output2
3

```




```output3
0

```



## Note

<p><span class="tex-font-style-it">Be as cool as Sasha, upsolve problems!</span></p><p>In the first example, the only <span class="tex-font-style-it">funny</span> pair is $(2, 5)$, as $2 \oplus 3 = 4 \oplus 5 = 1$.</p><p>In the second example, funny pairs are $(2, 3)$, $(1, 4)$, and $(3, 6)$.</p><p>In the third example, there are no <span class="tex-font-style-it">funny</span> pairs.</p>
