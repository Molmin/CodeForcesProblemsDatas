## Description

<div><p>Demiurges Shambambukli and Mazukta love to watch the games of ordinary people. Today, they noticed two men who play the following game.</p><p>There is a rooted tree on <span class="tex-span"><i>n</i></span> nodes, <span class="tex-span"><i>m</i></span> of which are <span class="tex-font-style-it">leaves</span> (a leaf is a nodes that does not have any children), edges of the tree are directed from parent to children. In the leaves of the tree integers from 1 to <span class="tex-span"><i>m</i></span> are placed in such a way that each number appears exactly in one leaf.</p><p>Initially, the root of the tree contains a piece. Two players move this piece in turns, during a move a player moves the piece from its current nodes to one of its children; if the player can not make a move, the game ends immediately. The <span class="tex-font-style-it">result</span> of the game is the number placed in the leaf where a piece has completed its movement. The player who makes the first move tries to maximize the result of the game and the second player, on the contrary, tries to minimize the result. We can assume that both players move optimally well.</p><p>Demiurges are omnipotent, so before the game they can arbitrarily rearrange the numbers placed in the leaves. Shambambukli wants to rearrange numbers so that the result of the game when both players play optimally well is as large as possible, and Mazukta wants the result to be as small as possible. What will be the outcome of the game, if the numbers are rearranged by Shambambukli, and what will it be if the numbers are rearranged by Mazukta? Of course, the Demiurges choose the best possible option of arranging numbers.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of nodes in the tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the ends of the edge of the tree; the edge leads from node <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to node <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the described graph is a rooted tree, and the root is the node 1.</p></div><div class="output-specification"><p>Print two space-separated integers — the maximum possible and the minimum possible result of the game.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of nodes in the tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the ends of the edge of the tree; the edge leads from node <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to node <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the described graph is a rooted tree, and the root is the node 1.</p>

## Output

<p>Print two space-separated integers — the maximum possible and the minimum possible result of the game.</p>





```input1
5
1 2
1 3
2 4
2 5

```




```input2
6
1 2
1 3
3 4
1 5
5 6

```




```output1
3 2

```




```output2
3 3

```



## Note

<p>Consider the first sample. The tree contains three leaves: 3, 4 and 5. If we put the maximum number 3 at node 3, then the first player moves there and the result will be 3. On the other hand, it is easy to see that for any rearrangement the first player can guarantee the result of at least 2.</p><p>In the second sample no matter what the arragment is the first player can go along the path that ends with a leaf with number 3.</p>
