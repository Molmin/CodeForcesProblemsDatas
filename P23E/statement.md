## Description

<div><p>Recently Bob invented a new game with a tree (we should remind you, that a tree is a connected graph without cycles): he deletes any (possibly, zero) amount of edges of the tree, and counts the product of sizes of the connected components left after the deletion. Your task is to find out the maximum number that Bob can get in his new game for a given tree.</p></div><div class="input-specification"><p>The first input line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 700</span>) — amount of vertices in the tree. The following <span class="tex-span"><i>n</i> - 1</span> lines contain the description of the edges. Each line contains the pair of vertices' indexes, joined by an edge, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It's guaranteed that the graph described in the input is a tree.</p></div><div class="output-specification"><p>Output the only number — the maximum product of sizes of the connected components, that Bob can get after deleting some of the tree's edges.</p></div>

## Input

<p>The first input line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 700</span>) — amount of vertices in the tree. The following <span class="tex-span"><i>n</i> - 1</span> lines contain the description of the edges. Each line contains the pair of vertices' indexes, joined by an edge, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It's guaranteed that the graph described in the input is a tree.</p>

## Output

<p>Output the only number — the maximum product of sizes of the connected components, that Bob can get after deleting some of the tree's edges.</p>





```input1
5
1 2
2 3
3 4
4 5

```




```input2
8
1 2
1 3
2 4
2 5
3 6
3 7
6 8

```




```input3
3
1 2
1 3

```




```output1
6
```




```output2
18
```




```output3
3
```


