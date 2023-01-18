## Description

<div><p>Dreamoon wants to climb up a stair of <span class="tex-span"><i>n</i></span> steps. He can climb <span class="tex-span">1</span> or <span class="tex-span">2</span> steps at each move. Dreamoon wants the number of moves to be a multiple of an integer <span class="tex-span"><i>m</i></span>. </p><p>What is the minimal number of moves making him climb to the top of the stairs that satisfies his condition?</p></div><div class="input-specification"><p>The single line contains two space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 &lt; <i>n</i> ≤ 10000, 1 &lt; <i>m</i> ≤ 10</span>).</p></div><div class="output-specification"><p>Print a single integer — the minimal number of moves being a multiple of <span class="tex-span"><i>m</i></span>. If there is no way he can climb satisfying condition print <span class="tex-span"> - 1</span> instead.</p></div>

## Input

<p>The single line contains two space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 &lt; <i>n</i> ≤ 10000, 1 &lt; <i>m</i> ≤ 10</span>).</p>

## Output

<p>Print a single integer — the minimal number of moves being a multiple of <span class="tex-span"><i>m</i></span>. If there is no way he can climb satisfying condition print <span class="tex-span"> - 1</span> instead.</p>





```input1
10 2

```




```input2
3 5

```




```output1
6

```




```output2
-1

```



## Note

<p>For the first sample, Dreamoon could climb in 6 moves with following sequence of steps: {2, 2, 2, 2, 1, 1}.</p><p>For the second sample, there are only three valid sequence of steps {2, 1}, {1, 2}, {1, 1, 1} with 2, 2, and 3 steps respectively. All these numbers are not multiples of 5.</p>
