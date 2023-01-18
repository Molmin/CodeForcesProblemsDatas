## Description

<div><p>Memory is now interested in the de-evolution of objects, specifically triangles. He starts with an equilateral triangle of side length <span class="tex-span"><i>x</i></span>, and he wishes to perform operations to obtain an equilateral triangle of side length <span class="tex-span"><i>y</i></span>.</p><p>In a single second, he can modify the length of a single side of the current triangle such that it remains a non-degenerate triangle (triangle of positive area). At any moment of time, the length of each side should be integer.</p><p>What is the minimum number of seconds required for Memory to obtain the equilateral triangle of side length <span class="tex-span"><i>y</i></span>?</p></div><div class="input-specification"><p>The first and only line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">3 ≤ <i>y</i> &lt; <i>x</i> ≤ 100 000</span>)&nbsp;— the starting and ending equilateral triangle side lengths respectively.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of seconds required for Memory to obtain the equilateral triangle of side length <span class="tex-span"><i>y</i></span> if he starts with the equilateral triangle of side length <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The first and only line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">3 ≤ <i>y</i> &lt; <i>x</i> ≤ 100 000</span>)&nbsp;— the starting and ending equilateral triangle side lengths respectively.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of seconds required for Memory to obtain the equilateral triangle of side length <span class="tex-span"><i>y</i></span> if he starts with the equilateral triangle of side length <span class="tex-span"><i>x</i></span>.</p>





```input1
6 3

```




```input2
8 5

```




```input3
22 4

```




```output1
4

```




```output2
3

```




```output3
6

```



## Note

<p>In the first sample test, Memory starts with an equilateral triangle of side length <span class="tex-span">6</span> and wants one of side length <span class="tex-span">3</span>. Denote a triangle with sides <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>c</i></span> as <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span>. Then, Memory can do <img align="middle" class="tex-formula" src="file://47NgH4qO.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample test, Memory can do <img align="middle" class="tex-formula" src="file://efMh3W9b.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third sample test, Memory can do: <img align="middle" class="tex-formula" src="file://JNnKeppk.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://kBiIH0Rp.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
