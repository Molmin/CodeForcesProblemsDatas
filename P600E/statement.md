## Description

<div><p>You are given a rooted tree with root in vertex <span class="tex-span">1</span>. Each vertex is coloured in some colour.</p><p>Let's call colour <span class="tex-span"><i>c</i></span> dominating in the subtree of vertex <span class="tex-span"><i>v</i></span> if there are no other colours that appear in the subtree of vertex <span class="tex-span"><i>v</i></span> more times than colour <span class="tex-span"><i>c</i></span>. So it's possible that two or more colours will be dominating in the subtree of some vertex.</p><p>The subtree of vertex <span class="tex-span"><i>v</i></span> is the vertex <span class="tex-span"><i>v</i></span> and all other vertices that contains vertex <span class="tex-span"><i>v</i></span> in each path to the root.</p><p>For each vertex <span class="tex-span"><i>v</i></span> find the sum of all dominating colours in the subtree of vertex <span class="tex-span"><i>v</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the colour of the <span class="tex-span"><i>i</i></span>-th vertex.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the edge of the tree. The first vertex is the root of the tree.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers — the sums of dominating colours for each vertex.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the colour of the <span class="tex-span"><i>i</i></span>-th vertex.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the edge of the tree. The first vertex is the root of the tree.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers — the sums of dominating colours for each vertex.</p>





```input1
4
1 2 3 4
1 2
2 3
2 4

```




```input2
15
1 2 3 1 2 3 3 1 1 3 2 2 1 2 3
1 2
1 3
1 4
1 14
1 15
2 5
2 6
2 7
3 8
3 9
3 10
4 11
4 12
4 13

```




```output1
10 9 3 4

```




```output2
6 5 4 3 2 3 3 1 1 3 2 2 1 2 3

```


