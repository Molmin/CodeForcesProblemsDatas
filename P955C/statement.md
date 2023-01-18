## Description

<div><p>You're given <span class="tex-span"><i>Q</i></span> queries of the form <span class="tex-span">(<i>L</i>, <i>R</i>)</span>. </p><p>For each query you have to find the number of such <span class="tex-span"><i>x</i></span> that <span class="tex-span"><i>L</i> ≤ <i>x</i> ≤ <i>R</i></span> and there exist integer numbers <span class="tex-span"><i>a</i> &gt; 0</span>, <span class="tex-span"><i>p</i> &gt; 1</span> such that <span class="tex-span"><i>x</i> = <i>a</i><sup class="upper-index"><i>p</i></sup></span>.</p></div><div class="input-specification"><p>The first line contains the number of queries <span class="tex-span"><i>Q</i></span> <span class="tex-span">(1 ≤ <i>Q</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next <span class="tex-span"><i>Q</i></span> lines contains two integers <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>R</i></span> each <span class="tex-span">(1 ≤ <i>L</i> ≤ <i>R</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>Q</i></span> lines — the answers to the queries.</p></div>

## Input

<p>The first line contains the number of queries <span class="tex-span"><i>Q</i></span> <span class="tex-span">(1 ≤ <i>Q</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next <span class="tex-span"><i>Q</i></span> lines contains two integers <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>R</i></span> each <span class="tex-span">(1 ≤ <i>L</i> ≤ <i>R</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p>

## Output

<p>Output <span class="tex-span"><i>Q</i></span> lines — the answers to the queries.</p>





```input1
6
1 4
9 9
5 7
12 29
137 591
1 1000000

```




```output1
2
1
0
3
17
1111

```



## Note

<p>In query one the suitable numbers are <span class="tex-span">1</span> and <span class="tex-span">4</span>. </p>
