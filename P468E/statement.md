## Description

<div><p>Little X has solved the #P-complete problem in polynomial time recently. So he gives this task to you. </p><p>There is a special <span class="tex-span"><i>n</i> × <i>n</i></span> matrix <span class="tex-span"><i>A</i></span>, you should calculate its permanent modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>. The special property of matrix <span class="tex-span"><i>A</i></span> is almost all its elements equal to <span class="tex-span">1</span>. Only <span class="tex-span"><i>k</i></span> elements have specified value.</p><p>You can find the definition of permanent at the link: <span class="tex-font-style-tt">https://en.wikipedia.org/wiki/Permanent</span></p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>k</i> ≤ 50</span>).</p><p>The next <span class="tex-span"><i>k</i></span> lines contain the description of the matrix. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>,  <i>y</i><sub class="lower-index"><i>i</i></sub> ≤  <i>n</i>;&nbsp;0  ≤  <i>w</i><sub class="lower-index"><i>i</i></sub>  ≤ 10<sup class="upper-index">9</sup></span>). These numbers denote that <span class="tex-span"><i>A</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></sub> = <i>w</i><sub class="lower-index"><i>i</i></sub></span>. All the elements of the matrix except of the given elements are equal to <span class="tex-span">1</span>.</p><p>It's guaranteed that all the positions <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> are distinct.</p></div><div class="output-specification"><p>Print the permanent of the matrix modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup>  +  7)</span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>k</i> ≤ 50</span>).</p><p>The next <span class="tex-span"><i>k</i></span> lines contain the description of the matrix. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>,  <i>y</i><sub class="lower-index"><i>i</i></sub> ≤  <i>n</i>;&nbsp;0  ≤  <i>w</i><sub class="lower-index"><i>i</i></sub>  ≤ 10<sup class="upper-index">9</sup></span>). These numbers denote that <span class="tex-span"><i>A</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></sub> = <i>w</i><sub class="lower-index"><i>i</i></sub></span>. All the elements of the matrix except of the given elements are equal to <span class="tex-span">1</span>.</p><p>It's guaranteed that all the positions <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> are distinct.</p>

## Output

<p>Print the permanent of the matrix modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup>  +  7)</span>.</p>





```input1
3 1
1 1 2

```




```input2
10 10
3 3 367056794
6 2 124561273
1 3 46718146
6 9 415916869
10 5 985968336
3 1 526792265
1 4 386357058
10 4 349304187
2 7 102032499
3 6 502679075

```




```output1
8

```




```output2
233333333

```


