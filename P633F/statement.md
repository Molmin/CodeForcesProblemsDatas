## Description

<div><p>Alice and Bob have a tree (undirected acyclic connected graph). There are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> chocolates waiting to be picked up in the <span class="tex-span"><i>i</i></span>-th vertex of the tree. First, they choose two different vertices as their starting positions (Alice chooses first) and take all the chocolates contained in them.</p><p>Then, they alternate their moves, selecting one vertex at a time and collecting all chocolates from this node. To make things more interesting, they decided that one can select a vertex only if he/she selected a vertex adjacent to that one at his/her previous turn and this vertex has not been already chosen by any of them during other move.</p><p>If at any moment one of them is not able to select the node that satisfy all the rules, he/she will skip his turns and let the other person pick chocolates as long as he/she can. This goes on until both of them cannot pick chocolates any further.</p><p>Due to their greed for chocolates, they want to collect as many chocolates as possible. However, as they are friends they only care about the total number of chocolates they obtain <span class="tex-font-style-bf">together</span>. What is the maximum total number of chocolates they may pick?</p></div><div class="input-specification"><p>The first line of the input contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ </span>n<span class="tex-span"> ≤ 100 000</span>)&nbsp;— the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>i</i></span>-th of these numbers stands for the number of chocolates stored at the node <span class="tex-span"><i>i</i></span>.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines that describe the tree. Each of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of vertices connected by the <span class="tex-span"><i>i</i></span>-th edge.</p></div><div class="output-specification"><p>Print the number of chocolates Alice and Bob can collect together if they behave optimally.</p></div>

## Input

<p>The first line of the input contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ </span>n<span class="tex-span"> ≤ 100 000</span>)&nbsp;— the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>i</i></span>-th of these numbers stands for the number of chocolates stored at the node <span class="tex-span"><i>i</i></span>.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines that describe the tree. Each of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of vertices connected by the <span class="tex-span"><i>i</i></span>-th edge.</p>

## Output

<p>Print the number of chocolates Alice and Bob can collect together if they behave optimally.</p>





```input1
9
1 2 3 4 5 6 7 8 9
1 2
1 3
1 4
1 5
1 6
1 7
1 8
1 9

```




```input2
2
20 10
1 2

```




```output1
25

```




```output2
30

```



## Note

<p>In the first sample, Alice may start at the vertex <span class="tex-span">9</span> and Bob at vertex <span class="tex-span">8</span>. Alice will select vertex <span class="tex-span">1</span> and Bob has no options now. Alice selects the vertex <span class="tex-span">7</span> and they both stop.</p><p>In the second sample, both of them will pick either of the nodes alternately.</p>
