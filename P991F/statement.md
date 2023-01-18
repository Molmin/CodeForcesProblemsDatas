## Description

<div><p>Vasya is a regular participant at programming contests and is already experienced in finding important sentences in long statements. Of course, numbers constraints are important&nbsp;— factorization of a number less than <span class="tex-font-style-tt">1000000</span> is easier than of a number less than <span class="tex-font-style-tt">1000000000</span>. However, sometimes it's hard to understand the number at the first glance. Could it be shortened? For example, instead of <span class="tex-font-style-tt">1000000</span> you could write $10^{6}$, instead of <span class="tex-font-style-tt">1000000000</span> &nbsp;—$10^{9}$, instead of <span class="tex-font-style-tt">1000000007</span>&nbsp;— $10^{9}+7$.</p><p>Vasya decided that, to be concise, the notation should follow several rules: </p><ul> <li> the notation should only consist of numbers, operations of addition ("<span class="tex-font-style-tt">+</span>"), multiplication ("<span class="tex-font-style-tt">*</span>") and exponentiation ("<span class="tex-font-style-tt">^</span>"), in particular, the use of braces is forbidden; </li><li> the use of several exponentiation operations in a row is forbidden, for example, writing "<span class="tex-font-style-tt">2^3^4</span>" is unacceptable; </li><li> the value of the resulting expression equals to the initial number; </li><li> the notation should consist of the minimal amount of symbols. </li></ul><p>Given $n$, find the equivalent concise notation for it.</p></div><div class="input-specification"><p>The only line contains a single integer $n$ ($1 \leq n \leq 10\,000\,000\,000$).</p></div><div class="output-specification"><p>Output a concise notation of the number $n$. If there are several concise notations, output any of them.</p></div>

## Input

<p>The only line contains a single integer $n$ ($1 \leq n \leq 10\,000\,000\,000$).</p>

## Output

<p>Output a concise notation of the number $n$. If there are several concise notations, output any of them.</p>





```input1
2018

```




```input2
1000000007

```




```input3
10000000000

```




```input4
2000000000

```




```output1
2018

```




```output2
10^9+7

```




```output3
100^5

```




```output4
2*10^9

```



## Note

<p>The third sample allows the answer <span class="tex-font-style-tt">10^10</span> also of the length $5$.</p>
