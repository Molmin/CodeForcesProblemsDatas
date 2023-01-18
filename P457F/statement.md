## Description

<div><p>Pieguy and Piegirl are playing a game. They have a rooted binary tree, that has a property that each node is either a leaf or has exactly two children. Each leaf has a number associated with it.</p><p>On his/her turn a player can choose any two leafs that share their immediate parent, remove them, and associate either of their values with their parent, that now became a leaf (the player decides which of the two values to associate). The game ends when only one node (the one that was the root of the tree) is left.</p><p>Pieguy goes first, and his goal is to maximize the value that will be associated with the root when the game ends. Piegirl wants to minimize that value. Assuming that both players are playing optimally, what number will be associated with the root when the game ends?</p></div><div class="input-specification"><p>First line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>) — number of test cases. Then <span class="tex-span"><i>t</i></span> test cases follow. Each test case begins with an empty line, followed by a line with a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 250</span>), followed by <span class="tex-span"><i>n</i></span> lines describing <span class="tex-span"><i>n</i></span> nodes of the tree. Each of those <span class="tex-span"><i>n</i></span> lines either contains a non-negative number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, indicating a leaf node with value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) associated with it, or <span class="tex-span"> - 1</span> followed by integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, indicating a non-leaf node with children <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>l</i>, <i>r</i> ≤ <i>n</i> - 1</span>). Nodes are numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>. The root is always node <span class="tex-span">0</span>.</p></div><div class="output-specification"><p>For each test case print one line with one integer on it — the number that will be associated with the root when the game ends.</p></div>

## Input

<p>First line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>) — number of test cases. Then <span class="tex-span"><i>t</i></span> test cases follow. Each test case begins with an empty line, followed by a line with a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 250</span>), followed by <span class="tex-span"><i>n</i></span> lines describing <span class="tex-span"><i>n</i></span> nodes of the tree. Each of those <span class="tex-span"><i>n</i></span> lines either contains a non-negative number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, indicating a leaf node with value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) associated with it, or <span class="tex-span"> - 1</span> followed by integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, indicating a non-leaf node with children <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>l</i>, <i>r</i> ≤ <i>n</i> - 1</span>). Nodes are numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>. The root is always node <span class="tex-span">0</span>.</p>

## Output

<p>For each test case print one line with one integer on it — the number that will be associated with the root when the game ends.</p>





```input1
4

3
-1 1 2
10
5

5
-1 1 2
-1 3 4
10
5
20

7
-1 1 2
-1 3 4
-1 5 6
1
2
3
4

11
-1 1 2
-1 3 4
-1 5 6
-1 7 8
15
7
-1 9 10
7
8
9
11

```




```output1
10
10
4
8

```


