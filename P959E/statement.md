## Description

<div><p>Ehab is interested in the bitwise-xor operation and the special graphs. Mahmoud gave him a problem that combines both. He has a complete graph consisting of <span class="tex-span"><i>n</i></span> vertices numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>. For all <span class="tex-span">0 ≤ <i>u</i> &lt; <i>v</i> &lt; <i>n</i></span>, vertex <span class="tex-span"><i>u</i></span> and vertex <span class="tex-span"><i>v</i></span> are connected with an undirected edge that has weight <img align="middle" class="tex-formula" src="file://04dl606X.png" style="max-width: 100.0%;max-height: 100.0%;"> (where <img align="middle" class="tex-formula" src="file://kYi2abKg.png" style="max-width: 100.0%;max-height: 100.0%;"> is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise-xor operation</a>). Can you find the weight of the minimum spanning tree of that graph?</p><p>You can read about complete graphs in <a href="https://en.wikipedia.org/wiki/Complete_graph">https://en.wikipedia.org/wiki/Complete_graph</a></p><p>You can read about the minimum spanning tree in <a href="https://en.wikipedia.org/wiki/Minimum_spanning_tree">https://en.wikipedia.org/wiki/Minimum_spanning_tree</a></p><p>The weight of the minimum spanning tree is the sum of the weights on the edges included in it.</p></div><div class="input-specification"><p>The only line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup>)</span>, the number of vertices in the graph.</p></div><div class="output-specification"><p>The only line contains an integer <span class="tex-span"><i>x</i></span>, the weight of the graph's minimum spanning tree.</p></div>

## Input

<p>The only line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup>)</span>, the number of vertices in the graph.</p>

## Output

<p>The only line contains an integer <span class="tex-span"><i>x</i></span>, the weight of the graph's minimum spanning tree.</p>





```input1
4

```




```output1
4
```



## Note

<p>In the first sample: <img class="tex-graphics" src="file://qnPE7afL.png" style="max-width: 100.0%;max-height: 100.0%;"> The weight of the minimum spanning tree is 1+2+1=4.</p>
