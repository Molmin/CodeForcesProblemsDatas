## Description

<div><p>Pavel is going to make a game of his dream. However, he knows that he can't make it on his own so he founded a development company and hired <span class="tex-span"><i>n</i></span> workers of staff. Now he wants to pick <span class="tex-span"><i>n</i></span> workers from the staff who will be directly responsible for developing a game.</p><p>Each worker has a certain skill level <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Besides, each worker doesn't want to work with the one whose skill is very different. In other words, the <span class="tex-span"><i>i</i></span>-th worker won't work with those whose skill is less than <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, and with those whose skill is more than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Pavel understands that the game of his dream isn't too hard to develop, so the worker with any skill will be equally useful. That's why he wants to pick a team of the maximum possible size. Help him pick such team.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of workers Pavel hired.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the minimum skill value of the workers that the <span class="tex-span"><i>i</i></span>-th worker can work with, the <span class="tex-span"><i>i</i></span>-th worker's skill and the maximum skill value of the workers that the <span class="tex-span"><i>i</i></span>-th worker can work with.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>m</i></span>&nbsp;— the number of workers Pavel must pick for developing the game.</p><p>In the next line print <span class="tex-span"><i>m</i></span> space-separated integers&nbsp;— the numbers of the workers in any order.</p><p>If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of workers Pavel hired.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the minimum skill value of the workers that the <span class="tex-span"><i>i</i></span>-th worker can work with, the <span class="tex-span"><i>i</i></span>-th worker's skill and the maximum skill value of the workers that the <span class="tex-span"><i>i</i></span>-th worker can work with.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>m</i></span>&nbsp;— the number of workers Pavel must pick for developing the game.</p><p>In the next line print <span class="tex-span"><i>m</i></span> space-separated integers&nbsp;— the numbers of the workers in any order.</p><p>If there are multiple optimal solutions, print any of them.</p>





```input1
4
2 8 9
1 4 7
3 6 8
5 8 10

```




```input2
6
3 5 16
1 6 11
4 8 12
7 9 16
2 10 14
8 13 15

```




```output1
3
1 3 4

```




```output2
4
1 2 3 5

```


