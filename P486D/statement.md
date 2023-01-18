## Description

<div><p>As you know, an undirected connected graph with <span class="tex-span"><i>n</i></span> nodes and <span class="tex-span"><i>n</i> - 1</span> edges is called a <span class="tex-font-style-underline">tree</span>. You are given an integer <span class="tex-span"><i>d</i></span> and a tree consisting of <span class="tex-span"><i>n</i></span> nodes. Each node <span class="tex-span"><i>i</i></span> has a value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> associated with it.</p><p>We call a set <span class="tex-span"><i>S</i></span> of tree nodes <span class="tex-font-style-underline">valid</span> if following conditions are satisfied:</p><ol><li> <span class="tex-span"><i>S</i></span> is non-empty.</li><li> <span class="tex-span"><i>S</i></span> is connected. In other words, if nodes <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are in <span class="tex-span"><i>S</i></span>, then all nodes lying on the simple path between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> should also be presented in <span class="tex-span"><i>S</i></span>.</li><li> <img align="middle" class="tex-formula" src="file://Syux5pUQ.png" style="max-width: 100.0%;max-height: 100.0%;">.</li></ol><p>Your task is to count the number of valid sets. Since the result can be very large, you must print its remainder modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>d</i></span> (<span class="tex-span">0 ≤ <i>d</i> ≤ 2000</span>) and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>(<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>).</p><p>Then the next <span class="tex-span"><i>n</i> - 1</span> line each contain pair of integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) denoting that there is an edge between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It is guaranteed that these edges form a tree.</p></div><div class="output-specification"><p>Print the number of valid sets modulo <span class="tex-span">1000000007</span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>d</i></span> (<span class="tex-span">0 ≤ <i>d</i> ≤ 2000</span>) and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>(<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>).</p><p>Then the next <span class="tex-span"><i>n</i> - 1</span> line each contain pair of integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) denoting that there is an edge between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It is guaranteed that these edges form a tree.</p>

## Output

<p>Print the number of valid sets modulo <span class="tex-span">1000000007</span>.</p>





```input1
1 4
2 1 3 2
1 2
1 3
3 4

```




```input2
0 3
1 2 3
1 2
2 3

```




```input3
4 8
7 8 7 5 4 6 4 10
1 6
1 2
5 8
1 3
3 5
6 7
3 4

```




```output1
8

```




```output2
3

```




```output3
41

```



## Note

<p>In the first sample, there are exactly 8 valid sets: <span class="tex-span">{1}, {2}, {3}, {4}, {1, 2}, {1, 3}, {3, 4}</span> and <span class="tex-span">{1, 3, 4}</span>. Set <span class="tex-span">{1, 2, 3, 4}</span> is not valid, because the third condition isn't satisfied. Set <span class="tex-span">{1, 4}</span> satisfies the third condition, but conflicts with the second condition.</p>
