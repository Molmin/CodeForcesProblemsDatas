## Description

<div><p>One day Masha came home and noticed <span class="tex-span"><i>n</i></span> mice in the corridor of her flat. Of course, she shouted loudly, so scared mice started to run to the holes in the corridor.</p><p>The corridor can be represeted as a numeric axis with <span class="tex-span"><i>n</i></span> mice and <span class="tex-span"><i>m</i></span> holes on it. <span class="tex-span"><i>i</i></span>th mouse is at the coordinate <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>j</i></span>th hole — at coordinate <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span>. <span class="tex-span"><i>j</i></span>th hole has enough room for <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> mice, so not more than <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> mice can enter this hole.</p><p>What is the minimum sum of distances that mice have to go through so that they all can hide in the holes? If <span class="tex-span"><i>i</i></span>th mouse goes to the hole <span class="tex-span"><i>j</i></span>, then its distance is <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>p</i><sub class="lower-index"><i>j</i></sub>|</span>.</p><p>Print the minimum sum of distances.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>) — the number of mice and the number of holes, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the coordinate of <span class="tex-span"><i>i</i></span>th mouse.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain pairs of integer numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub>, <i>c</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 5000</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> is the coordinate of <span class="tex-span"><i>j</i></span>th hole, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> is the maximum number of mice that can hide in the hole <span class="tex-span"><i>j</i></span>.</p></div><div class="output-specification"><p>Print one integer number — the minimum sum of distances. If there is no solution, print <span class="tex-font-style-tt">-1</span> instead.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>) — the number of mice and the number of holes, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the coordinate of <span class="tex-span"><i>i</i></span>th mouse.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain pairs of integer numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub>, <i>c</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 5000</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> is the coordinate of <span class="tex-span"><i>j</i></span>th hole, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> is the maximum number of mice that can hide in the hole <span class="tex-span"><i>j</i></span>.</p>

## Output

<p>Print one integer number — the minimum sum of distances. If there is no solution, print <span class="tex-font-style-tt">-1</span> instead.</p>





```input1
4 5
6 2 8 9
3 6
2 1
3 6
4 7
4 7

```




```input2
7 2
10 20 30 40 50 45 35
-1000000000 10
1000000000 1

```




```output1
11

```




```output2
7000000130

```


