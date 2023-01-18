## Description

<div><p><span class="tex-font-style-it">Permutation</span> <span class="tex-span"><i>p</i></span> is an ordered set of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,   <i>p</i><sub class="lower-index">2</sub>,   ...,   <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct positive integers not larger than <span class="tex-span"><i>n</i></span>. We'll denote as <span class="tex-span"><i>n</i></span> the length of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,   <i>p</i><sub class="lower-index">2</sub>,   ...,   <i>p</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Your task is to find such permutation <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span>, that the group of numbers <span class="tex-span">|<i>p</i><sub class="lower-index">1</sub> - <i>p</i><sub class="lower-index">2</sub>|, |<i>p</i><sub class="lower-index">2</sub> - <i>p</i><sub class="lower-index">3</sub>|, ..., |<i>p</i><sub class="lower-index"><i>n</i> - 1</sub> - <i>p</i><sub class="lower-index"><i>n</i></sub>|</span> has exactly <span class="tex-span"><i>k</i></span> distinct elements.</p></div><div class="input-specification"><p>The single line of the input contains two space-separated positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers forming the permutation. If there are multiple answers, print any of them.</p></div>

## Input

<p>The single line of the input contains two space-separated positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers forming the permutation. If there are multiple answers, print any of them.</p>





```input1
3 2

```




```input2
3 1

```




```input3
5 2

```




```output1
1 3 2

```




```output2
1 2 3

```




```output3
1 3 2 4 5

```



## Note

<p>By <span class="tex-span">|<i>x</i>|</span> we denote the absolute value of number <span class="tex-span"><i>x</i></span>. </p>
