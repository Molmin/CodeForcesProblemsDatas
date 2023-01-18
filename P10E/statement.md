## Description

<div><p>Billy investigates the question of applying greedy algorithm to different spheres of life. At the moment he is studying the application of greedy algorithm to the problem about change. There is an amount of <span class="tex-span"><i>n</i></span> coins of different face values, and the coins of each value are not limited in number. The task is to collect the sum <span class="tex-span"><i>x</i></span> with the minimum amount of coins. Greedy algorithm with each its step takes the coin of the highest face value, not exceeding <span class="tex-span"><i>x</i></span>. Obviously, if among the coins' face values exists the face value 1, any sum <span class="tex-span"><i>x</i></span> can be collected with the help of greedy algorithm. However, greedy algorithm does not always give the optimal representation of the sum, i.e. the representation with the minimum amount of coins. For example, if there are face values <span class="tex-span">{1, 3, 4}</span> and it is asked to collect the sum <span class="tex-span">6</span>, greedy algorithm will represent the sum as <span class="tex-span">4 + 1 + 1</span>, while the optimal representation is <span class="tex-span">3 + 3</span>, containing one coin less. By the given set of face values find out if there exist such a sum <span class="tex-span"><i>x</i></span> that greedy algorithm will collect in a non-optimal way. If such a sum exists, find out the smallest of these sums.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 400</span>) — the amount of the coins' face values. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), describing the face values. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &gt; <i>a</i><sub class="lower-index">2</sub> &gt; ... &gt; <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = 1</span>.</p></div><div class="output-specification"><p>If greedy algorithm collects any sum in an optimal way, output -1. Otherwise output the smallest sum that greedy algorithm collects in a non-optimal way.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 400</span>) — the amount of the coins' face values. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), describing the face values. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &gt; <i>a</i><sub class="lower-index">2</sub> &gt; ... &gt; <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = 1</span>.</p>

## Output

<p>If greedy algorithm collects any sum in an optimal way, output -1. Otherwise output the smallest sum that greedy algorithm collects in a non-optimal way.</p>





```input1
5
25 10 5 2 1

```




```input2
3
4 3 1

```




```output1
-1

```




```output2
6

```


