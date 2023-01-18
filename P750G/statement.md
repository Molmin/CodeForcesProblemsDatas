## Description

<div><p>The New Year tree is an infinite perfect binary tree rooted in the node <span class="tex-span">1</span>. Each node <span class="tex-span"><i>v</i></span> has two children: nodes indexed <span class="tex-span">(2·<i>v</i>)</span> and <span class="tex-span">(2·<i>v</i> + 1)</span>.</p><center> <img class="tex-graphics" src="file://DLT7loVP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Polar bears love decorating the New Year tree and Limak is no exception. As he is only a little bear, he was told to decorate only one simple path between some pair of nodes. Though he was given an opportunity to pick the pair himself! Now he wants to know the number of unordered pairs of indices <span class="tex-span">(<i>u</i>, <i>v</i>)</span> (<span class="tex-span"><i>u</i> ≤ <i>v</i></span>), such that the sum of indices of all nodes along the simple path between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (including endpoints) is equal to <span class="tex-span"><i>s</i></span>. Can you help him and count this value?</p></div><div class="input-specification"><p>The only line of the input contains a single integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ 10<sup class="upper-index">15</sup></span>).</p></div><div class="output-specification"><p>Print one integer, denoting the number of unordered pairs of nodes indices defining simple paths with the sum of indices of vertices equal to <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The only line of the input contains a single integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ 10<sup class="upper-index">15</sup></span>).</p>

## Output

<p>Print one integer, denoting the number of unordered pairs of nodes indices defining simple paths with the sum of indices of vertices equal to <span class="tex-span"><i>s</i></span>.</p>





```input1
10

```




```output1
4

```



## Note

<p>In sample test, there are <span class="tex-span">4</span> paths with the sum of indices equal to <span class="tex-span">10</span>:</p><center> <img class="tex-graphics" src="file://fdjWBhxr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
