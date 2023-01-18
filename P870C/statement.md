## Description

<div><p>You are given several queries. In the <span class="tex-span"><i>i</i></span>-th query you are given a single positive integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span>. You are to represent <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> as a sum of maximum possible number of composite summands and print this maximum number, or print <span class="tex-font-style-tt">-1</span>, if there are no such splittings.</p><p>An integer greater than <span class="tex-span">1</span> is composite, if it is not prime, i.e. if it has positive divisors not equal to <span class="tex-span">1</span> and the integer itself.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p><span class="tex-span"><i>q</i></span> lines follow. The (<span class="tex-span"><i>i</i> + 1</span>)-th line contains single integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>For each query print the maximum possible number of summands in a valid splitting to composite summands, or <span class="tex-font-style-tt">-1</span>, if there are no such splittings.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p><span class="tex-span"><i>q</i></span> lines follow. The (<span class="tex-span"><i>i</i> + 1</span>)-th line contains single integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>For each query print the maximum possible number of summands in a valid splitting to composite summands, or <span class="tex-font-style-tt">-1</span>, if there are no such splittings.</p>





```input1
1
12

```




```input2
2
6
8

```




```input3
3
1
2
3

```




```output1
3

```




```output2
1
2

```




```output3
-1
-1
-1

```



## Note

<p><span class="tex-span">12 = 4 + 4 + 4 = 4 + 8 = 6 + 6 = 12</span>, but the first splitting has the maximum possible number of summands.</p><p><span class="tex-span">8 = 4 + 4</span>, <span class="tex-span">6</span> can't be split into several composite summands.</p><p><span class="tex-span">1, 2, 3</span> are less than any composite number, so they do not have valid splittings.</p>
