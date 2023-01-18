## Description

<div><p>Little Dima misbehaved during a math lesson a lot and the nasty teacher Mr. Pickles gave him the following problem as a punishment. </p><p>Find all integer solutions <span class="tex-span"><i>x</i></span> <span class="tex-span">(0 &lt; <i>x</i> &lt; 10<sup class="upper-index">9</sup>)</span> of the equation:</p><center class="tex-equation"><span class="tex-span"><i>x</i> = <i>b</i>·<i>s</i>(<i>x</i>)<sup class="upper-index"><i>a</i></sup> + <i>c</i>, </span></center> <p>where <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> are some predetermined constant values and function <span class="tex-span"><i>s</i>(<i>x</i>)</span> determines the sum of all digits in the decimal representation of number <span class="tex-span"><i>x</i></span>.</p><p>The teacher gives this problem to Dima for each lesson. He changes only the parameters of the equation: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>. Dima got sick of getting bad marks and he asks you to help him solve this challenging problem.</p></div><div class="input-specification"><p>The first line contains three space-separated integers: <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 5;&nbsp;1 ≤ <i>b</i> ≤ 10000;&nbsp; - 10000 ≤ <i>c</i> ≤ 10000)</span>.</p></div><div class="output-specification"><p>Print integer <span class="tex-span"><i>n</i></span> — the number of the solutions that you've found. Next print <span class="tex-span"><i>n</i></span> integers in the increasing order — the solutions of the given equation. Print only integer solutions that are larger than zero and strictly less than <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div>

## Input

<p>The first line contains three space-separated integers: <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 5;&nbsp;1 ≤ <i>b</i> ≤ 10000;&nbsp; - 10000 ≤ <i>c</i> ≤ 10000)</span>.</p>

## Output

<p>Print integer <span class="tex-span"><i>n</i></span> — the number of the solutions that you've found. Next print <span class="tex-span"><i>n</i></span> integers in the increasing order — the solutions of the given equation. Print only integer solutions that are larger than zero and strictly less than <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>





```input1
3 2 8

```




```input2
1 2 -18

```




```input3
2 2 -1

```




```output1
3
10 2008 13726
```




```output2
0

```




```output3
4
1 31 337 967
```


