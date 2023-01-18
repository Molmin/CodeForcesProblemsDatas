## Description

<div><p>When Darth Vader gets bored, he sits down on the sofa, closes his eyes and thinks of an infinite rooted tree where each node has exactly <span class="tex-span"><i>n</i></span> sons, at that for each node, the distance between it an its <span class="tex-span"><i>i</i></span>-th left child equals to <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. The Sith Lord loves counting the number of nodes in the tree that are at a distance at most <span class="tex-span"><i>x</i></span> from the root. The distance is the sum of the lengths of edges on the path between nodes.</p><p>But he has got used to this activity and even grew bored of it. 'Why does he do that, then?' — you may ask. It's just that he feels superior knowing that only he can solve this problem. </p><p>Do you want to challenge Darth Vader himself? Count the required number of nodes. As the answer can be rather large, find it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of children of each node and the distance from the root within the range of which you need to count the nodes.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the length of the edge that connects each node with its <span class="tex-span"><i>i</i></span>-th child.</p></div><div class="output-specification"><p>Print a single number — the number of vertexes in the tree at distance from the root equal to at most <span class="tex-span"><i>x</i></span>. </p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of children of each node and the distance from the root within the range of which you need to count the nodes.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the length of the edge that connects each node with its <span class="tex-span"><i>i</i></span>-th child.</p>

## Output

<p>Print a single number — the number of vertexes in the tree at distance from the root equal to at most <span class="tex-span"><i>x</i></span>. </p>





```input1
3 3
1 2 3

```




```output1
8

```



## Note

<p>Pictures to the sample (the yellow color marks the nodes the distance to which is at most three)</p><center> <img class="tex-graphics" src="file://qPNkV7zx.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
