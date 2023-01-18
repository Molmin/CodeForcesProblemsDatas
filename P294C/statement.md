## Description

<div><p>There are <span class="tex-span"><i>n</i></span> lights aligned in a row. These lights are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Initially some of the lights are switched on. Shaass wants to switch all the lights on. At each step he can switch a light on (this light should be switched off at that moment) if there's at least one adjacent light which is already switched on. </p><p>He knows the initial state of lights and he's wondering how many different ways there exist to switch all the lights on. Please find the required number of ways modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> where <span class="tex-span"><i>n</i></span> is the number of lights in the sequence and <span class="tex-span"><i>m</i></span> is the number of lights which are initially switched on, <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>m</i> ≤ <i>n</i>)</span>. The second line contains <span class="tex-span"><i>m</i></span> distinct integers, each between <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive, denoting the indices of lights which are initially switched on.</p></div><div class="output-specification"><p>In the only line of the output print the number of different possible ways to switch on all the lights modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> where <span class="tex-span"><i>n</i></span> is the number of lights in the sequence and <span class="tex-span"><i>m</i></span> is the number of lights which are initially switched on, <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>m</i> ≤ <i>n</i>)</span>. The second line contains <span class="tex-span"><i>m</i></span> distinct integers, each between <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive, denoting the indices of lights which are initially switched on.</p>

## Output

<p>In the only line of the output print the number of different possible ways to switch on all the lights modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3 1
1

```




```input2
4 2
1 4

```




```input3
11 2
4 8

```




```output1
1

```




```output2
2

```




```output3
6720

```


