## Description

<div><p>Iahub is very proud of his recent discovery, propagating trees. Right now, he invented a new tree, called xor-tree. After this new revolutionary discovery, he invented a game for kids which uses xor-trees.</p><p>The game is played on a tree having <span class="tex-span"><i>n</i></span> nodes, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each node <span class="tex-span"><i>i</i></span> has an initial value <span class="tex-span"><i>init</i><sub class="lower-index"><i>i</i></sub></span>, which is either 0 or 1. The root of the tree is node 1.</p><p>One can perform several (possibly, zero) operations on the tree during the game. The only available type of operation is to pick a node <span class="tex-span"><i>x</i></span>. Right after someone has picked node <span class="tex-span"><i>x</i></span>, the value of node <span class="tex-span"><i>x</i></span> flips, the values of sons of <span class="tex-span"><i>x</i></span> remain the same, the values of sons of sons of <span class="tex-span"><i>x</i></span> flips, the values of sons of sons of sons of <span class="tex-span"><i>x</i></span> remain the same and so on.</p><p>The goal of the game is to get each node <span class="tex-span"><i>i</i></span> to have value <span class="tex-span"><i>goal</i><sub class="lower-index"><i>i</i></sub></span>, which can also be only 0 or 1. You need to reach the goal of the game by using minimum number of operations.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>) meaning there is an edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>The next line contains <span class="tex-span"><i>n</i></span> integer numbers, the <span class="tex-span"><i>i</i></span>-th of them corresponds to <span class="tex-span"><i>init</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>init</i><sub class="lower-index"><i>i</i></sub></span> is either 0 or 1). The following line also contains <span class="tex-span"><i>n</i></span> integer numbers, the <span class="tex-span"><i>i</i></span>-th number corresponds to <span class="tex-span"><i>goal</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>goal</i><sub class="lower-index"><i>i</i></sub></span> is either 0 or 1).</p></div><div class="output-specification"><p>In the first line output an integer number <span class="tex-span"><i>cnt</i></span>, representing the minimal number of operations you perform. Each of the next <span class="tex-span"><i>cnt</i></span> lines should contain an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, representing that you pick a node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>) meaning there is an edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>The next line contains <span class="tex-span"><i>n</i></span> integer numbers, the <span class="tex-span"><i>i</i></span>-th of them corresponds to <span class="tex-span"><i>init</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>init</i><sub class="lower-index"><i>i</i></sub></span> is either 0 or 1). The following line also contains <span class="tex-span"><i>n</i></span> integer numbers, the <span class="tex-span"><i>i</i></span>-th number corresponds to <span class="tex-span"><i>goal</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>goal</i><sub class="lower-index"><i>i</i></sub></span> is either 0 or 1).</p>

## Output

<p>In the first line output an integer number <span class="tex-span"><i>cnt</i></span>, representing the minimal number of operations you perform. Each of the next <span class="tex-span"><i>cnt</i></span> lines should contain an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, representing that you pick a node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
10
2 1
3 1
4 2
5 1
6 2
7 5
8 6
9 8
10 5
1 0 1 1 0 1 0 1 0 1
1 0 1 0 0 1 1 1 0 1

```




```output1
2
4
7

```


