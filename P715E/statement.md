## Description

<div><p>ZS the Coder is given two permutations <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> of <span class="tex-span">{1, 2, ..., <i>n</i>}</span>, but some of their elements are replaced with <span class="tex-span">0</span>. The <span class="tex-font-style-it">distance</span> between two permutations <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> is defined as the minimum number of moves required to turn <span class="tex-span"><i>p</i></span> into <span class="tex-span"><i>q</i></span>. A move consists of swapping exactly <span class="tex-span">2</span> elements of <span class="tex-span"><i>p</i></span>.</p><p>ZS the Coder wants to determine the number of ways to replace the zeros with positive integers from the set <span class="tex-span">{1, 2, ..., <i>n</i>}</span> such that <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are permutations of <span class="tex-span">{1, 2, ..., <i>n</i>}</span> and the distance between <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> is exactly <span class="tex-span"><i>k</i></span>.</p><p>ZS the Coder wants to find the answer for all <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i> - 1</span>. Can you help him?</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 250</span>)&nbsp;— the number of elements in the permutations.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the permutation <span class="tex-span"><i>p</i></span>. It is guaranteed that there is at least one way to replace zeros such that <span class="tex-span"><i>p</i></span> is a permutation of <span class="tex-span">{1, 2, ..., <i>n</i>}</span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the permutation <span class="tex-span"><i>q</i></span>. It is guaranteed that there is at least one way to replace zeros such that <span class="tex-span"><i>q</i></span> is a permutation of <span class="tex-span">{1, 2, ..., <i>n</i>}</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>i</i></span>-th of them should denote the answer for <span class="tex-span"><i>k</i> = <i>i</i> - 1</span>. Since the answer may be quite large, and ZS the Coder loves weird primes, print them modulo <span class="tex-span">998244353 = 2<sup class="upper-index">23</sup>·7·17 + 1</span>, which is a prime.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 250</span>)&nbsp;— the number of elements in the permutations.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the permutation <span class="tex-span"><i>p</i></span>. It is guaranteed that there is at least one way to replace zeros such that <span class="tex-span"><i>p</i></span> is a permutation of <span class="tex-span">{1, 2, ..., <i>n</i>}</span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the permutation <span class="tex-span"><i>q</i></span>. It is guaranteed that there is at least one way to replace zeros such that <span class="tex-span"><i>q</i></span> is a permutation of <span class="tex-span">{1, 2, ..., <i>n</i>}</span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>i</i></span>-th of them should denote the answer for <span class="tex-span"><i>k</i> = <i>i</i> - 1</span>. Since the answer may be quite large, and ZS the Coder loves weird primes, print them modulo <span class="tex-span">998244353 = 2<sup class="upper-index">23</sup>·7·17 + 1</span>, which is a prime.</p>





```input1
3
1 0 0
0 2 0

```




```input2
4
1 0 0 3
0 0 0 4

```




```input3
6
1 3 2 5 4 6
6 4 5 1 0 0

```




```input4
4
1 2 3 4
2 3 4 1

```




```output1
1 2 1 

```




```output2
0 2 6 4 

```




```output3
0 0 0 0 1 1 

```




```output4
0 0 0 1 

```



## Note

<p>In the first sample case, there is the only way to replace zeros so that it takes <span class="tex-span">0</span> swaps to convert <span class="tex-span"><i>p</i></span> into <span class="tex-span"><i>q</i></span>, namely <span class="tex-span"><i>p</i> = (1, 2, 3), <i>q</i> = (1, 2, 3)</span>.</p><p>There are two ways to replace zeros so that it takes <span class="tex-span">1</span> swap to turn <span class="tex-span"><i>p</i></span> into <span class="tex-span"><i>q</i></span>. One of these ways is <span class="tex-span"><i>p</i> = (1, 2, 3), <i>q</i> = (3, 2, 1)</span>, then swapping <span class="tex-span">1</span> and <span class="tex-span">3</span> from <span class="tex-span"><i>p</i></span> transform it into <span class="tex-span"><i>q</i></span>. The other way is <span class="tex-span"><i>p</i> = (1, 3, 2), <i>q</i> = (1, 2, 3)</span>. Swapping <span class="tex-span">2</span> and <span class="tex-span">3</span> works in this case.</p><p>Finally, there is one way to replace zeros so that it takes <span class="tex-span">2</span> swaps to turn <span class="tex-span"><i>p</i></span> into <span class="tex-span"><i>q</i></span>, namely <span class="tex-span"><i>p</i> = (1, 3, 2), <i>q</i> = (3, 2, 1)</span>. Then, we can transform <span class="tex-span"><i>p</i></span> into <span class="tex-span"><i>q</i></span> like following: <img align="middle" class="tex-formula" src="file://glsXKmAt.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
