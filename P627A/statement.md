## Description

<div><p>Two <span class="tex-font-style-bf">positive</span> integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> have a sum of <span class="tex-span"><i>s</i></span> and a bitwise XOR of <span class="tex-span"><i>x</i></span>. How many possible values are there for the ordered pair <span class="tex-span">(<i>a</i>, <i>b</i>)</span>?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>s</i> ≤ 10<sup class="upper-index">12</sup></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">12</sup></span>), the sum and bitwise xor of the pair of positive integers, respectively.</p></div><div class="output-specification"><p>Print a single integer, the number of solutions to the given conditions. If no solutions exist, print <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>s</i> ≤ 10<sup class="upper-index">12</sup></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">12</sup></span>), the sum and bitwise xor of the pair of positive integers, respectively.</p>

## Output

<p>Print a single integer, the number of solutions to the given conditions. If no solutions exist, print <span class="tex-span">0</span>.</p>





```input1
9 5

```




```input2
3 3

```




```input3
5 2

```




```output1
4

```




```output2
2

```




```output3
0

```



## Note

<p>In the first sample, we have the following solutions: <span class="tex-span">(2, 7)</span>, <span class="tex-span">(3, 6)</span>, <span class="tex-span">(6, 3)</span>, <span class="tex-span">(7, 2)</span>.</p><p>In the second sample, the only solutions are <span class="tex-span">(1, 2)</span> and <span class="tex-span">(2, 1)</span>.</p>
