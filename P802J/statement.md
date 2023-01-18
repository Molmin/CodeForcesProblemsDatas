## Description

<div><p>Heidi's friend Jenny is asking Heidi to deliver an important letter to one of their common friends. Since Jenny is Irish, Heidi thinks that this might be a prank. More precisely, she suspects that the message she is asked to deliver states: "Send the fool further!", and upon reading it the recipient will ask Heidi to deliver the same message to yet another friend (that the recipient has in common with Heidi), and so on.</p><p>Heidi believes that her friends want to avoid awkward situations, so she will not be made to visit the same person (including Jenny) twice. She also knows how much it costs to travel between any two of her friends who know each other. She wants to know: what is the maximal amount of money she will waste on travel if it really is a prank?</p><p>Heidi's <span class="tex-span"><i>n</i></span> friends are labeled <span class="tex-span">0</span> through <span class="tex-span"><i>n</i> - 1</span>, and their network of connections forms a tree. In other words, every two of her friends <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> know each other, possibly indirectly (there is a sequence of friends starting from <span class="tex-span"><i>a</i></span> and ending on <span class="tex-span"><i>b</i></span> and such that each two consecutive friends in the sequence know each other directly), and there are exactly <span class="tex-span"><i>n</i> - 1</span> pairs of friends who know each other directly.</p><p>Jenny is given the number <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line of the input contains the number of friends <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>). The next <span class="tex-span"><i>n</i> - 1</span> lines each contain three space-separated integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">4</sup></span>), meaning that <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are friends (know each other directly) and the cost for travelling between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> is <span class="tex-span"><i>c</i></span>.</p><p>It is guaranteed that the social network of the input forms a tree.</p></div><div class="output-specification"><p>Output a single integer – the maximum sum of costs.</p></div>

## Input

<p>The first line of the input contains the number of friends <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>). The next <span class="tex-span"><i>n</i> - 1</span> lines each contain three space-separated integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">4</sup></span>), meaning that <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are friends (know each other directly) and the cost for travelling between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> is <span class="tex-span"><i>c</i></span>.</p><p>It is guaranteed that the social network of the input forms a tree.</p>

## Output

<p>Output a single integer – the maximum sum of costs.</p>





```input1
4
0 1 4
0 2 2
2 3 3

```




```input2
6
1 2 3
0 2 100
1 4 2
0 3 7
3 5 10

```




```input3
11
1 0 1664
2 0 881
3 2 4670
4 2 1555
5 1 1870
6 2 1265
7 2 288
8 7 2266
9 2 1536
10 6 3378

```




```output1
5

```




```output2
105

```




```output3
5551

```



## Note

<p>In the second example, the worst-case scenario goes like this: Jenny sends Heidi to the friend labeled by number <span class="tex-span">2</span> (incurring a cost of <span class="tex-span">100</span>), then friend <span class="tex-span">2</span> sends her to friend <span class="tex-span">1</span> (costing Heidi <span class="tex-span">3</span>), and finally friend <span class="tex-span">1</span> relays her to friend <span class="tex-span">4</span> (incurring an additional cost of <span class="tex-span">2</span>).</p>
