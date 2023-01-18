## Description

<div><p>You are given an infinite checkered field. You should get from a square (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) to a square (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>). Using the shortest path is not necessary. You can move on the field squares in four directions. That is, when you are positioned in any square, you can move to any other side-neighboring one. </p><p>A square (<span class="tex-span"><i>x</i></span>; <span class="tex-span"><i>y</i></span>) is considered bad, if at least one of the two conditions is fulfilled:</p><ul><li> <span class="tex-span">|<i>x</i> + <i>y</i>| ≡ 0</span> <span class="tex-span">(<i>mod</i>&nbsp;2<i>a</i>)</span>,</li><li> <span class="tex-span">|<i>x</i> - <i>y</i>| ≡ 0</span> <span class="tex-span">(<i>mod</i>&nbsp;2<i>b</i>)</span>.</li></ul> <p>Your task is to find the minimum number of bad cells one will have to visit on the way from (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) to (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>).</p></div><div class="input-specification"><p>The only line contains integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — the parameters of the bad squares, the coordinates of the initial and the final squares correspondingly (<span class="tex-span">2 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span> and <span class="tex-span">|<i>x</i><sub class="lower-index">1</sub>|</span>,<span class="tex-span">|<i>y</i><sub class="lower-index">1</sub>|</span>,<span class="tex-span">|<i>x</i><sub class="lower-index">2</sub>|</span>,<span class="tex-span">|<i>y</i><sub class="lower-index">2</sub>| ≤ 10<sup class="upper-index">9</sup></span>). It is guaranteed that the initial and the final square aren't bad.</p></div><div class="output-specification"><p>Print a single number — the minimum number of bad cells that one will have to visit in order to travel from square (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) to square (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>).</p></div>

## Input

<p>The only line contains integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — the parameters of the bad squares, the coordinates of the initial and the final squares correspondingly (<span class="tex-span">2 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span> and <span class="tex-span">|<i>x</i><sub class="lower-index">1</sub>|</span>,<span class="tex-span">|<i>y</i><sub class="lower-index">1</sub>|</span>,<span class="tex-span">|<i>x</i><sub class="lower-index">2</sub>|</span>,<span class="tex-span">|<i>y</i><sub class="lower-index">2</sub>| ≤ 10<sup class="upper-index">9</sup></span>). It is guaranteed that the initial and the final square aren't bad.</p>

## Output

<p>Print a single number — the minimum number of bad cells that one will have to visit in order to travel from square (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) to square (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>).</p>





```input1
2 2 1 0 0 1

```




```input2
2 2 10 11 0 1

```




```input3
2 4 3 -1 3 7

```




```output1
1

```




```output2
5

```




```output3
2

```



## Note

<p>In the third sample one of the possible paths in (3;-1)-&gt;(3;0)-&gt;(3;1)-&gt;(3;2)-&gt;(4;2)-&gt;(4;3)-&gt;(4;4)-&gt;(4;5)-&gt;(4;6)-&gt;(4;7)-&gt;(3;7). Squares (3;1) and (4;4) are bad.</p>
